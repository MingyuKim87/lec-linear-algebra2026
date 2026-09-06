---
layout: course
title: "Linear Algebra | Fall 2026"
permalink: /
lang: en
description: "Textbook, course overview, class format, session-by-session textbook pages, and assessment for Linear Algebra, Fall 2026."
last_modified_at: "2026-09-06"
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

The textbook provides the definitions, theorems, and examples used in our board-based lectures. The class schedule lists the full page ranges of the relevant textbook sections. The copyrighted textbook PDF is distributed only through university-approved channels.

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

Each section range runs from the start of that section to the page immediately before the next section. Exam and review sessions list selected cumulative review pages instead of new material.

<nav class="week-nav" aria-label="Jump to a week" hidden></nav>

<div class="table-scroll schedule-table" markdown="1" role="region" aria-label="30 class sessions and textbook pages">

| Week | Date | Session | Class Topic | Textbook Pages (Printed) | Deadlines & Exams |
|---:|---|---|---|---|---|
| 1 | Sep. 1, 2026 | 1 | Course Introduction; Introduction to Linear Systems | §1.1 **pp. 2–10** |  |
| 1 | Sep. 3, 2026 | 2 | Introduction to the Programming Environment (NumPy) | §1.3 **pp. 25–39**<br><small>NumPy exercises are supplemental to the textbook</small> |  |
| 2 | Sep. 8, 2026 | 3 | Gaussian Elimination | §1.2 **pp. 11–24** |  |
| 2 | Sep. 10, 2026 | 4 | Gauss–Jordan Elimination | §1.2 **pp. 11–24** |  |
| 3 | Sep. 15, 2026 | 5 | Rank | §4.9 **pp. 276–290** |  |
| 3 | Sep. 17, 2026 | 6 | Solving Linear Systems | §1.2 **pp. 11–24** + §1.6 **pp. 62–68** |  |
| 4 | Sep. 22, 2026 | 7 | Basic Applications of Linear Systems I | §1.10 **pp. 98–109** |  |
| 4 | Sep. 24, 2026 | 8 | Basic Applications of Linear Systems II | §1.10 **pp. 98–109** | <span class="badge due">HW1 due</span> |
| 5 | Sep. 29, 2026 | 9 | Matrix Basics | §1.3 **pp. 25–39** |  |
| 5 | Oct. 1, 2026 | 10 | Block Matrices | §1.3 **pp. 25–39** |  |
| 6 | Oct. 6, 2026 | 11 | Elementary Matrices | §1.5 **pp. 53–61** |  |
| 6 | Oct. 8, 2026 | 12 | Inverses | §1.4 **pp. 40–52** + §1.5 **pp. 53–61** |  |
| 7 | Oct. 13, 2026 | 13 | LU Factorization and Its Applications | §9.1 **pp. 509–518** |  |
| 7 | Oct. 15, 2026 | 14 | Applications of LU Factorization | §9.1 **pp. 509–518** |  |
| 8 | Oct. 20, 2026 | 15 | Midterm Exam | Review: §1.2, §1.10, §9.1<br><small>Selected review pages: 16–17, 99–100, 518</small> | <span class="badge due">HW2 due</span> <span class="badge exam">Midterm Exam</span> |
| 8 | Oct. 22, 2026 | 16 | Midterm Exam Review | Review: §1.2, §1.5, §1.10<br><small>Selected review pages: 18–19, 58–59, 107</small> |  |
| 9 | Oct. 27, 2026 | 17 | Linear Combination | §4.3 **pp. 220–227** |  |
| 9 | Oct. 29, 2026 | 18 | Span | §4.3 **pp. 220–227** |  |
| 10 | Nov. 3, 2026 | 19 | Linear Independence | §4.4 **pp. 228–237** |  |
| 10 | Nov. 5, 2026 | 20 | Change of Basis | §4.7 **pp. 256–262** |  |
| 11 | Nov. 10, 2026 | 21 | Null Space, Column Space | §4.8 **pp. 263–275** |  |
| 11 | Nov. 12, 2026 | 22 | Linear Transformation | §1.8 **pp. 76–89** |  |
| 12 | Nov. 17, 2026 | 23 | Projection | §3.3 **pp. 172–182** |  |
| 12 | Nov. 19, 2026 | 24 | Orthogonality | §3.3 **pp. 172–182** + §6.2 **pp. 352–360** | <span class="badge due">HW3 due</span> |
| 13 | Nov. 24, 2026 | 25 | QR Factorization | §6.3 **pp. 361–375** |  |
| 13 | Nov. 26, 2026 | 26 | Least-Squares Solutions | §6.4 **pp. 376–384** |  |
| 14 | Dec. 1, 2026 | 27 | Eigenvalues & Eigenvectors | §5.1 **pp. 291–300** |  |
| 14 | Dec. 3, 2026 | 28 | Markov Chain | §5.5 **pp. 329–340** |  |
| 15 | Dec. 8, 2026 | 29 | Applications of Markov Chains | §5.5 **pp. 329–340** |  |
| 15 | Dec. 10, 2026 | 30 | Final Exam | Review: §4.7, §5.1, §5.5, §6.4<br><small>Selected review pages: 258–259, 297–298, 336, 379–380</small> | <span class="badge due">HW4 due</span> <span class="badge exam">Final Exam</span> |

</div>

The schedule and pace may be adjusted to reflect academic arrangements or class progress. Changes will be announced in class or through official course announcements.

## Assessment
{: #assessment}

<div class="table-scroll assessment-table" markdown="1" role="region" aria-label="Assessment components and weights">

| Component | Weight | Details |
|---|---:|---|
| Midterm Exam | 25% | Covers Weeks 1–7; held in the first session of Week 8 |
| Final Exam | 25% | Covers Weeks 9–15; held in the second session of Week 15 |
| Quizzes | 20% | Session-based checks of key concepts; scores are aggregated |
| Homework | 20% | HW1–HW4 combined; 6 questions each, 24 questions in total |
| Attendance | 10% | Based on attendance records |
| **Total** | **100%** | Relative grading |

</div>

Quiz administration and grading on exam days, as well as detailed attendance criteria, will be announced separately. If this page differs from an official course announcement, the latest official announcement takes precedence.

</div>
