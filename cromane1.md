Sprint 1:
For the first project, I was assigned to look at codeblocks (instance 813), which is an IDE. For the second, I was assigned hw55 (instance 2), which seems to be a python program that finds "easter eggs".

Instance 813:
Based on the history of commits to the main branch of this repo, I can tell that this project was quite active during early 2020. This is because there were many commits with consistent frequency from January through March. After that, the amount of commits greatly decreased and the most recent one was made 6 months ago. Currently, there are no active issues and no pending pull requests which leads me to believe that this project is no longer active.

Instance 2:
Just looking at the main branch of this repo, there are only two folders, both of which were posted 11 months ago. There are also no active issues or pending pull requests. I believe it is safe to assume that his project is no longer active.

Sprint 2:
For instance 2, I would say it is very safe to say that this project would no longer accept contibutions. This is not only because it has been inactive for so long, but it also appears that this project was a homework assignment for a software engineering student, and hopefully this student has submitted his assignment by now. For instance 813, I would say there is a small possibility that this project still accepts contributions, and this is only because the project has had updates for bug fixes before, so it is possible more bugs could be found. However, it has been inactive for months and there are no current issues so I doubt it still accepts contributions.

Sprint 3:

Instance 813:
It would seem that the vulnerability for this project is that an attacker is able to execute arbitrary code via a crafted project file. If found this vulnerability by searching the project through: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-10814  With this, it would appear that this vulnerablity still exists because there do not seem to be any patches that reference this issue.

Instance 2:
Since instance 2 does not seem to be an open source project (it looks like it is meant to be meant for a homework assignment), I think it is safe to say that there are no viable vulnerabilities that could be patched.

Sprint 4:

Instance 813:
The patch for CodeBlocks can be found [here](https://github.com/cromane1/codeblocks). To do this, I simply forked the library and updated the pngpread.c and pngrutil.c files.

Instance 2:
Again, no patch would be necessary for this instance because it was a homework assignment and no vulnerabilites could be found for this project.


Sprint 5:
PR for instance 813 can be found here: https://github.com/dreamsdk/codeblocks/pull/1
