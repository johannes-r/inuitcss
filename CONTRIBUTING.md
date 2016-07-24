# Contributing

Whilst inuitcss gratefully welcomes contributions from the open-source
community, there are a number of requirements and principles that need adhering
to before code is eligible for inclusion in the project.

- - -

0. [Philosophy](#philosophy): What do we want to achieve with inuitcss?
0. [Coding Style](#coding-style): What should your code look like?
  0. [Template](#template)
0. [Git(Hub) Workflow](#github-workflow): How should you go about contributing?

- - -

## Philosophy

inuitcss’ scope, goals, and philosophy are quite strict and opinionated. In
brief:

* **No design:** inuitcss should provide zero cosmetic styling—it is a framework
  in its truest sense. Pull requests that introduce cosmetic styling will not be
  accepted.
* **Simplicity:** Readability, clarity, and simplicity are very important
  features of inuitcss—please ensure that code you are adding does not obscure
  or overcomplicate any parts of the project.
* **Performance:** inuitcss aims to be a lightweight framework that helps both
  developers and their sites run faster—please ensure that performance is at the
  forefront of your mind as you add new features.

## Coding Style

* 2 space indents
* 80 character wide files
* Liberal use of whitespace

### Template

Please use the inuitcss template](https://github.com/inuitcss/template) as a
starting point for additional files. It has the required comment and spacing
formats.

## Git(Hub) Workflow

If you would like to submit a pull request, please follow the below Git
process/workflow. It helps to give us a better paper-trail, and allows us to
follow work through the issue/pull request process.

1. **Create a new issue for the proposed addition/change/fix.** This allows us
   to discuss the suitability of the proposal before you begin work.
2. **Create a new branch entitled `tkt-<issue-number>`.** Look at the URL of
   your new issue; take its number (e.g. 99) and create a branch called
  `tkt-0099` (with leading zeroes). Do all of your work in this branch.
3. **Start all commit messages with `[refs #<issue-number>]`.** If you’re
   working on issue 99, all of your commits should begin with `[refs #0099]`.
   This allows us to link every commit back to both an issue and a branch.
4. **Open a pull request into `develop`.** Our main branch is `develop`, and
   this is where we want new work to be merged into. `master` is a release
   branch only.

Example:
[`f000350`](https://github.com/inuitcss/inuitcss/commit/f000350dd23b92cb403142f4a8af84d92d300cf7).
Here I can see that the ‘Implement proposed flag object fix’ commit happened
against [issue 76](https://github.com/inuitcss/inuitcss/issues/76), and took
place in a branch named `tkt-0076`. This means that I can find any discussions
around this piece of work, and I know in which branch I should commit and
further, related work.

The one downside to this workflow is that branches no longer have descriptive
names, so running `$ git branch` might leave you looking at something like this:

```
develop
master
tkt-0014
tkt-0021
tkt-0058
tkt-0080
tkt-0083
tkt-0089
```

Use [ghi](https://github.com/stephencelis/ghi) to get detailed information about
a particular branch and its related issue, e.g.:

```
$ ghi 14
```
