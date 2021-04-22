# Sprint 1
I was assigned [QK-Lite/wePRO](https://github.com/QK-Lite/wePRO) (Instance 418) and [water111/jak-disassembler](https://github.com/water111/jak-disassembler) (Instance 1189),
and I reviewed the repository, the issue history, and the pull request history of each to determine whether these OSS projects are still active.

**wePRO**  
This project has not been active since May 19, 2020, when the last commit (of 4 in total) was made. The initial commit was made on May 16, 2020, so this project
was really only active for a few days, and all changes were committed by the repository owner, who is still active on GitHub, so this project likely will not be returned to.
There are no issues, pull requests, milestones, other watchers, stars, or forks on this project, so there is no evidence of any additional activity from other users.

**jak-disassembler**  
There are two contributors to this project, water111 and xTVaser.
The most recent commit was to the other branch, cfg-dev, on August 22, 2020. It had 5 commits throughout August, but it seems these changes have not been merged with master.
The last activity on the master branch was on August 1, 2020, and there have been 20 commits spread across 3 different days starting on July 26, 2020 (short, dense periods of activity
from the two contributors).
There are no issues or milestones, but there is a work-in-progress pull request left open from July 26 and a closed merged pull request from July 31--both from xTVaser.
There are two watchers who seem to be "lurking," 5 stars from a few other lukers, and two forks--one from one of the lurkers and the other from xTVaser--but they are both inactive.
This lack of recent activity from all who have left a trace on this repository leads me to believe that it is inactive.
However, a quick look at water111's GitHub profile reveals that this jak-disassembler was likely used in a newer, very active project [here](https://github.com/water111/jak-project).

# Sprint 2
Both projects seem to have been abandoned, and there never was any GitHub collaboration on wePRO, so it likely they are both not accepting contributions. In addition, contributing to this instance of the jak-disassembler would be a waste of time, as it seems to have been advanced by a lot in its new repository "jak-project" (linked above), where contributions are likely welcome given that there have been 9 contributors in total, but only 3 of them (the project leads, it seems) have made commits in the last month. On this project, the README contains detailed information about the project, its goals, etc., so someone who was interested may be able to contribute.

# Sprint 3
Both projects' vulnerabilities were in files pngpread.c and pngrutil.c from libpng, a popular reference library for handling PNGs. jak-disassembler seems to have removed these files as I cannot find them in the path specified by the vulnerability page, so the vulnerability is also gone. However, wePRO's libpng files are still there and the file headers claim that this is a version from 2014, and the vulnerability was patched in 2017, so it has not yet been fixed here. I checked the files to confirm that the code segment from the libpng commit was missing.

# Sprint 4
I produced a patch for the project that still contained the vulnerability, wePRO, by forking the project and simply making the changes that the specific commit made rather than updating the whole version of libpng, which could create other incompatibility issues with the project. See https://github.com/s4mpl/wePRO/commit/13d4e26365bb64776b73882c933c2b9ff2331ff5 and https://github.com/s4mpl/wePRO/commit/b8db29a9ea49fdca4f30e2e72d9e4d624c9dafd8

# Sprint 5
I submitted a pull request to QK-Lite/wePRO, as seen [here](https://github.com/QK-Lite/wePRO/pull/1).

# Sprint 6
I got no activity regarding my pull request, so I did not need to make any additional responses.
