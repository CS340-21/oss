## Sprint 1 - Determine if projects are active

The projects I have been assigned are [Qt5-Genode](https://github.com/cproc/qt5#readme) and [Universal-Tools](https://github.com/utechnique/universal_tools).
For each project, I reviewed the repository, commit history, issues (open and closed), pull requests (open and closed), milestones (if any), 
and contributors. Through looking at these factors, I determined whether each project was still in active development. 

#### _Qt5 Project (Instance 1231)_
This project is a port to allow [Qt5](https://www.qt.io/) to be used with [Genode](https://genode.org/) based operating systems. 
There are 15 total commits for the project from two contributors with the most recent being from Sep. 17, 2020. 
There are three open pull requests, but all are from bots to update dependencies. This project does not appear
to be in active development.

#### _Universal Tools (Instance 457)_
This project is a light-weight cross-platform framework for c++ development. It does not use the STL or Boost 
libraries, though it provides much of the same functionality without any external dependencies. There are 115
total commits to the project, with the most recent being from March 10, 2021. There is only one contributor to
the project, and there is currently one active branch that is ahead of the master branch. This project appears 
to still be in active development.

## Sprint 2 - Determine if projects are accepting contributions

#### _Qt5 Project (Instance 1231)_
Based on the information gathered in Sprint 1, I do not believe that the Qt5 Project is accepting new contributions. There have been no commits 
since Sep. 2020, and no pull requests have been submitted other than depencency updates by bots. 

#### _Universal Tools Project (Instance 457)_
The Universal Tools project has recent commits and is in active development. Because of this, I believe that Universal Tools is currently
accepting new contributions. However, since there is only one contributor to this project, it is unclear if they will accept contributions
made by others.

## Sprint 3 - Determine if vulnerability still exists

#### _Qt5 Project (Instance 1231)_
By comparing the changes made in the [referenced commit](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55) with the contents of the `qtbase/src/3rdparty/libpng/pngpread.c` and `qtbase/src/3rdparty/libpng/pngrutil.c` files in this project, I determined that the files have not been updated with the necessary modifications, and the vulnerability still exists. Each file should be modified to reflect the changes made in the referenced commit.

#### _Universal Tools Project (Instance 457)_
By comparing the changes made in the [referenced commit](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55) with the contents of the `/contrib/fltk/png/pngpread.c` and `/contrib/fltk/png/pngrutil.c` files in this project, I determined that the files have not been updated with the necessary modifications, and the vulnerability still exists. Each file should be modified to reflect the changes made in the referenced commit.

## Sprint 4 - Produce a patch for the vulnerability

To produce a patch for each vulnerability, I forked each project and edited the files referenced in Sprint 3 above. I encountered no issues in doing this, 
and I will be submitting a PR for each. My forks containing the patches for the vulnerabilities of each project are linked below.
* [Qt5 - patched](https://github.com/rossketron/qt5)
* [Universal Tools - patched](https://github.com/rossketron/universal_tools)

## Sprint 5 - Create pull requests for the vulnerabilty patches made in sprint 4

I made a pull request to merge my fork of each project (containing the vulnerabilty patch) with the master/main branch of the project's repository.
The pull requests are linked below.
* [Qt5 - pull request](https://github.com/cproc/qt5/pull/9)
* [Universal Tools - pull request](https://github.com/utechnique/universal_tools/pull/1)
