### Sprint 1:
I was assigned OOP_indie_studip and ebf_stm32f407_batianhu_emwin_demo. The most recent activity for OOP_indie_studip was 9 months ago. Though the most recent activity isn't too long ago, looking at the activity and commits it seems the project was already written and uploaded all at once. This seems to indicate the project is inactive and brings concern issues may not be accepted.
ebf_stm32f407_batianhu_emwin_demo, on the other hand, has commits ranging from 3 years ago to 7 months ago. Considering the range in timing of activity on the repository, it is plausible the project is still active. However, much of the repository is in Chinese, which could pose a great issue in understanding.
Neither of the projects had issues or pull requests indicating project activity.

### Sprint 2:
To find out if the assigned projects are still accepting contributions the times of contibution, the amount of contribution, and number of contrigutors were observed. For OOP_indie_studip, the most recent contributions were made 9 months ago. The contributions were made by a single contributor during a single week. It also appears by the amount of lines that were contributed that the code may have been mostly pre-written, then uploaded to github. This inicates that the project will most likely not accept additional contributions. As for ebf_stm32f407_batianhu_emwin_demo, three different people have made contributions to the project. There seems to have been one initial commit where all the code was written or uploaded several years ago, and several smaller changes and uploads every so often since. Since small changes have been made over time, it is plausible that contributions may be accepted. As an additional note, pull requests and submitted issues would have been taken into account as part of determining the activity of the project, however, there was no information of this type for either project.

### Sprint 3:
When looking at the OOP_indie_studip repository, it can be seen that the vulnerability has not been fixed. This can be seen by comparing
libpng with the corrected vulnerability to libpng of OOP_indie_studip.

When looking at ebf_stm32f407_batianhu_emwin_demo, there are many paths that are listed for libpng. Looking through the different paths and comparing pngpread.c and pngrutil.c to the corrected libpng files, it became clear that the files used in the github repository aren't even the same files. There is overlap with some of the function and variable names; however, the majority of the files are completely different.

### Sprint 4:
The OOP_indie_stupid repository was forked. The proper changes were made to pngpread.c and pngrutil.c to correct the vulnerability. A pull request has been made for the files. The commits for these files can be found in the links below.
pngpread.c: https://github.com/GaryAF/OOP_indie_studip/pull/1/commits/257194536ebbb06a59bc38f32d952105fa932ec3
pngrutil.c: https://github.com/GaryAF/OOP_indie_studip/pull/1/commits/b0e1a02201ba48420b897483800e1fff0612b3b2

When looking at ebf_stm32f407_batianhu_emwin_demo and considering comments mentioned in class, the circumstances surrounding the pngpread.c and pngrutil.c files looking completely different than expected were rexamined. Upon further observation, it can be discoved that the version of libpng that is used in this repository is from 2006. Since the changes in the library would be significant and would cause issues of dependancy, it is not reasonable to suggest changes for this repository.
