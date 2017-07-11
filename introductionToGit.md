# An introduction to git

First, let’s start with github. I’m guessing most of you know what github is, but for those who don’t, I will explain it.

## What is github?
Github is a platform that a lot of developers use. Developers can create a repository (folder), for a project that they are working on. They can place their code on here, and write a README.md which explains what the project is. Other developers can watch this code (if the repository is public) and they can suggest changes, by creating an issue. Or when the change is bigger, they can create a pull request. As you can hear, github is a great platform where developers can benefit from other developers code and they can work together, to make each other’s work better.

Now I will explain some of the terms I used above.
A README.md is a file every github repository should have. A readme is written in markdown, a type of code, that allows you to create headers, **bold**/*italic* text, etc. When the markdown file is called README, github will automatically render it on the bottom of the repository. The markdown code will be rendered like a normal document.

An issue is something each repository has. When something on the project is missing, or has yet to be done, you can create an issue. You can give issues a label like ‘must-have’, ‘enhancement’ or ‘could-have’. This way you’ve made a task list for yourself, which also shows what task is more important than the other.

With a pull request, you can suggest a code change in the project of someone else. Say you are using someone else’s code for your own project, and you see some things in the code that can be improved. You can create a pull request with those changes. The project owner can see what changes you’ve made and if he likes them, he can pull your suggestions into his own project.

## But, what is git?
Git is a software that runs in the terminal of your computer. Github is the social network around it. So, with git you can create, add, commit and push to repository.
With git you can connect folders on your computer to a repository on github, with this connection, you can push the code from your computer, to your github repository.

### So how do you set up
When you create a repository on github, github already gives you the steps you have to do, to link the repo to your folder with git. (See the image below)
![Connect repo to folder](/images/repo.jpg)
<sup>1: github.com</sup>

If you follow the steps above, your folder is linked to the github repository. The results from these steps are shown in the image below. After this you can execute the git commando’s that will push your code onto the repository.

![Repo is connected to folder](/images/repo-made.jpg)
<sup>1: github.com</sup>

 
### The basic git commando’s
There are a few basic commando’s you’ll have to know when you want to use git. I will explain this to you with a small example.

Say you’ve connected your folder to the repository and after that you created your index.html file. In your command line, you browse to your folder. If you run the commando `git status`. You can see that the file index.html is created. But still is red, because you haven’t added it with git yet.

The next commando you have to run is `git add index.html`. This will add your index file to git. If you’ve edited a lot of files you can also run `git add .`. The point stands for ‘all’, so you will add all the files at once. Which will save you some time.

After adding the files, you’ll want to commit your files. With a commit, you can say what you did in these changes. The commando you have to run is `git commit -m “[your message]”`. In this message, you can for example say: “Create index.html”.
When other developers will read this commit, they know what you’ve changed, and in a commit, they can also see what files you’ve changed.

But before these steps will be visible on github, you have to push your changes. **NOTE:** You don’t have to push after every commit. You can commit 10 times, and push them at once, that is no problem. Though, you have to add every time you want to commit.
Once you think the code is ready to push to github. You run the commando `git push`. <sup>2: rogerdudler.github.io/git-guide/</sup>

TIP: First check your changes on your localhost or what you’re testing on. Only commit something that works, so your commit flow on github will be a logical flow. Instead of a lot of commits that say something like ‘Fixing error’ or ‘Rewrite code so it does work’.

Of course, git has a lot more commando’s for much more complicated stuff. But for now, this will do just fine. With these basics, you can upload your projects to github without any problems. And of course, if a problem does appear, just google for it, on stack overflow almost all problems are answered.


## Sources
1.	https://github.com/shyanta/minor-weeklyNerdArticles
2.	http://rogerdudler.github.io/git-guide/
