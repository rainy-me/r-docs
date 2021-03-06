# 1 Introduction

---

R is a system for statistical computation and graphics. It provides,
among other things, a programming language, high level graphics,
interfaces to other languages and debugging facilities. This manual
details and defines the R language.

The R language is a dialect of S which was designed in the 1980s and has
been in widespread use in the statistical community since. Its principal
designer, John M. Chambers, was awarded the 1998 ACM Software Systems
Award for S.

The language syntax has a superficial similarity with C, but the
semantics are of the FPL (functional programming language) variety with
stronger affinities with Lisp and APL. In particular, it allows
"computing on the language", which in turn makes it possible to write
functions that take expressions as input, something that is often useful
for statistical modeling and graphics.

It is possible to get quite far using R interactively, executing
simple expressions from the command line. Some
users may never need to go beyond that level, others will want to write
their own functions either in an ad hoc fashion to systematize
repetitive work or with the perspective of writing add-on packages for
new functionality.

The purpose of this manual is to document the language _per se_. That
is, the objects that it works on, and the details of the expression
evaluation process, which are useful to know when programming R
functions. Major subsystems for specific tasks, such as graphics, are
only briefly described in this manual and will be documented separately.

Although much of the text will equally apply to S, there are also some
substantial differences, and in order not to confuse the issue we shall
concentrate on describing R.

The design of the language contains a number of fine points and common
pitfalls which may surprise the user. Most of these are due to
consistency considerations at a deeper level, as we shall explain. There
are also a number of useful shortcuts and idioms, which allow the user
to express quite complicated operations succinctly. Many of these become
natural once one is familiar with the underlying concepts. In some
cases, there are multiple ways of performing a task, but some of the
techniques will rely on the language implementation, and others work at
a higher level of abstraction. In such cases we shall indicate the
preferred usage.

Some familiarity with R is assumed. This is not an introduction to R but
rather a programmers' reference manual. Other manuals provide
complementary information: in particular
[Preface](./R-intro.html#Preface) in An Introduction to R provides an
introduction to R and [System and foreign language interfaces](./R-exts.html#System-and-foreign-language-interfaces) in
Writing R Extensions details how to extend R using compiled code.

---
