# Участие в проекте

Спасибо за интерес к нашему проекту!

Вне зависимости от уровня вашей подготовки мы приглашаем вас поучаствовать в развитии проекта. В *Hexlet-CV* есть разные направления по разработке, в которых вы можете на практике применить свои знания.

## Указать на баг или неточность

Перед тем как сообщить о какой-либо ошибке, проверьте, не сообщили ли о ней ранее в [issue-трекере.](https://github.com/Hexlet/hexlet-cv/issues)

## Взяться за выполнение задачи

На нашем [issue-трекере](https://github.com/Hexlet/hexlet-cv/issues) вы можете выбрать интересующую вас задачу и взяться за ее выполнение. Перед этим желательно согласовать свои действия с другими участниками, описав свой план действий и оповестив их о том, что приступили к работе. Если кто-то уже взялся за выполнение задачи, то вы все равно можете начать выполнять ее, а лучше всего скооперироваться с теми, кто ее уже выполняет.

Если вы не можете подобрать себе задачу, но очень хотите поучаствовать, то обратитесь за помощью в [Telegram-сообщество](https://t.me/hexletcommunity/12) Хекслета. 

## Как начать разработку

1. Если у вас нет SSH-ключей, [сгенерируйте и подключите](https://help.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account) их к гитхабу, чтобы работать с репозиторием по SSH.

1. Ознакомьтесь принципами разработки с принятыми в этом проекте.
    1. Качество:
       * Весь код прогоняется через линтеры.
       * Любая фича неотделима от своих тестов. Фича без тестов - не фича 
       * Баги сначала нужно воспроизводить тестами, а потом писать исправляющий код.
       * Увидел неточность в README или любом описании - поправь.
       * https://12factor.net/
    2. Автоматизация:
       * Всё, что автоматизируемо, должно быть автоматизировано. Думайте о тех, кто работает рядом с вами.
       * Развёртывание девелоперского окружения должно работать с одной кнопки ( команды ).
   
1. Сделайте fork проекта ( кнопка fork в правом верхнем углу на странице <https://github.com/Hexlet/hexlet-cv> ) и клонируйте репозиторий:

    ```bash
    git clone git@github.com:%your-username%/hexlet-cv.git
    ```

1. Следуйте [инструкциям по установке](https://github.com/Hexlet/hexlet-cv/blob/main/README.md#install).

1. Перед тем как начать писать код, необходимо создать ветку ( например _iss7_ ) для разработки из ветки `main`. Важно учитывать, что в одной ветке может находиться решение только одной задачи!

    ```bash
    git checkout main
    git checkout -b %your_branch_name%
    ```

1. После выполнения задачи закоммитите изменения. Комментарии коммита пишем на английском [со ссылкой на PR](https://help.github.com/articles/closing-issues-using-keywords) ( пример: "Create new footer [issue 7]" ). 
    * Справочно [Соглашение о коммитах](https://www.conventionalcommits.org/ru/v1.0.0/)

    ```bash
    git add . && git commit -m "%useful_commit_message%"
    git push --set-upstream origin %your_branch_name%
    ```

1. Создайте `pull request`.

## Создание pull request 
Чтобы создать PR, необходимо:

* Убедитесь, что все тесты выполняются успешно и линтер не выдает ошибок
* Зайте на [основной репозиторий](https://github.com/Hexlet/hexlet-cv)
* Скорее всего гитхаб сам предложит вам создать PR. Или самостоятельно по [инструкции](https://help.github.com/articles/creating-a-pull-request)
* После завершения работы над задачей следует [синхронизировать ваш fork с основным репозиторием](https://help.github.com/articles/syncing-a-fork/).

[Подробные инструкции по работе с PR](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)

## Создание первого pull request
* Создать ветку ( например firstPR )
    ```bash
    git checkout -b firstPR
    ```
* В файл FirstPR.txt написать приветственную фразу ( например Hello world ).
* Закоммитеть изменения:
    ```bash
    git add . && git commit -m "This is the first PR"
    git push --set-upstream origin firstPR
    ```
* Зайти на [основной репозиторий](https://github.com/Hexlet/hexlet-cv)  и создайть PR

После того как PR будет принят, можно будет вернуться на ветку main, [обновить](https://docs.github.com/ru/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) репозитории и удалить ветку firstPR

    ```bash
    git checkout main
    git pull 
    git branch -d firstPR 
    ```

### Спасибо за помощь `!`

