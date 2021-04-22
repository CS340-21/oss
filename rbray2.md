# Sprint 1
For Sprint 1, I was assigned instances 1101 and 869.  

## Instance 1101:   Ultraschall/ultraschall-soundboard    
My first vulnerability is for a project called Ultraschall-Soundboard (Ultrasonic in English), which is a soundboard   
that can be used by podcasters, according to the README. It seems fairly active, since the last commit was eight days   
ago, and there seems to be a few commits every month. It also has eleven open issues right now, one of them to make   
the README more descriptive, and it has nine closed issues. I think this project is fairly active by these criteria.
  
## Instance 869:   slowrunner/Carl   
The second vulnerability is for a project called Carl, which is a the code for running a robot named Carl, who has a   
minion on top of him. This project seems very active, since there were thirteen commits in the last month, and this project   
has existed since 2018. There are no open issues, but that seems to be more because there is only one contributor than a   
sign of inactivity, since there are so many comits.
   
# Sprint 2   

## Instance 1101:   Ultraschall/ultraschall-soundboard   
It seems like this project is still accepting pull requests, since the last one was merged on February 16. It seems   
feasible that they would still accept contributions from a new person.

## Instance 869:   slowrunner/Carl   
It does not look like this project is accepting pull requests, since the only contributions have been made by one person,   
and there are currently none open. This person may be open to having contributions, since they are so active, but it is likely   
that they just want to work on their robot alone. 

# Sprint 3

## Instance 1101:   Ultraschall/ultraschall-soundboard 
Since the vulnerability was in pngread.c and pngrutil.c, I checked to see the last time that these were committed in the project. Since the vulnerability was fixed in 2017, this patch would need to have been after. The last commit to both pngread.c and pngrutil.c was on January 6, 2021, so it is reasonable to conclude that the vulnerability no longer exists in this project. Even though the exact change cannot be found in the code, it has been many years since this vulnerability has been resolved, and libpng is a very active project, so it seems reasonable that the code would have changed since then.

## Instance 869:   slowrunner/Carl  
In this project, I was going to use the same method for checking if the vulnerability still exists. When I searched for the path to these files, though, it appeared that the path no longer exists. It seems like this program is no longer using libpng, so it is safe to conclude that the vulnerability no longer exists in this project, either.

# Sprint 4

## Instance 1101:   Ultraschall/ultraschall-soundboard
Since it seems like the vulnerability does not exist any longer using the above criteria, it is not reasonable to commit a patch for this project, especially since the commit that they made was this year on January 6, 2021.

## Instance 869:   slowrunner/Carl 
As stated in the previous sprint, this project does not use libpng any longer. Therefore, it is also not reasonable to commit a patch to this project, either.

# Sprint 5

## Instance 1101:   Ultraschall/ultraschall-soundboard
Because the vulnerability does not exist any longer, no patch was applied, so there is no pull request for this project.

## Instance 869:   slowrunner/Carl 
As stated above, this project no longer even has libpng in its directories, so there was no pull request for this project, because no patch was needed


## Instance 869:   slowrunner/Carl 
As stated in the previous sprint, this project does not use libpng any longer. Therefore, it is also not reasonable to commit a patch to this project, either.

# Sprint 6

## Instance 1101:   Ultraschall/ultraschall-soundboard
As stated in the last sprint, there was no need for a pull request, since this project already had the most up-to-date libpng files, so there were no responses to any pull requests, or notes to give. 

## Instance 869:   slowrunner/Carl 
As state in the last sprint, there was no need for a pull request, since the project no longer uses libpng at all, so there are no questions or notes to show.
