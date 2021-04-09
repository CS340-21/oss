# Sprint 1

Criteria used was the commit history, number of open/closed issues, number of pull requests, and milestones/releases if any.

### libgender age model project (instance 921)
This project is a linux dynamic library for the insightface gender/age model. 
I determined that this project is not active. Every commit in the project's history was on the same day in Aug, 2020, and most of these commits
past the initial commit were small changes such as typos. There is only one open issue from Nov, 2020 and there have been no releases for this project.

### lighttpd project (instance 4)
This project is a fast and flexible webserver softwware.
I determined that this project is not active. The only commit to the project is the initial commit from April, 2020. There are no open issues, pull
requests, or releases.

# Sprint 2

Criteria used was the same as Sprint 1 with the addition of the number of contributors.

### Instance 921
Since I determined this project is not active based on the commit history, number of issues, pull requests, and only having one contributor, I also
belive this project is not currently accepting contributions.

### Instance 4
I also determined this project to be inactive based on the commit history and lack of issues and pull requests. There is also only one contributor, so 
I believe this project is not accepting any new contributions as well.

# Sprint 3

Criteria used was comparing the vulnerability fixes in libpng and lighttpd with the files in the assigned repos.

### Instance 921
The vulnerability fix seems to be absent in pngread.c, however, the fix exists (although it is altered) in pngrutil.c. This leads me to belive these
vulnerabilities are still exploitable in this instance.

### Instance 4
The out of bounds read vulnerability in this instance is not fixed. There is no cast to an unsigned char in the same place as the fixed library. This
vulnerability is still exploitable.

# Sprint 4

### Instance 921
Added vulnerability fix for pngread.c.
https://github.com/CBrooks36/libgender_age_model.so/blob/ae7492f5df33e94fdddcb2869bf79000a304ebf8/opencv-3.4.5/3rdparty/libpng/pngread.c#L135

### Instance 4
Added vulnerability fix for http_auth.c.
https://github.com/CBrooks36/lighttpd-1.4.20/blob/1886dbbedc12e3b5a385f1387c306f16e80f1730/src/http_auth.c#L93
