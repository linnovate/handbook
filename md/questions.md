# questions


**how to test my project using selenium ?**
- tell the integrator person to create a new runner machine which contains selenium
- the gitlab-ci web interface should list the new registered machines(the runners)
- the developer can assosiate a runner with his project by selecting a runner from a list.

**can I change the runner-machine - and install another tool on it ?**
- yes, after we pick the runner - we have to edit the a webpage (Aka: 'custom-script') and type commands which will run on the runner machine after it cloned our repository. 


**how to be productive when I edit the custom-script ?**
- if I use command: 'npm install grunt' on the custom-script - is is not effective - tell the integrator-person to install grunt on the runner-machine and use that runner (tell him also to update the web-interface of gitlab-ci with a new description for the updated runner instance: 'Description: machine has: mongo, npm and grunt' )
