# Open Source Project Assignment

## Sprint 1
Please describe criteria you have used to determine if your OSS projects are still active. Please consider lecture or any other sources.

I have been assigned [instance 182](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html) and [instance 422](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html). Firstly, none of the links to instance 182 seem to be working, so I am unable to determine if this project is still active. So, I will instead consider [instance 183](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html). There is a single link associated with instance 183, and this project does seem to be inactive. There are two links associated with instance 422, and both of these forked projects also seem to be inactive. In order to determine this, I looked mainly at the commits, issues, pull requests, and number of contributors for each fork. For the commits, issues, and pull requests, I considered their frequency, their number, the interactions with them, and how recent they are.

### Instance 183
For the [link](https://github.com/FreeSouth/3ryparty) associated with instance 183, all six commits were made on May 23, 2020 by a single contributor. There do not exist any issues or pull requests. As such, it does not seem like this branch was very active when it was made, nor does it seem to have been active since then.

### Instance 422
For the [first fork](https://github.com/SeanRog/SER401-FALL-19-Project35), all commits were made between April 18 and April 27 in 2020, with multiple commits being made almost daily. There were five contributors at the time. There are neither open nor closed issues, although there were many pull requests made between October 2, 2019 and April 27, 2020. All of these have been closed now, however, so it looks like this fork is not active. There is nothing else that I can see from the page on Github that would lead me to believe that this fork is still active, especially since all work on the fork seems to have been made within a relatively short amount of time nearly a year ago.

For the [second fork](https://github.com/dsandy12/teammaker), we had all commits made within the same time period as the first fork from the same five contributors as the first fork. This fork also has no issues, open or closed, nor does it have any pull requests. As such, it seems to be fairly similar to the first fork, and it also seems to be inactive.

Both forks for instance 422 seem to have been fairly active roughly one year ago, but they do not seem to be so anymore.

## Sprint 2
Determine if the projects still accept contributions, note the criteria you have used.

In order to determine if the projects are still accepting contributions, I used similar criteria to what I looked for above. I also tried to look more at the contributors' interactions with commits, pull requests, and issues, in order to judge their openness to new contributions. As noted above, both of the projects seem like they have been inactive for nearly a year, so it is unlikely that they would accept a contribution if it were to be added now. Furthermore, while the projects were active, contributions were made by a small number of people, so it does not seem like they were very open to outside help. That is not to say that they would necessarily turn it away, but there does not seem to be a history of them accepting contributions from others. Most of the work was added through commits, rather than with pull requests, which further leads me to believe they were more of a select group working on a project for a short amount of time and would not accept a contribution now. The lack of issues, open or closed, tells a similar story.

## Sprint 3
Determine if the vulnerability still exists (the file in question has not been changed or, if changed, can it still be exploited). Please note the method you have used and the findings.

### Instance 183
This project is a branch from libpng, and the vulnerability that was originally in libpng seems to still exist in this project. Specifically, the section of code that was added to pngpread.c within libpng to fix the vulnerability does not seem to exist within this instance. In order to determine this, I compared the version of pngpread.c within the instance to the fixed version of pngpread.c within libpng. The other file that was changed for libpng, namely pngrutil.c, does not seem to exist within this instace, so that vulnerability might no longer be a problem.

### Instance 422
Similarly, the first project for instance 422 is also a branch of libpng, and the vulnerability that was originally in libpng seems to still exist in this project. This is due to the same reasons as the above.

## Sprint 4
Produce patches for both projects. Note any issues.

For both instances, I simply forked the project to my own account and added the vulnerability fix to pngpread.c. I did nothing to pngrutil.c, since this file does not exist in either instance. The commit containing the fix for instance 183 can be seen [here](https://github.com/SHANNON-HALL/3ryparty/commit/a9252e6139cc3e78d6522abf13dba77e7b829bf0), and the commit for instance 422 can be seen [here](https://github.com/SHANNON-HALL/SER401-FALL-19-Project35/commit/824810b4cc68e7dab162d7d2ca58e4956f8256cb). I do not expect any issues, since everything other than this missing section seems mostly the same.
