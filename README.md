# nginx-config-samples
Some sample pattern ideas for nginx and services


* single host location routing
* multi-host routing
* map based dispatch routing


| Method | Pros | Cons |
| :----- | :--- | :--- |
| [Single Host][1] | <ul><li>Upstream and locations in a single config</li></ul> | <ul><li>Will get verbose quickly if your back-end API is handling lots of end-points per service.</li></ul> |
| [Multiple VHosts][2] | <ul><li>Simplest configuration management</li><ul> | <ul><li>Requires multiple (sub-)domains so you lose a clean landing interface.</li><ul> |
| [Mapped Dispatch][3] | <ul><li>Self-contained `upstream` directives.</li><li>Simple server configuration with just 2 end-points. One for `discovery` and one for all the mapped end-points.</li><ul> | <ul><li>Mapping config will have to be re-written with every new upstream service added.</li><ul> |


[1]: ./single-host/
[2]: ./multi-host/
[3]: ./map-dispatch/
