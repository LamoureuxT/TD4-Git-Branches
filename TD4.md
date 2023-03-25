# TD4
## Exercice 1

### Q1
```

```
### Q2
```

```
### Q3
```
git clone https://github.com/LamoureuxT/TD4-Git-Branches/
```
### Q4
```

```

## Exercice 2

### Q1
```
git branch Thibaut
git checkout Thibaut
```
### Q2
```
touch Thibaut.txt
git add Thibaut.txt
```
### Q3
```
git commit -m "Add file created by Thibaut"
```
### Q4
```
git push -u origin Thibaut
```
## Exercice 3

### Q1
```
git checkout main
git config pull.rebase false
git merge Thibaut
```
### Q2
```
git commit -m "Merge Thibaut into main"
git pull
git push
```
## Exercice 4
```
git checkout Thibaut
vim README.md
git add README.md
git commit -m "Update README.md with new text"
git checkout main
git pull origin main
git merge Thibaut
git push origin master
```
## Exercice 5

```
git checkout main
git pull origin main
git checkout Thibaut
git merge main
git add README.md
git commit -m "Merge main to branch"
git push origin Thibaut
```

## Exercice 6

```
git branch -d Thibaut
git push origin --delete Thibaut
```

## Exercice 7

```
git checkout main
git pull
git checkout Thibaut
echo "" > README.md
echo "Git interactive rebase" > README.md
nano README.md
echo "Changing Multiple Commit Messages" >> README.md
sed -i '11d' README.md
sed -i '10i Changing Multiple Commit Messages' README.md
echo "Created by Thibaut" >> README.md
git rebase -i HEAD~n
#n the number of commit that you do
git push -u origin Thibaut
```

## Exercice 8

```
git checkout main
git pull origin main
git checkout Thibaut
git rebase main
git push -f origin Thibaut
```
