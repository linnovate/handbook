# custom_script.sh

[ Example: for gitlab-project-id: **4** ](http://ci0.gitlab.linnovate.net/projects/4/edit)


```bash
git checkout testing              #switch to a branch which contain the selenium-tests
git pull                          #get the selenium test-suite 
ls -la   
/extra/.test_me_please.sh         #run a script which looks for suite.json and run its tests.
```