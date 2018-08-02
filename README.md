## Common commands for Git I used for development

#### For the first time, clone(get) the source files.
```
git clone <url>
```

#### If I create a project locally, then create a project in github
```
echo "# README" >> README.md
git init
git add *
git commit -m "first commit"
git remote add origin <url>
git push -u origin master
```

#### If there is some udpates from the branch, pull (fetch+merge)
```
git pull
```

#### If your are done with the bugs fix or new features, then push your files to main, there is a temporay local repo, you need to add it and commit and push.
```
git add *
git commit -m "I fix a bug"
git push
```

#### If there is issues with your local repos and you don't want to delete your updated files, do a hard reset.
```
git fetch origin
git reset --hard HEAD
git clean -fdx
```

#### For anytime, you can check the status.
```
git status
```

#### Remember to set your username and email.
```
git config --global user.name "moonbury"
git config --global user.email "moonbury@hotmail.com"
```
and/or localy
```
git config user.name "moonbury"
git config user.email "moonbury@hotmail.com"
```

#### Check out this post if you think you understand well.
[11 Painful Git Interview Questions You Will Cry On](https://dev.to/aershov24/11-painful-git-interview-questions-you-will-cry-on-1n2g?utm_source=digest_mailer&utm_medium=email&utm_campaign=digest_email)
