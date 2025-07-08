---
layout: post
title: "A SAT Based Scheduler"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: Overview.png
---

Twice a year, the [Interdisciplinary Humanities Center at UC Santa Barbara](https://www.ihc.ucsb.edu/) matches volunteer language interpreters with student-teacher conferences throughout the Goleta and Santa Barbara school districts. After a few successful iterations, the demand for interpreters increased enough to justify the application of a sophisticated scheduling system. In this project, I teamed up with the _Interdisciplinary Humanities Center_ to develop such a system, utilizing [Google's CP-SAT Solver](https://developers.google.com/optimization) to arrange a schedule that fairly, conveniently and optimally pairs interpreters with student-teacher conferences.

## Goals

* Collect and organize all interpreter availability and teacher meeting requests.

* When pairing interpreters with student-teacher conferences, the scheduling approach should be:

  * _Objective-driven_: A maximal number of student-teacher conferences include an interpreter.

  * _Constraint-driven_: Schedules are fair, convenient and practical for all interpreters and teachers.

* Create and distribute personalized schedules for both interpreters and teachers.

## Takeaways

* Google’s open source software suite [OR-Tools](https://developers.google.com/optimization) provides many useful models for constraint programming problems.

* The solution space of all combinations matching interpreters to student-teacher conferences is huge.

* As expected, the SAT solver does not scale efficiently and quickly grows unmanageable as input increases.

* While unable to scale efficiently, Google's CP-SAT Solver nonetheless provides an optimal schedule.

## Documents

* [Presentation](/assets/pdf/SAT_Presentation.pdf)
* [Report](/assets/pdf/SAT_Report.pdf)
* [Code](https://github.com/dweinflash/IHC-Scheduler_SAT-Solver)
