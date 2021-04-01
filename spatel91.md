# Sprint 1

libpng - (Instance 820)

After examing this project i came to the conclusion that this project is no longer active. The last commit to this project was 6 days ago which just removed a single space. Other than that, the previous commit was from December of 2020. Additionally, this project has a lot of outstanding pull request and issues.

QEMU - (Instance 8)

This project is active becuase there was a commit made today. Additionally all of it's issues are resolved and pull request have been either approved or denied. Futhermore, there are multiple different users commit/contributing to this project. In conclusion, i would categorize this project as active

---

# Sprint 2

libpng - (Instance 820)

After examining this git repo, i came to the conclusion that this project still accepts contributions. Some of the most recent commits were done by three different contributors, who were relatively new contributors according to the commit history.

QEMU - (Instance 8)

This project also appears to accept contributions because the webstie states "QEMU welcomes contributions of code (either fixing bugs or adding new functionality)". However inorder to contribute to this project you have to submit a bug inquiry on their bug report page or submit patches to the website.

---

# Sprint 3

libpng - (Instance 820)

The vulnerability that i identified was the code's inability to determine if a data chuck being processed was too large. This vulnerabilty was fixed by adding pngpread.c and pngutil.c files, which checked the chuch size before processing. I concluded that this vulnerability was fixed in this project

QEMU - (Instance 8)

This project has a buffer overflow bug due to an interger variable being cast as a size_t variable. This bug can be solved simply by changing the type of the variable in question to size_t. This bug exist in pcnet.c and has not been fixed yet on their repo.
