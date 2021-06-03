Новый проект для вебсайта лучше начинать с помощью composer, а не symfony cli, из-за периодических багов в последнем

    composer create-project symfony/website-skeleton my_project_name

Т.к. для разработки из под windows будет использоваться локальный вебсервер на базе apache, устанавливаем дополнение

    composer require symfony/apache-pack

Создаем новый контроллер. Это можно сделать вручную, но быстрее с помощью генератора (компонент MakerBundle уже установлен)

    php bin/console make:controller NameNewController

Просмотр url и маршрутов

    php bin/console debug:router

