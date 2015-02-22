# questions

**Example: how to test my project using selenium ?**
- tell the integrator person to create a new machine(gitlab-ci-runner machine) and install selenium and register this machine on gitlab-ci machine
- gitlab-ci server should list the new registered machines(the runners)
- the developer can link a runner to his project (Notice: if we have a project in JS we want the runner to have npm pre-installed)


**can I change the runner-machine - and install another tool on it ?**
- yes, after we pick the runner - we have to edit the a webpage (Aka: 'custom-script') and type commands which will run on the runner machine after it cloned our repository. 


**how to be productive when I edit the custom-script ?**
- if I use command: 'npm install grunt' on the custom-script - is is not effective - tell the integrator-person to install grunt on the runner-machine and use that runner (tell him also to update the description of the runner such as: 'machine has: mongo, npm and grunt' )
