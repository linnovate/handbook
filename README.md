# Introduction

**goal**
Q: what is our **motivation** ?
A: we want to create a connection between **a code change(call it "a commit")** to an **automatic action(call it "a build")** which takes our code as a parameter and test it .


**the build process:**
Q: how to create 1 build for 1 commit ?
A: we use gitlab to store our code, and gitlab-ci server for creating a **build** for each code **commit**.


the gitlab-ci it the bridge between our code and the machine which run an operating system  and knows how to run spacific tasks ( for example: for a mean application we need the O.S to have Mongo and Node and Npm ).


