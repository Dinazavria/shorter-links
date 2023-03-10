# О проекте

Это мой дипломный проект в рамках курса "Fullstack" от itproger.com

# Техническое задание

Необходимо создать веб-ресурс по сокращению ссылок для успешной сдачи диплома. Проект, что вы будете создавать, должен выполнять следующее:

* весь проект должен быть реализован с учетом ООП и MVC;
* использовать Laravel, а также WordPress не нужно;
* система регистрации и авторизации;
* личный кабинет;
* страница контакты, где отправление на почту происходит через библиотеку PhpMailer;
* добавление ссылки и создание её сокращения;
* вывод и удаление ссылок;
* переадресация на другой веб сайт при переходе по сокращенной ссылке.

## Требования к функционалу

1. На главной странице должна отображаться форма регистрации или же форма добавления ссылки. Это зависит от того зарегистрирован ли пользователь на сайте. В форме регистрации необходимо выполнить проверку на логин пользователя. Если в базе данных уже есть такой же логин, что вводит пользователь для регистрации, то должна выдаваться ошибка:

> Пользователь с таким логином уже существует
2. Форма авторизации должна принимать логин и пароль и в зависимости от их корректности либо авторизовывать пользователя, либо выводить ошибку под формой:

> Пароли не совпадают
3. В личном кабинете необходимо отобразить лишь Логин пользователя, а также кнопку выход:

> Привет, [имя]
4. Если пользователь авторизован, то на главной странице он может указать длинную ссылку, а также указать сокращение и создать сокращенную ссылку. Если он вводит сокращенное имя что уже есть в базе данных, то должна вызываться ошибка:

> Такое сокращение уже используется в базе
5. Все ссылки что создал конкретный пользователь отображаются для него на главной странице. Каждую ссылку можно удалить

При переходе по сокращенной ссылке пользователя должно перекидывать на тот URL адрес, который использовался в качестве длинного URL.

На странице с контактами пользователь сможет отправить письмо к вам на почту. Отправка письма должна происходить не через встроенную функцию mail(), а через библиотеку PhpMailer.
