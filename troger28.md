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
I believe the vulnerablility still exists in this project. I determined this by comparing the pngpread.c and pngrutil.c files from the commit listed above with those in this specific project. The c files in this project were not updated with the corrections, which hints that this project is still vulnerable. 

### Instance 1391: rognar/webkit-wince-5-6-7-2013-mobile-
After reviewing the pngpread.c and pngrutil.c files in this project, I conclude the vulnerability still exists. These files do not contain the additions/modifications that were included in the libpng commit which fixed the vulnerability. The lack of properly addressing the issues leads me to believe this project remains vulnerable. 
