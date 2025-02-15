# GitCLI
GitHubCLI

## Скачивание и установка GitCLI
```shell
winget install --id GitHub.cli
```

## Проверить\посмотреть версию GitCLI
```shell
gh --version
```

## Настройка и авторизация
```shell
gh auth login
```

## Создание репозитория
```shell
gh repo create "simple-GitHubCLI" --public
```

## Просмотр всех удалённых(на сервере) репозиториев
```shell
gh repo list
```

## ```shell
gh auth refresh -h github.com -s admin:public_key
```

## Генерируем ключ
```shell
ssh-keygen -t rsa -b 4096 -C "griarsvah@gmail.com"
```

## Копируем ключ

## Добавляем SSH-ключ ([doc](https://docs.github.com/ru/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=cli)) в GitHub через GitHub CLI
```shell
gh ssh-key add ~/.ssh/id_rsa.pub --title "Title"
```

## Проверяем работоспособность
```shell
ssh -T git@github.com
```

## Связываем локальный репозиторий с удаленным репозиторием на GitHub
```shell
git remote add origin https://github.com/griarsvah/simple-GitHubCLI.git
```

## А вот теперь
```shell
git push -u origin main
```

## pages.github
```shell
gh repo edit griarsvah/simple-GitHubCLI --source <source>
```
