# Git commands lists

## 📁 Create a new repository on the command line

```bash
echo "# Hi This is my Readme file" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin git@github.com:BiratAryal/Automation.git
git push -u origin master
```

## 🔄 Push an existing repository from the command line

```bash
git remote add origin github:BiratAryal/<git repo name>.git
git branch -M master
git push -u origin master
```
 *github is the alias that has been defined on the ssh config where ssh key based authentication has been done.*