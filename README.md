# Falling In Love with Git in Six Acts

##Act One. LUST :heart_eyes:
Here it is, the big “Wow!” the big “Gee!” the big “YesYesYes!” you’ve been waiting for...**YOU HAVE A NEW PROJECT ASSIGNMENT**. This is where you decide to build something better, greater, cuter, wiser, more wonderful than anything anyone has ever known. Lust isn’t a sin, it’s a necessity, for with lust as our guide we think: I have no need of food, I have no need of sleep, I have no needs other than occasionally chewing a breath mint. I am going to code my face off. And so it begins...

*There are two paths to the start of this journey. You must be comfortable in both.*

### Path-A) I create my project on the big Github :octocat: in the sky first:

- I visit my profile on GH and I create a new repo, following these [steps](https://help.github.com/articles/creating-a-new-repository/).
- Yay! I will now clone this very shiny new, empty repository onto my machine. And the lovely GH provides the [steps](https://help.github.com/articles/cloning-a-repository/) to do so.
- I do not have to ```git init``` in ```<my-awesome-project-name>```. Because I cloned from the big GH in the sky, I am all initialized with an empty .git repository. I am special. :tulip:
- And just to be sure all is well, I will double check that the project on my machine is in fact connected to the big :octocat: in the sky.
```
cd <my-awesome-project-name>
git remote -v
```
Eeeeeeeee!!!! :clap: Life is so good, because this:
```
# origin	git@github.com:you/my-awesome-project-name.git (fetch)
# origin	git@github.com:you/my-awesome-project-name.git (push)
```
I have the correct remotes in place for my local machine to both push and fetch from the big :octocat: in the sky.:thumbsup:

### Path-B) I create my project locally first:
```
mkdir <my-awesome-project-name>
cd <my-awesome-project-name>
git init
```
Boom. :boom: ```#Initialized empty Git repository in /Users/you/my-awesome-project-name/.git```

I want to share the love with everyone!!! How do I do this? OH RIGHT! I push my project up :arrow_up: to the big Github :octocat: in the sky. I will go there now and follow these [steps](https://help.github.com/articles/creating-a-new-repository/) to create a new repository.

:speech_balloon: BUT WAIT! Can they talk to one another? Is the project on my machine connected to my github repo? :confused: I get that for free when I clone from Github like in Path-A, but because I chose Path-B, I must create the connection between the two entities. I will do it. :muscle:
```
cd <my-awesome-project-name>
git remote -v
(# see that it is empty, nothing happens)

git remote add origin git@github.com:you/my-awesome-project-name.git
(# copy paste the GH url of your project and assign it to the label of 'origin')
(# side note, you could label it 'cupcake' if you wanted, although not recommended)
(# typical remote labels include things like 'staging', 'production', 'heroku')
(# use 'origin' for the your project's corresponding gh repo, because...convention)

git remote -v
(# check that you have the remotes in place)
```
You are ready to Rock and Roll. :microphone: :guitar:

##Act Two. EUPHORIA :lollipop:
You feel funny inside. You feel funny outside. You feel you could do anything and no one would dare laugh at you. This git and github, you will treasure. You will not put it in the basement next to your rowing machine, treadmill, and thermal body sweat wrap. And you will not take the git for granted, because that is the biggest sin of all. You will commit. And commit often. You will make your first commit like no other. Because you are solo. This is your repo, your project, your one-person-in-charge-of-every-last-commit-domain.

### You are making changes and coding things:
```
git status
(# prints the status of your current situation.)
(# expect git to tell you what you branch you are on)
(# expect git to tell you which files are "untracked", meaning changes were made)

git add .
(# this command will add ALL the changes you just made)
(# this command will add all those changed files to staging) 
(# files on staging are ready to be committed)

git add <path/filename>
(# this command will add changes based upon the file you specify)
(# this command forces you to think about each file before atomically adding all)

git status
(# run this command after EVERY git command)
(# actually read git's output messages)
(# do this until you know what you are doing)

```
### You are ready to commit:
```
git status
(# doublecheck the changed file names that are "staged" and ready for commit)

git commit -m "My awesome commit message"
(# you are happy with your staged changes then unapologetically commit)

git status
(# at this juncture, you might see "nothing to commit, working tree clean")
```
### You want to share your masterpiece with the world (aka "push to Github" :octocat:):
```
git push origin master
(# you are pushing your local commits up to the big :octocat: in the sky)
(# you are the master of your local commits and in charge of the master gh repo)
(# you care not about branches, nor collaborators - that comes in the next phase...)

```
But even though you are the master of your own domain, what if your gh is mistaken about this? What if you are DENIED? Never fear. The FORCE is with you:
```
git push -f origin master
(# you will now overwrite the entire repo on the big gh in the sky with your local copy)
(# it is good. it is powerful. it is necessary. it is also dangerous. think before you push)
```

##Act Three. FEAR :see_no_evil:
Now you must collaborate with a ###TEAM###. More than one person all up in your git and github. This is where the doubt begins, where the mind comes back from shopping, yells at the heart, binds and gags it to a nice lounge chair and allows guilt, failure, and remembrances of things past to sit in for a nice game of bridge. This is where you become afraid to commit, to push, to share anything with that damn :octocat:.

Add some collaborators to your gh repo. Follow these [steps](https://help.github.com/articles/inviting-collaborators-to-a-personal-repository/) and make sure you understand "collaborator access" - you are no longer the sole key holder of your kingdom.

```


```
- branching
- pull, merge, push order
- pull requests

##Act Four. DISGUST :poop:
Now comes that unavoidable time when you say to anyone who will listen: I got myself up git creek without a paddle! You have merge conflicts and find yourself desperately seeking a git blame. You've lost your teammates in a sea of git branching that has you feeling out of sync and off the reservation. You hate git. You hate collaborating. You pulled when you should of merged and then pushed. You force pushed and sunk the canoes of your teammates. You are a mess.

Points to add:
- git reset hard
- git revert
- git stash
- git force

##Act Five. TRUTH :raised_hands:
Git is not the enemy. If they didn’t tell you before, we will tell you now. Git is forgiving. Git is your friend. Anything you git, you can un-git. Git loves you. Git is easy, or at least it will be soon. Just don't git up. Git with it. And most importantly, this is only the beginning of git. It is enough to git you going, but there is so much more to learn. Go forth and explore, confident in your ability to navigate the git creek.

Points to add:
- git log
- git diff
- git gui tools, like github desktop and/or gitx?
- git rebase
- git interactive rebase

##Act Six. FINALE :sparkling_heart:
So this is git, as demanding and nourishing and difficult as it can be, and as strong and wise as it makes you become. There is something to be gained from commitment. There are rewards for staying when you would rather leave. And there is something to be said for running up that hill when you would rather slide down it. And so you let git come perch upon your shoulder. And you do not turn it away. You do the tango. Just git it.

(Add several great resources/tutorials for furthering study and becoming a "git master"):
____________________________________________________________________________________________________________________________
**(This love story inspired by [Nike's 1993 Vanity Fair Ad](http://www.rogerhorberry.com/falling-in-love-in-six-acts-courtesy-of-nike/))**
