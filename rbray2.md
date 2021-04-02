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
Since the vulnerability was in pngread.c and pngrutil.c, I checked to see the last time that these were committed in the project. Since the vulnerability was fixed in 2017, this patch would need to have been after. The last commit to both pngread.c and pngrutil.c was on January 6, 2021. Upon further digging, it seems like the changes from the fixed commit to libpng  so it is reasonable to conclude that the vulnerability no longer exists in this project. 

## Instance 869:   slowrunner/Carl  
In this project, I was going to use the same method for checking if the vulnerability still exists. When I searched for the path to these files, though, it appeared that the path no longer exists. It seems like this program is no longer using libpng, so it is safe to conclude that the vulnerability no longer exists in this project, either.
