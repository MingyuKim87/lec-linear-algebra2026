# GitHub Pages 업로드 안내

저장소: `mgyukim87/lec-linear-algebra2026`

이 폴더의 파일은 `main`에서 관리합니다. `main`에 푸시하면 GitHub Actions가 Jekyll 사이트를 빌드하고, 완성된 파일을 `gh-pages` 브랜치에 자동으로 반영합니다. GitHub Pages는 `gh-pages`의 루트를 게시합니다.

```text
main: index.md · _config.yml · _layouts · assets
  → GitHub Actions: Jekyll 빌드
  → gh-pages: index.html · assets · .nojekyll
  → https://mgyukim87.github.io/lec-linear-algebra2026/
```

## 1. 새 저장소 만들기

GitHub에서 소유자 `mgyukim87`, 이름 `lec-linear-algebra2026`인 빈 Public 저장소를 만듭니다. 아래 명령은 README, .gitignore, License를 GitHub에서 자동 생성하지 않은 빈 저장소를 기준으로 합니다.

로컬 `docs` 폴더의 **내용 전체**를 새 저장소의 루트에 올립니다. GitHub 저장소 안에 `docs` 폴더를 한 번 더 만들지 않습니다.

```text
lec-linear-algebra2026/         ← 저장소 루트, main 브랜치
├── .github/
│   └── workflows/
│       └── deploy.yml         ← main 푸시 → 빌드 → gh-pages 자동 갱신
├── .gitignore
├── _config.yml
├── _layouts/
│   └── course.html
├── index.md
├── UPLOAD_GUIDE.md
└── assets/
    ├── css/course.css
    ├── js/course.js
    └── docs/
        ├── syllabus.pdf
        └── LinearAlgebra_2026_Textbook_Page_Mapping_Guide.pdf
```

`.github`는 숨김 폴더이지만 자동화에 필요합니다. 아래 `git add .` 명령은 이 폴더도 포함합니다. `UPLOAD_GUIDE.md`와 `.github`는 Jekyll 빌드에서 제외되어 사이트에는 게시되지 않습니다.

## 2. main에 첫 업로드

아래는 이 로컬 폴더에 아직 Git 저장소와 원격 주소를 설정하지 않은 경우의 최초 명령입니다.

```bash
cd "/Users/mgyukim/Documents/Lectures/2026_Fall/1_Linear_Algebra/docs"
git init
git branch -M main
git add .
git commit -m "Add course site and automatic gh-pages deployment"
git remote add origin https://github.com/mgyukim87/lec-linear-algebra2026.git
git push -u origin main
```

GitHub의 **Actions → Build and publish course site**에서 실행 결과를 확인합니다. 첫 빌드와 푸시가 완료되면 `gh-pages` 브랜치가 자동으로 만들어집니다. 직접 만들거나 `main`을 수동으로 병합할 필요가 없습니다.

워크플로는 같은 저장소에서 자동 발급되는 `GITHUB_TOKEN`을 사용하며, 브랜치 갱신에 필요한 `contents: write` 권한을 해당 작업에 선언했습니다. 별도의 개인 토큰을 Secrets에 등록할 필요는 없습니다.

## 3. GitHub Pages 최초 설정

`gh-pages` 브랜치가 생성된 뒤 다음 항목을 선택합니다.

1. 저장소의 **Settings → Pages**
2. **Build and deployment → Source: Deploy from a branch**
3. **Branch: gh-pages**
4. **Folder: /(root)**
5. **Save**

이 구성에서 빌드는 Actions가 담당하지만, Pages의 게시 소스는 **Deploy from a branch**입니다. 첫 설정 이후에도 화면이 게시되지 않으면 **Actions → Build and publish course site → Run workflow → Branch: main → Run workflow**로 한 번 더 실행합니다.

게시 주소:

```text
https://mgyukim87.github.io/lec-linear-algebra2026/
```

프로젝트 경로는 이미 `_config.yml`에 설정되어 있습니다.

```yaml
url: "https://mgyukim87.github.io"
baseurl: "/lec-linear-algebra2026"
```

## 4. 이후 수정 방법

항상 `main`의 `index.md`에서 수업 내용·교재 페이지·HW·시험 일정을 수정합니다. 교재 쪽수는 책에 실제로 인쇄된 번호를 사용합니다. 일반 회차에는 절 전체 범위를 표시하고, 시험·리뷰 회차에는 누적 대표 쪽수를 표시합니다. PC와 모바일이 같은 표를 사용하므로 한 번만 수정하면 됩니다.

화면 디자인은 `assets/css/course.css`, 전체 화면 구조는 `_layouts/course.html`에서 수정합니다. 첫머리의 `layout: course`를 유지하십시오.

```bash
git switch main
git pull --ff-only origin main
# index.md 등 필요한 파일 수정
git add index.md _config.yml _layouts assets .github UPLOAD_GUIDE.md
git commit -m "Update course schedule"
git push origin main
```

GitHub 웹에서 `main`의 `index.md`를 편집하고 커밋해도 같은 자동화가 실행됩니다. 다른 브랜치에서 작업했다면 `main`에 병합될 때 배포가 시작됩니다.

`gh-pages`는 빌드 결과 전용이며 다음 배포 때 새 결과로 갱신됩니다. 사이트 내용은 `main`에서 수정하십시오. 빌드가 실패하면 `gh-pages` 갱신 단계가 실행되지 않아 기존 게시본이 유지됩니다.

## 자동 배포 확인

- Actions에서 **Build and publish course site**가 성공했는지 확인합니다.
- `gh-pages` 루트에 `index.html`, `assets`, `.nojekyll`이 있는지 확인합니다.
- Pages 배포 작업까지 완료된 뒤 사이트와 PDF 링크 두 개를 확인합니다.
- `.nojekyll`은 배포 Action이 생성합니다. 이미 빌드된 HTML에 Jekyll을 다시 적용하지 않도록 하는 파일입니다.

첫 배포 이후 화면이 갱신되지 않으면 Pages의 게시 브랜치와 폴더를 다시 확인하고, Actions 탭에서 빌드 작업과 Pages 배포 작업의 오류를 확인합니다.

## 공개 업로드 대상에서 제외한 자료

이 배포 폴더에는 교재 원본·발췌 PDF, 시험 문제·답안, Quiz 정답, HW 해설, 강의자용 내부 검증 보고서를 포함하지 않습니다.

## 참고 문서

- [GitHub Pages 게시 소스 설정](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [공식 Jekyll 빌드 Action](https://github.com/actions/jekyll-build-pages)
- [gh-pages 배포 Action과 최초 배포 안내](https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-first-deployment-with-github_token)
- [gh-pages의 .nojekyll 처리](https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-enable-built-in-jekyll-enable_jekyll)
