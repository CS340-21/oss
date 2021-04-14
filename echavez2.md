**Sprint 1**

- Instance 559

    this project is no longer active as it only has 1 contributor and the last commit was 8 months ago. 
    The only commit was the initial commit and there are no issues or milestones

- Instance 250
    
    This project is also inactive as there has been no commits in 2 years.
    There was only an initial commit and 1 commit following that. 
    There is only 1 contributor and no issues or milestones.
    
**Sprint 2**
    
- Instance 559
    
    since this project is not active, it does not seem to be accepting contributions. There is only 1 contributor implying it never accepted contributions
    
- Instance 250

    Since this project is not active, it is not accepting contributions. There is also 1 pull request from 2020 that was never accepted.

**Sprint 3**
    
- Instance 559
    
    This project seems to have a version of pngrutil.c that has been updated to fix the vulnerablility. On line 185 there is a funcion call (defined in line 3143) that fixes the issue. The pngpread.c file is not fixed because it is missing any function or code at the location where the fix would have been.
    
- Instance 250

    The version of libpng used in this project is from 2012 so both pngpread.c and pngrutil.c still have the vulnerability.
    
**Sprint 4**
    
- Instance 559
    
    Since the version of libpng is so close to the release of this fix, there are likely no other vulnerabilities that have been discovered. https://github.com/beanh0le/python/commit/38a5f1f0a3cdd3b9faa5debec8bcdf439212a0cf
    
- Instance 250

    since the version of libpng is so old compared to the single piece of code added, there may be many other vulnerabilities that were fixed before this that are still in place. Since there will likely be other problems, it is probably better to update to a newer version of libpng
