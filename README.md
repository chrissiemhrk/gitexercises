# Git Exercises

## Bundle 1

### Exercise 1 

```bash
 mkdir gitexercises
 cd gitexercises
 git init
 git branch -m 'main'
 touch index.html
 gaa && gcmsg "initial commit"
 git remote add origin https://github.com/chrissiemhrk/gitexercises.git
 git push -u origin main
 git checkout -b dev
 git checkout -b test
 git checkout dev
 git branch -d test
```

### Exercise 2 

```bash
 vim home.html
 git add .
 git stash
 git stash list
 vim about.html
 git add .
 git stash
 git stash list
 vim team.html
 git add .
 git stas
 git stash
 git stash list
 git stash pop stash@{1}
 git add . && git commit -m 'add home and about page'
 git push
 git push --set-upstream origin dev
 git stash pop stash@{0}
 git reset --hard
```

## Bundle 2

### Exercise 1

```bash
git checkout -b ft/bundle-2
vim services.html
git add . && git commit -m 'add services page' && git push
git push --set-upstream origin ft/bundle-2
```

### Exercise 2 

```bash
git checkout main
git pull
git checkout -b ft/service-redesign
vim services.html
git add . && git commit -m 'add offered services' && git push
git push --set-upstream origin ft/service-redesign
git checkout main
vim services.html
git add . && git commit -m 'list offered services' && git push
git checkout ft/service-redesign
git diff
git merge main
git add . && git commit -m 'fix mmerge ocnflict with main' && git push
```

## Bundle 3

### Exercise 1

```bash
git checkout main
git checkout -b ft/team-page
vim team.html
git add . && git commit -m 'add team page' && git push
git push --set-upstream origin ft/team-page
git checkout main
git checkout -b ft/contact-page
git checkout ft/team-page
git log
git checkout ft/contact-page
git cherry-pick ccd18dbc03784cd244e84c73edf809de0fefd5b0
git add . && git commit -m 'add team page from ft/team-page' && git push
git status
git push
git push --set-upstream origin ft/contact-page
git checkout ft/faq-page
git checkout -b ft/faq-page
vim faq.html
git add . && git commit -m 'add faq page' && git push
git push --set-upstream origin ft/faq-page
git log
git checkout ft/team-page
git log
git checkout ft/faq-page
git revert ccd18dbc03784cd244e84c73edf809de0fefd5b0
git status
git log
git push
```

### Exercise 2

```bash
git checkout -b ft/home-page-redesign
git checkout main
vim home.html
git add . && git commit -m 'change heading of the home page' && git push
git checkout ft/home-page-redesign
git rebase main
vim home.html
git add . && git commit -m 'upadte heading of the home page' && git push
git push --set-upstream origin ft/home-page-redesign
```

## Bundle 4

### Exercise 1

```bash
git checkout main
git remote add git-copy https://github.com/chrissiemhrk/gitexercises-2.git
vim home.html
git add . && git commit -m 'add paragraph to the home page'
git push origin
git push git-copy
```

### Exercise 2 

```bash
 git checkout -b ft/footer
 vim footer.html
 git add . && git commit -m 'add footer'
 vim footer.html
 git add . && git commit -m 'add copyright to footer'
 git push
 git push --set-upstream origin ft/footer
 git checkout main
 git checkout -b ft/squashing
 git merge --squash ft/footer
 git add . && git commit -m 'footer changes squashing'
 git push --set-upstream origin ft/squashing
```

## Bundle 5

### Exercise 2

```bash
git clone https://github.com/chrissiemhrk/git-cafe-exercise.git
cd git-cafe-exercise/
vim index.html
git add . && git commit -m 'edit heading text' && git push
```
