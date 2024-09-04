# Занятие 1

### Настройка конфигурации GIT

```shell
git config --global --list
git config --global user.name <username>
git config --global user.email <username@gmail.com>
```

### Инициализация репозитория и первый коммит

```shell
git init -b main
git status
echo .idea >> .gitignore
git status
git add .
git status
git commit -m "Initial commit"
git remote add origin git@github.com:ArtemE91/MISIS.git
git push -u origin main
```

### Создание ветки и ускоренное слияние
```shell
git branch feature 
git checkout feature 
git branch 
echo "feature branch" > lesson1/.keep
git status
git add .
git commit -m "the first commit in the branch feature"
git checkout main
git merge feature
```

### Трехслойное слияние
```shell
git checkout feature
git merge main
echo "the second commit in the branch feature" > lesson1/.keep
git add .
git commit -m "the second commit in the branch feature"
git checkout main
```
