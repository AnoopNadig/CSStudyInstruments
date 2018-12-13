## Meta
* Project: iostat
* Project Bug Identifier: 
* Link to Bug on Project Bug Tracker: 
* Current Stage: Bug Hunting
* Brief description (This can change as you progress) : iostat is a utility used to monitor the performance of input/output devices.



## Updates


### Week 3

**Current Stage: Bug Hunting**

Tried using the time mutator but it didn't show any discernable differences during the replay.


### Week 4

**Current Stage: Bug Hunting**

Unable to complete the complete replay when manually changing the time values in the snip file or testing for weird filetypes as it failed when the system calls stat64() and write() were in the snip file. Here's the link to the issue I raised (https://github.com/pkmoore/rrapper/issues/81) which turned out to be an ongoing issue.

