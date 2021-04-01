# Sprint 1
The two instances I am looking at are [instance 1182](https://github.com/glennrp/libpng) and [instance 15](https://github.com/qemu/qemu). The project for instance 
1182 is a graphics library written primarily in C. The project for instance 15 is a machine & userspace emulator and virtualizer primarily written in C. To 
determine if these two projects are active, I looked at the number of contributors, the recency of issues, the recency of pull requests, and the 
frequency of changes to the repository.

### github.com/glennrp/libpng (Instance 1182)
This project has 47 total contributors and several active contributors. There are several issues that have been open within the past month. 
Several pull requests have been resolved within the last 3 days. Changes to the repository have been made as recently as 5 days ago. These things lead me 
to believe that this project is active.

### github.com/qemu/qemu (Instance 15)
This project has more than 1000 total contributors and several active contributors. Although there are no open pull requests, there are several closed pull 
requests from the last month. There are several recent changes that have been made to the repository. One change having been made a day ago (03/17/2021). Other
changes have been made within the last few days. These things lead me to believe that this project is active.

# Sprint 2
The two instances I am looking at are [instance 1182](https://github.com/glennrp/libpng) and [instance 15](https://github.com/qemu/qemu). To 
determine if these two projects are still accepting contributors, I looked at the number of contributors, the recent commit activity, the recent pull requests, and the frequency with which issues are closed.

### github.com/glennrp/libpng (Instance 1182)
This project has 47 total contributors. The latest commits was made on 03/13/2021, but all except for one were made by the same person. There are several issues that have been open within the past month. The latest closed issue was from 19 days ago, but the second most recent issue was closed several months ago (12/11/2020). 
Several pull requests have been resolved within the last 8 days, although, most of them were rejected. Although there are very few accepted contributions, there are signs of fairly recent interactions between contributors and maintainers of the project. This leads me to believe that this project is still accepting contributors.

### github.com/qemu/qemu (Instance 15)
This project has 1113 total contributors. Although there are no open pull requests, there are several closed pull 
requests resolved within the last month. There are many recent commits that have been made to the repository. Several commits having been made today (03/22/2021). The recent commits have been authored by several different contributors.
The recency of commits in the repository, the variety of active contributors, and the total number of contributors lead me to believe that this project is still accepting contributors.

# Sprint 3
### (Instance 1182)
This repository's pngpread.c file is missing which has the vulnerability. The repository's other vulnerable file, pngrutil.c, is also missing.
Because the repository does not seem to include the files specified in the vulnerability, I believe the vulnerability does not exist in the repository.

### (Instance 15)
This repository's pcnet.c file is missing the changes that were specified in the commit. With this being the case, it is clear that the repository still
contains the vulnerability from the referenced commit for github.com/qemu/qemu. 
