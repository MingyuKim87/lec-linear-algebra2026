---
layout: course
title: "Linear Algebra | Fall 2026"
permalink: /
lang: en
description: "Textbook, course overview, class format, session-by-session textbook pages and exercises, and assessment for Linear Algebra, Fall 2026."
last_modified_at: "2026-10-06"
---

<!--
  Edit course content and tables in this Markdown file.
  Screen styles: assets/css/course.css
  Textbook references use printed page numbers.
-->

<div class="course-page" markdown="1">

<header class="course-hero">
  <p class="eyebrow">Kookmin University · Fall 2026</p>
  <h1>Linear Algebra</h1>
  <p class="lead">Course Syllabus</p>
</header>

<nav class="course-nav" aria-label="Course syllabus sections">
  <a href="#textbook">Textbook</a>
  <a href="#overview">Overview</a>
  <a href="#operation">Course Format</a>
  <a href="#schedule">Schedule &amp; Pages</a>
  <a href="#assessment">Assessment</a>
</nav>

## Textbook
{: #textbook}

**Required textbook:** *Elementary Linear Algebra*, 12th Edition, Howard Anton, Chris Rorres, and Anton Kaul. Wiley, 2019.

The textbook provides the definitions, theorems, and examples used in our board-based lectures. The class schedule lists focused readings and the locations of selected exercises. The copyrighted textbook PDF is distributed only through university-approved channels.

<div class="course-note warning" markdown="1">

**Before purchasing:** The ISBN in the original syllabus differs from the ISBN on the copyright page of the course textbook PDF. Confirm the title, 12th edition, authors, and publisher, and follow the instructor's guidance when choosing a copy.

</div>

## Course Overview
{: #overview}

This course introduces vectors, matrices, and their operations, and develops the ability to model and solve engineering problems using linear systems. Topics include Gaussian and Gauss–Jordan elimination, LU and QR factorizations, vector spaces, linear transformations, least-squares solutions, eigenvalue analysis, and Markov chains, with connections to computer science applications.

### Learning Objectives

- Understand methods for solving multidimensional linear systems.
- Formulate linear systems to model engineering problems.
- Understand and apply matrix factorizations and least-squares solutions.
- Explain the meaning of eigenvalue analysis and explore applications of Markov chains in computer science.

## Course Format
{: #operation}

The course uses a **required textbook and board-based lectures**, with step-by-step explanations and worked problems. Lecture materials support the flow of the board work and provide a resource for review. Selected sessions include hands-on exercises. The second session of Week 1 introduces NumPy arrays, shape, indexing, and matrix multiplication.

- **Before class:** Read the assigned textbook sections and pages, and locate the key definitions and theorems.
- **During class:** Take notes on the calculations and reasoning developed on the board.
- **After class:** Review the session quiz and representative textbook examples.
- **Assignments:** Write all calculations and the theorems or formulas used by hand.

## Class Schedule & Textbook Pages
{: #schedule}

<div class="course-note" markdown="1">

**Page references:** All page numbers below are **printed on the textbook pages**. Use these numbers to find the assigned reading in the book.

</div>

Reading ranges identify the relevant explanations and worked examples. Exercise pages are listed separately in the **Exercises** column; they may share a page with the next section. Exam and review sessions revisit previously assigned material.

<div class="course-note" markdown="1">

**Exercises:** Numbers in the **Exercises** column refer to the numbered problems in the **Exercise Set** at the end of each textbook section (for example, `§1.2 #5–8` means problems 5 through 8 of Exercise Set 1.2). These numbers are **Exercise Set** problems, not the worked **Examples** within the text or the chapter supplementary exercises. They are review practice; graded assignments are announced separately as HW1–HW4.

</div>

**Schedule:** Topic order follows the [eCampus weekly outline](https://ecampus.kookmin.ac.kr/course/view.php?id=86283), reviewed September 29, 2026. Topics spanning a whole week are divided into two study sessions below. The final exam is in **Week 16**; its exact date will be announced.

<nav class="week-nav" aria-label="Jump to a week" hidden></nav>

<div class="table-scroll schedule-table" markdown="1" role="region" aria-label="16-week schedule, textbook readings, and selected exercises">

| Week | Date | Session | Class Topic | Reading Pages (Printed) | Exercises (Exercise Set) | Deadlines & Exams |
|---:|---|---|---|---|---|---|
| 1 | Sep. 1, 2026 | 1 | Course Introduction; Introduction to Linear Systems | §1.1 **pp. 2–8** | §1.1 **#1–4, #7–10**<br><small>pp. 8–9 · linear equations, augmented matrices, checking solutions</small> |  |
| 1 | Sep. 3, 2026 | 2 | Introduction to the Programming Environment (NumPy) | §1.3 **pp. 25–30, 35–36**<br><small>Matrix background; NumPy syntax is supplied in class</small> | §1.3 **#3(a–h), #4(a–h), #5(a–f)**<br><small>p. 37 · rework arithmetic, transpose, and matrix products in NumPy; matrix arithmetic returns in Week 6</small> |  |
| 2 | Sep. 8, 2026 | 3 | Gaussian Elimination | §1.2 **pp. 11–12, 14–15, 20** | §1.2 **#1–2, #5–8**<br><small>pp. 22–23 · echelon forms, elimination, back-substitution</small> |  |
| 2 | Sep. 10, 2026 | 4 | Gauss–Jordan Elimination | §1.2 **pp. 14–17** | §1.2 **#9–12, #31–32**<br><small>pp. 23–24 · reduced row echelon form and Gauss–Jordan elimination</small> |  |
| 3 | Sep. 15, 2026 | 5 | Structure of Solutions in Linear Systems I (1/2) | §1.1 **pp. 5–6** · §1.2 **pp. 12–14** | §1.1 **#13–16**<br><small>p. 9 · free variables and parametric descriptions of solution sets</small> |  |
| 3 | Sep. 17, 2026 | 6 | Structure of Solutions in Linear Systems I (2/2) | §1.2 **pp. 16–17, 20, 22** | §1.2 **#3(b–c), #4(b–c), #40(b)**<br><small>pp. 23–24 · general solutions from echelon forms, pivots, number of parameters</small> |  |
| 4 | Sep. 22, 2026 | 7 | Homogeneous Linear Systems | §1.2 **pp. 17–19** | §1.2 **#13–14, #17–20**<br><small>p. 23 · trivial/nontrivial solutions and free variables</small> |  |
| 4 | Sep. 24, 2026 | 8 | Structure of Solutions in Linear Systems II: Existence and Uniqueness | §1.1 **pp. 3–5** · §1.2 **pp. 21–22** | §1.2 **#23–24, #27–28**<br><small>pp. 23–24 · consistency, unique versus infinitely many solutions, compatibility conditions</small> |  |
| 5 | Sep. 29, 2026 | 9 | Scalars, Vectors, Matrices; Linear Combinations and Span | §1.3 **pp. 25–28** · §4.3 **pp. 221–224**<br><small>Numerical vectors and elimination-based examples</small> | §4.3 **#1–2, #7–8**<br><small>p. 226 · linear combinations, spanning sets, membership in a span</small> |  |
| 5 | Oct. 1, 2026 | 10 | Linear Independence and Dependence; Rank | §4.4 **pp. 228–230, 232–233** · §4.9 **pp. 276–279**<br><small>Use elimination and pivot counts; formal basis/dimension in Week 9</small> | §4.4 **#1(a–b), #2–3, #9–10** · §4.9 **#1–2, #7–8**<br><small>pp. 236–237, 287 · dependence relations, rank, nullity, maximum rank</small> |  |
| 6 | Oct. 6, 2026 | 11 | Matrix Arithmetic | §1.3 **pp. 28–30, 34–36** · §1.4 **pp. 40–43** | §1.3 **#1–2, #3(a–h), #5(a–f), #11–14**<br><small>pp. 37–38 · dimensions, arithmetic, transpose, products, Ax = b</small> |  |
| 6 | Oct. 8, 2026 | 12 | Block Matrices | §1.3 **pp. 30–34** | §1.3 **#7–10, #17–20**<br><small>pp. 37–38 · product rows/columns, column linear combinations, column–row expansions supporting partitioned multiplication</small> | <span class="badge due">HW1 due</span> |
| 7 | Oct. 13, 2026 | 13 | Elementary Matrices | §1.5 **pp. 53–57** | §1.5 **#1–8**<br><small>p. 60 · elementary matrices, inverse row operations, EA, constructing E</small> |  |
| 7 | Oct. 15, 2026 | 14 | Inverse Matrices and Solving Linear Systems | §1.4 **pp. 44–47** · §1.5 **pp. 58–59** · §1.6 **pp. 62–64** | §1.4 **#5–6** · §1.5 **#9, #11** · §1.6 **#1, #3, #9**<br><small>pp. 51, 60, 67 · 2×2 inverses, inversion algorithm, singularity, x = A⁻¹b, multiple right-hand sides</small> |  |
| 8 | Oct. 20, 2026 | 15 | Midterm Exam | Review the **Weeks 1–7** readings above<br><small>Linear systems; independence/rank; matrix arithmetic, elementary matrices, and inverses</small> | **Selected review:** §1.2 **#5, #9, #17, #23, #27** · §4.4 **#2** · §4.9 **#1** · §1.3 **#7, #17** · §1.5 **#9** · §1.6 **#3**<br><small>pp. 23–24, 236, 287, 37–38, 60, 67</small> | <span class="badge due">HW2 due</span> <span class="badge exam">Midterm Exam</span> |
| 8 | Oct. 22, 2026 | 16 | Midterm Exam Review | Revisit the **Weeks 1–7** readings for missed concepts | **Follow-up practice:** §1.2 **#6, #10, #18, #24, #28** · §4.4 **#3** · §4.9 **#2** · §1.5 **#11**<br><small>pp. 23–24, 236, 287, 60 · compare elimination, consistency, rank, and inverse methods</small> |  |
| 9 | Oct. 27, 2026 | 17 | Linear Combinations, Independence, Span and Rank; Basis and Change of Basis | §4.5 **pp. 238–245** · §4.6 **pp. 248–254** · §4.7 **pp. 256–261**<br><small>Review: §4.3 pp. 220–226; §4.4 pp. 228–236; §4.9 pp. 276–279</small> | §4.5 **#1–2, #11–13** · §4.6 **#7–8** · §4.7 **#1–2, #8–9**<br><small>pp. 246, 254, 261–262 · bases, dimension, coordinate vectors, transition matrices</small> |  |
| 9 | Oct. 29, 2026 | 18 | Null Space and Column Space | §4.8 **pp. 263–273** | §4.8 **#3–4, #9–13, #16–17**<br><small>pp. 273–274 · membership, null/row/column-space bases, pivot columns of the original matrix</small> |  |
| 10 | Nov. 3, 2026 | 19 | Linear Transformations | §1.8 **pp. 76–87** | §1.8 **#1–2, #13–16, #21–24, #27–28**<br><small>pp. 88–89 · domain/codomain, standard matrices, evaluation, linearity</small> |  |
| 10 | Nov. 5, 2026 | 20 | Inner Product | §6.1 **pp. 341–349** | §6.1 **#1–2, #9–12, #33–34**<br><small>pp. 349–350 · inner products, norms and distances, matrix/polynomial examples, inner-product axioms</small> |  |
| 11 | Nov. 10, 2026 | 21 | Orthogonality | §6.2 **pp. 352–358** · §6.3 **pp. 361–365** | §6.2 **#1–2, #7–8, #25, #27–28** · §6.3 **#1–2, #5–6**<br><small>pp. 358–359, 374 · angles, orthogonal complements, orthogonal/orthonormal sets, normalizing a basis</small> |  |
| 11 | Nov. 12, 2026 | 22 | Projection | §3.3 **pp. 175–179** · §6.3 **pp. 365–367** | §3.3 **#15–18, #37–38** · §6.3 **#19–22**<br><small>pp. 181–182, 374 · line/plane projections, perpendicular components, projection matrices</small> |  |
| 12 | Nov. 17, 2026 | 23 | QR Factorization | §6.3 **pp. 361–373**<br><small>Review orthonormal bases; focus on Gram–Schmidt and QR</small> | §6.3 **#27–32, #45–48**<br><small>p. 375 · Gram–Schmidt and constructing R from an orthonormal Q</small> |  |
| 12 | Nov. 19, 2026 | 24 | Least-Squares Solutions | §6.4 **pp. 376–383** | §6.4 **#1–10, #15–16, #23–24**<br><small>p. 384 · normal equations, residuals, column-space projection, QR least squares</small> | <span class="badge due">HW3 due</span> |
| 13 | Nov. 24, 2026 | 25 | Eigenvalues and Eigenvectors | §5.1 **pp. 291–298**<br><small>Determinant background: §2.1 pp. 118–123 (2×2 determinants, cofactors, triangular determinants)</small> | §5.1 **#1–2, #5–10, #13–14, #19–20, #25**<br><small>p. 299 · eigenpairs, characteristic equations, eigenspaces, triangular matrices, geometry</small> |  |
| 13 | Nov. 26, 2026 | 26 | Markov Chains | §5.5 **pp. 329–337**<br><small>Markov-chain focus: pp. 331–337</small> | §5.5 **#1–12**<br><small>pp. 337–338 · stochastic matrices, state vectors, regularity, steady states, transition probabilities</small> |  |
| 14 | Dec. 1, 2026 | 27 | LU Factorization and Its Applications | §9.1 **pp. 509–516** | §9.1 **#1–6**<br><small>p. 518 · triangular systems, forward/back substitution, constructing and using LU</small> |  |
| 14 | Dec. 3, 2026 | 28 | Applications of LU Factorization | §9.1 **pp. 510–517** | §9.1 **#7–8, #10–11, #13–16**<br><small>p. 518 · inverse from LU, pivoting, PLU systems, LDU</small> |  |
| 15 | Dec. 8, 2026 | 29 | Applications of Linear Systems | §1.10 **pp. 98–107** | §1.10 **#3–4, #7–8, #13–17**<br><small>pp. 108–109 · traffic networks, circuits, polynomial interpolation</small> |  |
| 15 | Dec. 10, 2026 | 30 | Applications of Markov Chains | §5.5 **pp. 331–337** | §5.5 **#13–17, #19–20**<br><small>p. 338 · applied transition models, steady states, long-term behavior</small> | <span class="badge due">HW4 due</span> |
| 16 | Dec. 15–21, 2026<br><small>Exact date TBA</small> | TBA | Final Exam | Review the **Weeks 9–15** readings above | **Review:** revisit the selected exercises for Weeks 9–15; no new set | <span class="badge exam">Final Exam</span> |

</div>

The schedule and pace may be adjusted to reflect academic arrangements or class progress. Changes will be announced in class or through official course announcements.

## Assessment
{: #assessment}

<div class="table-scroll assessment-table" markdown="1" role="region" aria-label="Assessment components and weights">

| Component | Weight | Details |
|---|---:|---|
| Midterm Exam | 25% | Covers Weeks 1–7; held in the first session of Week 8 |
| Final Exam | 25% | Covers Weeks 9–15; held in Week 16, exact date to be announced |
| Quizzes | 20% | Session-based checks of key concepts; scores are aggregated |
| Homework | 20% | HW1–HW4 combined; 20 questions each, 80 questions in total |
| Attendance | 10% | Based on attendance records |
| **Total** | **100%** | Relative grading |

</div>

Quiz administration and grading on exam days, as well as detailed attendance criteria, will be announced separately. If this page differs from an official course announcement, the latest official announcement takes precedence.

</div>
