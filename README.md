# r001-lemp
Учебный проект LEMP c простым кодом. 
Стек: nginx + PHP + MySQL.
Автоматизация деплоя через Actions в папке .github/workflows.
Автоматизация в плейбуке в файле mywf.yml.
Необходимо задать переменные (env), определяющие сайт, например:
  SERVER_HOST: '85.28.47.165'
  SERVER_USER: root
  SERVER_PATH: /var/www/trur/
А также установить приватный ключ (secrets.PKEY), который сопряжен с публичным ключом, лежащим на сервере в файле authorized_keys.
Для установки приватного ключа (дать имя PKEY), нужно перейти в раздел репозитория Settings -> Security -> Secret and variables -> Actions -> Secrets -> Repository secrets -> New repository secret.
Даем имя (PKEY), вставляем приватный ключ и сохраняем (add secret).
ВНИМАНИЕ! Автоматизация вызовет ошибку, если на сервере не установлен rsync.
******************************************************************************************************
МАТЕРИАЛЫ ДЛЯ ДАЛЬНЕЙШЕГО ИЗУЧЕНИЯ PHP
[1] Канал на yutube Kirill Kocherov "Простенький сайт с авторизацией"
https://www.youtube.com/watch?v=u2mDQIP_fds

