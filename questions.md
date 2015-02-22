# questions

**Example: how to test my project using selenium ?**
- tell the integrator person to create a new machine and install selenium and register this machine on gitlab-ci
- then gitlab-ci server should list the new machine and we can setup our project to use that runner.


**can I change the runner-machine - and install another tool on it ?**
- yes, after we pick the runner - we have to edit the 'custom-script' and type commands which will run on the runner machine. 


**how to be productive when I edit the custom-script ?**
- if I use command: 'npm install grunt' on the custom-script - is is not effective - tell the integrator to install grunt on a runner-machine and use that runner.
