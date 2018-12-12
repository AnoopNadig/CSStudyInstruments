## Meta
* Project: chown
* Project Bug Identifier: 
* Link to Bug on Project Bug Tracker: 
* Current Stage: Bug Hunting
* Brief description (This can change as you progress) : chown changes the ownership of a file



## Updates


### Week 1

**Current Stage: Bug Hunting**

Trying to use crashsim to search for a filetype bug in the command chown.

### Week 2

**Current Stage: Bug Hunting**

Unable to complete rreplay. Identified the fix was to run the rrtest as a root user.

### Week 3

**Current Stage: Bug Hunting**

Ran into various problems while trying to use crashsim as a root user. Chief among them was that the self.pickle file wasn't being created. Preston pointed out to install the setup the crashsim environment again as a root user.

### Week 4

**Current Stage: Bug Hunting**

I was unable to work on this project.

### Week 5

**Current Stage: Bug Hunting**

Unable to complete the replay as I encountered two system calls without any handlers. Here are the links to their issues:
fstatat64(): https://github.com/pkmoore/rrapper/issues/86
fchownat(): https://github.com/pkmoore/rrapper/issues/87

