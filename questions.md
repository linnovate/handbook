# questions

**Example: how to test my project using selenium ?**
- the integrator person has to create a machine which runs selenium.
- this runner-machine has to registered itself on the gitlab-ci server.
- the gitlab-ci server list available runners
- the developer should pick a runner-machine which suite his projects needs.


**can I change the runner-machine - and install another tool on it ?**
- yes, for interacting with the runner-machine we use a "bridge"
- this bridge is a blank bash script which we can edit
- we can add commands on the custom-scripts
- the custom script is run by the tester-machine.


**how to be productive when I edit the custom-script ?**
- if for example I want to test a Mean-Application, I need node-modules such as grunt.
- so I can type in the custom-script: npm install grunt
- it might me more efficient to tell the integrator-person to pre-install grunt on the runner-machine.