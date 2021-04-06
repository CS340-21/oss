# Sprint 1
I am looking at [instance 1105](https://bitbucket.org/hhrhhr/factorio-tools-lua/src/master/) for "Project 1" and [instance 3](https://bitbucket.org/andreyu/simple-viewer-gl/src/master/) for "Project 2." These projects use the libraries libpng and LZ4 respectively. For each project I used the following critera to determine if it is still active: number of participants, frequency of commits and issues, and enthusiams of discussion in the community.

### Factorio tools (Lua) (Instance 1105)
This project is a fork of [this repo](https://github.com/KirkMcDonald/factorio-tools) rewritten in Lua. It uses the [libpng](https://github.com/glennrp/libpng) graphics library. The only participant is Dmitry Zaitsev, who was maintaining this repo from 4/13/2020 until 6/13/2020 (the dates of his initial and final commits). As stated by the last commit, this project have been moved to a new repo leaving the old one "frozen." There are currently no open pull requests or community discussion. Since there has been no progress since June of 2020 and activity has halted on the "new" repo (last commit 7/27/20), I deem this project inactive.

### Simple Viewer GL (Instance 3)
This project is a "tiny image viewer" for Unix based on OpenGL. It utilizes the [LZ4](https://github.com/lz4/lz4) library for lossless compression. The only participant is Andrey Ugolnik, who has been mainting this project from 4/4/10 until 2/26/21. Commits usually occur several times a month with seemingly meaningful development updates. There are currently no open pull requests or community activity. There are numerous open issues (all assigned to Andrey, of course) and two main branches (main and development). Using the critera stated initially, I determine that this project is active.

# Sprint 2
Projects consist of the same instances in Sprint 1. I used the following criteria to determine if the project actively acceps contributions: latest commit, number of contributors, frequency of commits, and if the project is welcoming to new contributors.

### Factorio tools (Lua) (Instance 1105)
As I determined this project is inactive last week, I can say without a doubt that the project does not accept new contributions. There also wouldn't be a reason for inherting this project, since the author has moved development to a new repo entirely (i.e. contribute to that one). If development had not been moved and this repo was still used, it is likely that it still would not accept contributions for the following reasons: 1. there is only one author with no signs of external issues or pull requests and 2. the commits seemed to come in rapid bursts every 2 or so months so you would have to catch the author in their cycle of development.

### Simple Viewer GL (Instance 3)
Since this project is active, it is likely that the author is accepting of contributions. Although there have not been any outside issues or pull requests on the repo to date, it is possible that Andrey would merge meaningful changes/additions. I determine this by examing the frequency of commits in the past and the dwindling development in the present. Although this is a long term project maintained by a single developer, it is possible his progress is slowing because of interest or lack of ideas for further improvements. Using this logic and since this repo has commits in the last month or so, I would say the chances of getting a legitimate pull request merged is high.

# Sprint 3
Still looking at same two projects. I used the information provided for [instance 1105](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html) and [instance 3](https://davidalanreid.github.io/output/d7cad81093cd805110291f84d64d385557d0ffba/vulnerable.hack.html) to determine if the fix has been implemented in the projects or not. This was done by looking at the project files and comparing the fixed ones.

### Factorio tools (Lua) (Instance 1105)
The [vulnerability](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-12652) for this project stemmed from the libpng library not properly checking the length of chunks against the users limit. The vulnerability is fixed by modifying two files: pngpread.c and pngrutil.c (found [here](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55). The first vulnerable file in the project, pngpread, does not contain the proper fix. The second file, pngrutil, also does not contain the proper fix. Therefore, I conclude this project still contains the libpng vulnerability mentioned previously.

### Simple Viewer GL (Instance 3)
The [vulnerability](https://cve.mitre.org/cgi-bin/cvename.cgi?name=2019-17543) for this project stems from the lz4 compression library containing a heap-based buffer overflow which affect certain applications. Thankfully, only a few uncommon usages are at risk, but it's a problem to be addressed (and has!). The fix is in file lz4.c and simply changes a '<' to a '<='. After checking this file in the project source, I have determined that it does not implement the fix and thus currently contains the overvlow mentioned before.

# Sprint 4
Now I will produce patches for both of the projects and note any issues. These fixes can be found in the previous sprint.

### Factorio tools (Lua) (Instance 1105)
Since the original repo is completely obsolete, I decidede to take a look at the current one I noted in earlier sprints. (Un)Luckily, this repo contains the same vulnerabilities as the old one. I began by forking the [new repo](https://bitbucket.org/hhrhhr/factorio-lab-tools/src/master/) and making the changes noted in Sprint 3. Sadly, it would seem I am unable to freely create pull requests for this project due to permissions. Furthermore, I do not see how to contact the rpo owner and request him to pull these changes. Anyhow, here is my forked [repo](https://bitbucket.org/ObsidianSkin/factorio-lab-tools/src/master/) with the [fix](https://bitbucket.org/ObsidianSkin/factorio-lab-tools/commits/da943561fec1fb221af2e3ba7ae89f2257d26d43). 

### Simple Viewer GL (Instance 3)
Again, I noticed the ability to create pull requests was disabled. However, this time I was at least able to make an issue. First, I forked and cloned the [repo](https://bitbucket.org/ObsidianSkin/simple-viewer-gl/src/master/) and [fixed](https://bitbucket.org/ObsidianSkin/simple-viewer-gl/commits/da7a346edf4ae166eeb77eb2f164e50f3884f7a9) the vulnerability (one symbol :D). Then, I proceeded to make the [issue](https://bitbucket.org/andreyu/simple-viewer-gl/issues/25/fixing-off-by-one-error-in-lz4c) and wait patiently.
