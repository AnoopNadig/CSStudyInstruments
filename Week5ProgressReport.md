* Made significant progress regarding uniq. The function stat() seemed like the perfect candidate to perform the required check for character and block type devices. Created my initial patch based off of the information on it's man page. Made some modifications to my initial patch to make sure it didn't break any tests. Finally, reported the bug to Ubuntu's launchpad and also uploaded the patch. [Here's the link](https://bugs.launchpad.net/ubuntu/+source/coreutils/+bug/1808095)
* Continued working on chown as a root user and encountered two system calls without any handlers so raised issues for them:
  * [fstatat64()](https://github.com/pkmoore/rrapper/issues/86)
  * [fchownat()](https://github.com/pkmoore/rrapper/issues/87)
* Continued working on hostname as a root user and encountered issues with two system calls:
  * No handler found for sethostname() so raised an [issue](https://github.com/pkmoore/rrapper/issues/90)
  * Same issue with system call fstat64() as what I encountered last week with the command iostat so didn't raise an issue.
* Tried testing utility iotop for time related bugs but was unable to create a test. I suspect that a sub-process is being created.
* Also tried testing the utility tcpdump but was unable to replay the test as it just hangs indefinitely. Have to continue troubleshooting.
