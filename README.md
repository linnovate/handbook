# Introduction

**goal**
Q: what is our **motivation** ?
A: we want to create connection between changes to our code and an automatic process which take our code commit as a parameter and prepare a build for it.


**the build process:**
Q: sound like integration between 2 servers, no ?
A: yes, we use gitlab to store our code, and gitlab-ci server for creating a **build** on each code **commit**.


**customising the test environment**
Q: how we test selenium for 1 project , and we use karma to test a 2nd project  ?
A: the gitlab-ci server is a bridge between different kind of "testers" and the repositories stored on the gitlab.

**how to customize a tester  ?**
- the tester is actually called the "runner-machine" it stores a machine which dedicated to run a project of type X.
- 

**Example: how to test my project using selenium ?**
- the integrator person has to create a machine which runs selenium.
- this runner-machine has to registered itself on the gitlab-ci server.
- the gitlab-ci server eventualy list the available runners
- the developer should pick a runner-machine which suite his projects needs.

