# questions

 **w.t.f is a build ?**
- a build is the test-suite that we can run on our code (like: "grunt test" )
- a build finished with a status: 'test ok' OR 'test error'.



**customising the test environment**
 Q: how we test selenium for 1 project , and we use karma to test a 2nd project  ?
 A: the gitlab-ci server is a bridge between different kind of "testers" and the repositories stored on the gitlab.


**how to customize a tester  ?**
- the tester is actually called the "runner-machine" it stores a machine which dedicated to run a project of type X.


**Example: how to test my project using selenium ?**
- the integrator person has to create a machine which runs selenium.
- this runner-machine has to registered itself on the gitlab-ci server.
- the gitlab-ci server eventualy list the available runners
- the developer should pick a runner-machine which suite his projects needs.


**can I change the runner-machine - and install another tester on it ?**
- yes, for interacting with the runner-machine we use a "bridge"
- this bridge is a blank bash script which we can edit
- we can add commands on the custom-scripts
- the custom script is run by the tester-machine.


**how to be productive when I edit the custom-script ?**
- if for example I want to test a Mean-Application, I need node-modules such as grunt.
- so I can type in the custom-script: npm install grunt
- it might me more efficient to tell the integrator-person to pre-install grunt on the runner-machine.