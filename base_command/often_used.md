# Часто используемые

## git remote
Установка связи с удаленным репозиторием
```
git remote add name_app link_app
```

Удаление подключения к репозиторию
```
git remote rm name_app link_app
```

Переподключение к другому репозиторию
```
git remote set-url name_app link_app
```

Просмотр используемых репозиториев
```
git remote -v
```

Просмотр хэшей действующих ссылок
```
git ls-remote name_app
```

Просмотр доп информации по используемым репозияториям
```
git remote show name_app
```

Смена имени (alies) у репозитория
```
git remote rename old_name_app new_name_app
```

## git branch
Создание новой ветки
```
git branch new_branch
```

Просмотр локальных подключенных веток
```
git branch
```

Переход на другую ветку
```
git checkout other_branch
```

Создание новой ветки и одновременный переход на нее
```
git checkout -b new_branch
```

Копирование файла из текущей ветки в новую
```
git checkout other_branch -- file_or_path_to_file
```

Просмотр последний коммитов каждой ветки
```
git branch -v
```

Переименование ветки
```
git branch -m new_name_branch
```

### Варианты удаления веток
Удаление ветки при котором могут быть вызваны конфликты
```
git branch -d name_branch
```

Принудительное удаление ветки
```
git branch -D name_branch
```

Удаление ветки из удаленного репозитория
```
git push name_app -d name_branch
```

### Переход на удаленную ветку и добавление ее локально
Просмотр всех возможных веток
```
git branch -a 
```

Прямое подключение к удаленной ветке
```
git checkout name_app/name_branch
```

Добавление ветки на локальную машину
```
git checkout name_branch
```

## git add
Добавление новых файлов из текущей ветки в зону видимости гита
```
git add .
```

Добавление конкретного файла в зону видимости гита
```
git add file_name
```

Удаление измененного отслеживаемого файла или файлов из зоны видимости 
```
git restore --staged file_name
```

## git commit
Создание коммита для всех файлов в зоне видимости гит
```
git commit -m "message_about_changes"
```

Создание коммита для всех файлов в которых были изменения, даже если их нет в области видимости
```
git commit -a
```

Создание коммита для конкретного файла
```
git commit -m "message_about_changes" file_name
```

Изменение описания последнего незапушенного коммита
```
git commit --amend -m "New_commit_message"
```

## git status
Проверка состояния файлов/модулей
```
git status
```

## git diff
Просмотр всех изменений с последнего коммита
```
git diff
```

Просмотр изменений конкретного коммита
```
git diff hash_commit file_name
```

Сравнение изменений в файлах
```
git diff hash_commit file_name file_name
```

## git log
Просмотр всех логов
```
git log
```

Просмотр заданного количества коммитов
```
git log -n 3
```

Вывод дерева веток с коммитами
```
git log --all --graph --oneline
```

## git push
Отправка изменений на удаленный репозиторий
```
git push name_app branch_name
```


