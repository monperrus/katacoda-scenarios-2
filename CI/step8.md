**Note:** This part can only be done on your local machine. If you have done the previous steps on Katacoda, it's now time to fork and clone [this repo](https://github.com/nwessman/katacoda-scenarios/tree/express-app-complete). Make sure to fork the repo before cloning since *step: 8* requires you to have permission to push to the repository. 

The source code of the complete project, including the code implemented in *steps 1-7*, resides in the branch `express-app-complete`. Checkout to this branch before you continue.

#### Activating the Github Action in your fork

Github will have a problem recognizing our Action-file when forking a repository with the file already existing. To activate it, we must rename the Action-file and push the changes. This notifies Github to register the new file as a Github Action config file and the Actions magically start working. Let's do this!

Rename the file `.github/workflows/CI.yml` to `.github/workflows/CI-fork.yml`.

**Note:** It is important that you do not use Git's file renaming feature, since it will not fool Github that we have created a new file.

#### Test the Action

You can try pushing dummy changes to your project to see the status of the automatic tests, for instance, by changing a comment in the file `index.js`.

To see the status of your Github Actions, go to the action tab on your Github project. Here you can see a list of all your push and pull requests, including the automatic testing and linting status.
![Github action tab](https://github.com/nwessman/katacoda-scenarios/blob/main/CI/assets/Action-bar.jpg?raw=true)
<br/>

A green marker means that the tests have passed, a yellow that the tests are still conducted, and a red means that the tests have failed. Click on an instance to get more information on the tests, where they failed, and so forth.
![Github action tab](https://github.com/nwessman/katacoda-scenarios/blob/main/CI/assets/Actions-workflow.jpg?raw=true)
<br/>

The status marker can also be seen in your commit history
![Commit status](https://github.com/nwessman/katacoda-scenarios/blob/main/CI/assets/Commit-checkbox.jpg?raw=true)
