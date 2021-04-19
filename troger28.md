# Sprint 1
I was assigned [instance 611](https://github.com/catmasteryip/kivy_glucose) for Project 1 and [instance 1391](https://github.com/rognar/webkit-wince-5-6-7-2013-mobile-) for Project 2. In order to determine if these OSS projects are still active, I reviewed their commit and issue histories, the number of contributors, and any other activity that stood out.

### Instance 611: catmasteryip/kivy_glucose
The most recent activity I saw on this project is from July 2020, which includes commits that the project "can be run on android now." This leads me to believe that the primary task or purpose of the project was completed because there is a signifier of accomplishment and no activity since. Furthermore, there is only one contributor, and there are no issues or pull requests. These observations convince me that this project is no longer active.

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
The most recent activity on this project was in April 2020, which like with the previous instance, may imply that the project is no longer being worked on. Similarly, there are no pull requests, issues, or other evidence of current activity. There is only one contributor, and I believe that this project is also no longer active.

### Conclusions
The activity histories of each of these OSS projects imply that neither is currently active. The few commits and single contributor per project makes me think that they could be brief personal projects that were fairly smoothly completed (or poorly documented). Another explanation that comes to mind is that these projects were completed prior to their addition on GitHub, and the users uploaded them to GitHub later in order to document their work. Regardless of whether these things are right about the projects, I believe instances 611 and 1391 are no longer active.

# Sprint 2

### Instance 611: catmasteryip/kivy_glucose
Considering that this project only has one contributor and does not seem to be currently active, I believe it is not accepting contributions. Furthermore, there are no pull requests, issues, or a README file. 

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
Similarly, based on the fact that this project is no longer active and has a single contributor, I suspect it is not accepting contributions. The lack of pull requests and issues supports this.

# Sprint 3

Both projects I was assigned utilize libpng, a popular graphics library. It is subject to [CVE-2017-12652](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-12652). This vulnerability was addressed by [commit 347538efbdc21b8df684ebd92d37400b3ce85d55](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55).

### Instance 611: catmasteryip/kivy_glucosec
I believe the vulnerablility does not exist in this project. I determined this by comparing the pngpread.c and pngrutil.c files from the commit listed above with those in this specific project. The c files in this project do not contain the additions/modifications from the commit listed above, which was from August 3, 2017. However, the comments at the header of this project's pngpread.c include "Last changed in libpng 1.6.32 [August 24, 2017]," which shows this project contains a more updated and recent libpng. Thus, it is reasonable to conclude that the vulerability we were looking for is not in this project. There could be another vulnerability associated with the more recent libpng, but that is beyond the scope of this task.

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
After reviewing the pngpread.c and pngrutil.c files in this project, I have concluded the vulnerability may or may not exist. These files do not contain the additions/modifications that were included in the libpng commit which fixed the vulnerability. The header comments in this project's pngpread.c contain "Last changed in libpng 1.4.3 [June 26, 2010]," which hints that this project utilizes an older version of libpng. The structure of the relevant c files is very different from those in the commit that fixed the vulnerability. From this, it is hard to determine if the specific vulnerability of interest is present here. This project may contain other vullnerabilities, it may still contain the one we have reviewed, or it could be free from the vulnerability (perhaps the vulnerability was introduced in a later libpng version). 

# Sprint 4

### Instance 611: catmasteryip/kivy_glucosec
It looks as though the vulnerability we have reviewed in libpng is not present in this project. Therefore, a patch related to it is not needed. This does not mean that updates could not be made. For example, if the more recent version of libpng that this project uses contains another vulnerability, a patch for that could be beneficial.

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
Since the version of libpng in this project is significantly older and different than the one seen with this vulnerability, patching it is not realistic. First, we are not sure if the vulnerability existed in this past version. If the vulnerability is present, a justifiable solution would be to update the project to include the most recent libpng files. This would require extensive testing as simply modifying those files may not compile with the older code currently used. For this reason, producing a patch in this project is not realistic for this sprint task.

# Sprint 5

### Instance 611: catmasteryip/kivy_glucosec
This project's libpng is up to date, so no patch is necessary. Thus, I did not create a pull request on this project.

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
This project currently includes a much older version of libpng than the one corresponding to the vulnerability of interest. Instead of producing a patch that would likely cause more problems than it would fix, I created an [issue](https://github.com/rognar/webkit-wince-5-6-7-2013-mobile-/issues/1) suggesting that the libpng files are updated to reflect the most recent release.

# Sprint 6

### Instance 611: catmasteryip/kivy_glucosec
Not applicable, since no patch was necessary and I did not submit a pull request.

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
There is no response to the issue I created - there are neither comments/questions, nor have there been changes to the project. I will continue to check on this and provide an update if necessary.

