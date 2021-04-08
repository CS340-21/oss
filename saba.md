## Sprint 1
I was assigned [Orange](https://github.com/mis9ter/orange) (Instance 1016) and [cengizkandemir](https://github.com/cengizkandemir/uwmf) (Instance 1257).
By looking at their commit history, pull requests, open issues, and the number of recent contributors, I determined whether the projects were still active.

### Orange (Instance 1016)
*Inactive Project
There are 36 total commits and the most recent one was last month.
All commits are made by a single user, so they are probably not accepting
outside contributions.
There are no open issues and no pull resquests. 
Because of this I determined the project to be inactive.

### Unbiased Weighted Mean Filter (Instance 1257)
*Inactive Project
This project has 96 total commits, and the most recent commit was only a few days ago.
However, before this month, there had been no activity on the project in over a year.
Again there are no pull requests or open issues, and there is only a single contributor.
Because of all of this, even though there was a very recent string of commits, I would still consider this project inactive. 


## Sprint 2

### Orange (Instance 1016)
I have determined determined that this project is not accepting contributions.
There is a single forked repo, but there are no open issues or pull requests.
There has not been any activity in over 1.5 months, and there is only one contributor listed in the commit history.

### Unbiased Weighted Mean Filter (Instance 1257)
This project is most likely not accepting new contributions. 
Again there are no active issues or pull requests and only a single contributor in the commit hisotry.
While there were some recently made commits, the project was left untouched for over a year before this so I cannot say
with certainty whether a contribution would be accepted, but I am inclined to say "no" for the other reasons.

## Sprint 3
To find out whether the projects had the vulnerability, I searched their files for pngpread.c and pngrutil.c and 
compared these to the commit found [here](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55?branch=347538efbdc21b8df684ebd92d37400b3ce85d55&diff=split).
### Orange (Instance 1016)
This is a little wierd, but it seems this project has removed libpng from the repository. The filepath
that was listed [here](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html) no longer exists, and I could not find either of the edited files by searching. I went through the commit history and [found the most recent version that still contained the libpng](https://github.com/mis9ter/orange/tree/29e089d52caf418312316c58d0b9e5218e2b2903/agent/reference/reactos-master/reactos-master/dll/3rdparty/libpng). Unfortunately,
this file had the vulnerability.

### Unbiased Weighted Mean Filter (Instance 1257)
This project still has the vulnerability. I simply went to the lines in pngpread.c and pngrutil.c that had changes marked
and compared them. 

## Sprint 4

### Orange (Instance 1016)
My forked repository can be found [here](https://github.com/samababa/orange). My latest commit adds the libpng library, while fixing the vulnerability. There shouldn't be any problems; however, a pull request may not be accepted since libpng was recently removed the original repository.

### Unbiased Weighted Mean Filter (Instance 1257)
My forked repository can be found [here](https://github.com/samababa/uwmf). My two latest commits should fix
the vulnerability with no errors. 

## Sprint 5

### Orange (Instance 1016)
Create a pull request [here](https://github.com/mis9ter/orange/pull/1).
### Unbiased Weight Mean Filter (Instance 1257)
Created a pull request [here](https://github.com/cengizkandemir/uwmf/pull/1).
