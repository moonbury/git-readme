## Common Git commands I used in development

For the first time, clone(get) the source files.
```
git clone <url>
```
If I create a project locally, then create a project in github
```
echo "# README" >> README.md
git init
git add *
git commit -m "first commit"
git remote add origin <url>
git push -u origin master
```

If there is some udpates from the branch, pull (fetch+merge)
```
git pull
```

If your are done with the bugs fix or new features, then push your files to main, there is a temporay local repo, you need to add it and commit and push.
```
git add *
git commit -m "I fix a bug"
git push
```

If there is issues with your local repos and you don't want to delete your updated files, do a hard reset.
```
git fetch origin
git reset --hard HEAD
git clean -fdx
```

For anytime, you can check the status.
```
git status
```
If need to reorganize files or folders.
```
git mv <file1> <file2>
git rm <file>
```

Remember to set your username and email.
```
git config --global user.name "moonbury"
git config --global user.email "moonbury@hotmail.com"
```
and/or localy
```
git config user.name "moonbury"
git config user.email "moonbury@hotmail.com"
```

For simiplist, you may add the .gitignore file, see [ignore file template](https://github.com/github/gitignore/blob/master/Node.gitignore)
```
touch .gitignore
```

Create a Development branch & work on the development branch
```
git checkout -b develop master
git checkout develop
```
When done, merge back to master branch
```
git checkout master
git merge --no-ff develop
git branch -d develop
git push origin develop
```

Check out this post if you think you understand well.
[11 Painful Git Interview Questions You Will Cry On](https://dev.to/aershov24/11-painful-git-interview-questions-you-will-cry-on-1n2g?utm_source=digest_mailer&utm_medium=email&utm_campaign=digest_email)

More information can be found [here](https://nvie.com/posts/a-successful-git-branching-model/)
