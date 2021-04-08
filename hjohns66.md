# Sprint 1

For my projects, I was assigned [instance 558](https://github.com/SuperEver/snb-vision) and [instance 476](https://github.com/antoine2000/TDL). I checked 
the number of participants and the frequency of commits and issues to determine if these two projects were still active.

### Instance 558: SuperEver/snb-vision

I could not not find a number of participants, and unfortunately this project has no README. Because there have not been any new commits or changes to this
project in thirteen months, I think that it was either finished over a year ago or has been abandoned. It is probably no longer active.

### Instance 476: antoine2000/TDL

Interestly, this entire project is in French I think. I have no idea what they were trying to do, but I'm pretty sure they finished because the last commit
to be added was called "final commit!" which seems pretty final. There have also been no more commits for a year. I therefore think that this project is
no longer active. 

### Conclusion

Neither of my projects seem to be active any longer, and I have no idea what one them was meant to do at all because it was in a different language.

-------------

# Sprint 2

For this sprint, I determined if these projects are still accepting contributions. 

### Instance 558: SuperEver/snb-vision

Since this project has no issues, milestones, or commits that I could find, I believe that this project is no longer accepting contributions. I also 
could not find any list of contributors or participants. 

### Instance 476: antoine2000/TDL

Since this project is entirely in a different language, possibly French, I'm not sure how to get in contact with the contributors because of the 
language barrier. I also believe that this project was completed because the last commit is from a year ago and is titled "final commit!"

### Conclusion

I believe that neither of my projects are accepting contributions any longer. 

-------------------

# Sprint 3

For this sprint, I tried to determine if the vulnerabilities still exist in these projects.

### Instance 558: SuperEver/snb-vision

In order to determine if the vulnerability still exists in this project, I followed the link that took me to the commit that is supposed to fix the
particular vulnerability that this project has. There was one change each done to pngread.c and pngrutil.c. This project's pngread.c was very different
from the fixed commit's version of pngread.c; therefore, I'm not sure if the patch would help or not. On the other hand, this project's pngrutil.c was
missing the patch which were if, ifdef, elif, and endif statements. I think that this patch could potentially help fix this particular vulnerability. 

### Instance 476: antoine2000/TDL

In order to determine if the vulnerability still exists in this project, I followed the link that took me to the commit that is supposed to fix the
particular vulnerability or vulnerabilities this program has. There was again one change each to pngread.c and pngrutil.c. Both this project's pngread.c
and pngrutil.c were different from the patches' versions. The projects' versions were also from 2014 while the patches' were from 2017. They both seem to 
be missing if, indelf, elif, and endif statements. I'm not sure if adding these patches would help, but I'll see if I can replace the older versions with
the more updated ones from 2017 to see if that fixes the vulnerability. 

### Conclusion

I'm reasonably confident that adding the additional statements to the first project could fix the vulnerability, but I'm not sure if completely replacing
or adding the more recent pngread.c and pngrutil.c will fix the vulnerability in the second project.

-----------------

# Sprint 4

I was mistaken in Sprint 3. Upon closer inspection, both the pngread.c and the pngrutil.c for the first project are more updated versions than the 
patches for them. The pngrutil.c doesn't have the if, ifdef, elif, and endif statements from the patch, but it does have a single line of code meant 
to "Check for too large chunk length" like the patch does. I'm no longer certain that a patch would fix this vulnerability. For the second project, 
much older versions of the pngread.c and pngrutil.c were used and any patches would probably cause more harm than good. 
