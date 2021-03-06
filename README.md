# git-tute

Please ensure that you have git installed by running:

```
git --version
```

---

## Git installation

We will be using [package managers](https://en.wikipedia.org/wiki/Package_manager) to install git, so we do not need to deal with any installation wizards!

For Windows 11 users, run:

```
winget install -e --id Git.Git
```

For Mac users please run:

```
xcode-select --install
```

For Ubuntu users, run:

```
sudo apt-get update && sudo apt-get install git
```

If you were unable to install with one of the options above, please install through the [git website](https://git-scm.com/downloads)

## Git Setup

If this is your first time using git, you will need to set up your username and email.

Configure your username by running:

```
git config --global user.name "<Your Username>"
```

Configure your email by running:

```
git config --global user.email johndoe@example.com
```

## Exercise Setup

1. Open Terminal / Power Shell and change directory into where you would like to store project and run:

```
git clone https://github.com/codersforcauses/lets-git-started.git
```

Please nominate one person from your group to do steps 2-5

2. Create a new branch for your group by running (please create branch with the same name as your group):

```
git branch <name of branch>
```

3. To view all branches available (not on github), Run:

```
git branch
```

Now that we have created our branch, it is time we checkout(switch to) that branch so we can edit code!

4. to change to the branch created, Run:

```
git checkout <name of your branch>
```

5. Let push your newly created branch to github by running:

(name of remote will be origin for today)

```
git push <name of remote> <name of branch>
```

---

## Checkpoint!

Now that your group has created the branch, we need to update the repositories of other group members by running:

```
git pull
```

Once everyone in your group has updated their repository, please checkout to the branch created by your group

We will be running this command several times to 'pull' in changes made by our group members!

---

## Exercise

Please ensure that you are on the branch your group has created before continuing further!

1. Now that you are on your branch, you are free to do whatever you like with the code! For the excercise, create a copy of the template folder and rename it to the name of your group. Run:

```
cp -r ./template/ ./<name of group>
```

For this exercise, there are 4 files that require completion

```
addition.py
subtraction.py
multiplication.py
division.py
```

Lets start by correcting `addition.py`, modify the code so that it looks like this:

```py
def addition(a,b):
    return a+b
```

After saving your file, it is time to add this to the staging area by running:

```
git add addition.py
```

Once you are happy with your changes, it is time to commit! Don't forget to leave meaningful commit messages! Commit your change by running:

```
git commit -m "your commit message"
```

After commiting, we still need to push our changes to GitHub so they can be viewed by our team mates.
Push your changes by running:

```
git push origin <name of branch>
```

Work with your team to complete the other TODOs. For the purpose of this activity, please only modify 1 file per commit. Remember to push your changes and pull in changes made by your team.

---

## Adding changes to the main code base

Now that you are satisfied with changes on your branch, we need to merge these changes with our main branch so that your changes can be added into the codebase. Head over to the pull request section to create a new pull request.

There is no command for creating a pull request as a pull request is something that a cloud provider like GitHub, GitLab or BitBucket provide. It is not part of Git itself.

Once your code has been reviewed. Click squash and merge to merge your changes into the main branch.

---

## Suggestions and feed back

Please leave any suggestions for future events or feedback in `suggestions.txt` and submit by creating a pull request :)
