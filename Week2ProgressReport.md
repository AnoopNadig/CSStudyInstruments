* Switched to the new version of crashsim which doesn't require to configure the event number for creating replays.
* After experimenting more with utility uniq I concluded that there indeed was a bug as it wasn't performing any checks for the file types. Got the green signal to proceed to source code review. 
* During troubleshooting the issues for chown and hostname I realized that I had to create the tests as a root user. Preston also pointed out that it'll be interesting to use crashsim as a root user and rightly predicted that there'll be new issues. Performed further troubleshooting.
