1.Все объекты хранятся в сжатом виде по имени их sha значения. Они содержат тип объекта, размер и содержимое в формате gzipped.
Главная отличительная черта Git состоит в подходе к обработке данных. Каждый раз при сохранении данных проекта (коммите) система фиксирует состояние файла (делает снимок) и создает ссылку на этот снимок. Последующие изменения отражаются через ссылки на более ранние версии файла. Нет необходимости снова сохранять файл целиком. К тому же, основываясь на контрольных hash-суммах, система снимков обеспечивает целостность всей истории изменений. На практике это означает, что невозможно (либо крайне трудно) полностью удалить данные из рабочего каталога и утратить к ним любой доступ. В большинстве случаев данные можно восстановить из ранней версии проекта.
Таким образом, систему контроля версий в Git проще всего представлять как поток снимков (сохраненных состояний проекта).

2.git config --list --show-origin (mkdir project-dir
cd project-dir
git init)

3.$ cd C:/Users/user/my_project
$ git init
$ git add *.c
$ git add LICENSE
$ git commit -m 'Initial project version'

4. it add <filename> <filename> - добавит нескольких файлов по имени

  5.https://github.com-> Profile or Top repositories on (https://github.com) -> new repository -> in the window “Repository name”  write Name of repository ->  choose “Public or Private” -> on down, tap “Create repository” -> upload New File. => git push -u origin master

  6. curl -u 'USER_NAME' https://api.github.com/user/repos -d'{"name":"demo"}' -> Создаем удаленный репозиторий, указывая имя учетной записи
Enter host password for user 'USER_NAME': -> Вводим пароль от учетной записи
Репозиторий demo создан
git remote add origin https://github.com/USER_NAME/demo.git
git push -u origin master -> Теперь выгружаем проек



