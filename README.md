### Важное объявление

---

Этот проект является первой практикой в курсе по обучению GIT.
https://practicum.yandex.ru/git-basics/

---

#### Что сделал для решения практики?

* Инициировал новую директорию и привязал её к ГИТу
* На ГитХабе создал новый репозиторий
* Привязал локальный репозиторий к удаленному на ГитХаб
* Добавил файл readme.md с описание проекта
* Синхронизировал локальный репозиторий с удаленным (убедился, что все необходимые изменения есть на ГитХаб)

---

#### Mindmap на mermaid


```mermaid
mindmap
  root((GIT))
    Удаленный репозиторий
      Создание удаленного репозитория            
    Синхронизация репозиториев (локального и удаленного)
      1.Привязать удалённый репозиторий к локальному — git remote add. $ cd ~/dev/first-project $ git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git 
      2.Убедиться, что репозитории связаны, — git remote -v    
    Навигация по коммитам. Статусы файлов
        1.Git преобразует информацию о коммитах с помощью алгоритма SHA-1 и для каждого из них рассчитывает уникальный идентификатор — хеш. Хеш — основной идентификатор коммита и позволяет узнать его автора, дату и содержимое закоммиченных файлов. Все хеши, а также таблицу соответствий хеш → информация о коммите Git хранит в папке .git.
        2.Можно вызвать не только полный лог, но и сокращённый — это делается командой git log --oneline. В сокращённом логе выводятся сокращённые хеши — их можно использовать точно так же, как и полные.
        3.В числе прочих файлов в папке .git есть служебный файл HEAD. Он указывает на самый свежий коммит.Вместо хеша последнего коммита можно написать слово HEAD — Git вас поймёт.
        4.Статусы untracked/tracked, staged и modified. Статусом untracked помечается файл, о существовании которого Git знает, но не следит за изменениями в нём. Этот статус — противоположность tracked, в который попадают все файлы, отслеживаемые Git. Файл переходит в статус staged после выполнения git add. Статус modified означает, что файл был изменён. Большинство файлов в проектах «шагает» по следующему циклу: «изменён» → «добавлен в список на коммит» → «закоммичен» → «изменён» → и так далее.
        5.Команда git status всегда подскажет, что происходит с файлом: например, он добавлен в список «на коммит» или ещё вообще не отслеживается, или изменён. git status показывает явно следующие состояния файлов: untracked, staged и modified. git status подсказывает, какие команды можно выполнить, чтобы поменять состояние файла.
```
