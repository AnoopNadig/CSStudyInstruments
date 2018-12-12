## Meta
* Project: hostname
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: 
* Brief description (This can change as you progress) : utility displays and sets the hostname of the system


## Updates


### Week 1

**Current Stage: Bug Hunting**

Observed hostname accepts different file types. Need to explore further.

### Week 2

**Current Stage: Bug Hunting**

Unable to complete rreplay after the switch to the experimental branch. Identified the fix was to run the rrtest as a root user.

### Week 3

**Current Stage: Bug Hunting**

Ran into various problems while trying to use crashsim as a root user. Chief among them was that the self.pickle file wasn't being created. Preston pointed out to install the setup the crashsim environment again as a root user.

### Week 4

**Current Stage: Bug Hunting**

I was unable to work on this project.

### Week 5

**Current Stage: Bug Hunting**
Unable to complete the replay as I encountered issues with two system calls:

sethostname(): No handler found so raised an issue (https://github.com/pkmoore/rrapper/issues/90)

fstat64(): Didn't raise an issue as it's part of an ongoing issue.
