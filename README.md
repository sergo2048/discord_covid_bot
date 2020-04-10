# Бот для Discord выводящий статистику вируса COVID19 #

## Содержание ##

* [Создание discord бота](#creature)
* [Функционал](#function)
* [Настройка](#settings)

<h2 id='creature'> Создание бота в Discord </h2>

Для создания бота перейдите по [ссылке](https://discordapp.com/developers/applications). Далее необходимо нажать на **New Application**, и указать имя нашего приложения.

![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/create.png)

Создав приложение, необходимо создать самого *бота*. Для этого переходим в раздел **bot**, указываем имя бота, а так же, ниже, выбираем его *права*.

![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/bot_creation.png)

По сути бот готов. Копируем его **TOKEN** и сохраняем в отдельный файл (у меня это *settings.py* ~~тут показывать не буду~~). Потом мы будем импортировать этот *токен* в основную программу для подключения.

Теперь осталось добавить бота на наш канал. Для этого переходим на вкладку OAuth2, ставим галочку где bot, а так же выбираем его возможности (это кстати очень важно).

> **НЕ ДАВАЙТЕ БОТУ БОЛЬШЕ ПРАВ ЧЕМ ТРЕБУЕТ ЕГО ФУНКЦИОНАЛ**

![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/add.png)
![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/permission.png)

После всего этого просто копируем сгенерированную ссылку, переходим по ней и выбираем канал, на который мы хоти добавить бота.

![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/conected.png)

Если вы все сделали правильно, то бот должен был присоединиться к каналу.

<h2 id='function'> Функционал </h2>

На данный момент бот поддерживает 5 основных команд:

* $hello - здоровается с пользователем отправившим команду.
* $info - выводит в чат информацию о своих возможностях.
* $world - выводит инфомацию o covid19 по миру.
* $russia - выводит инфомацию o covid19 по России.
* $country+<Название страны> - выводит инфомацию o covid19 по указанной вами стране.

Зная это вы спокойно сможете использовать моего бота.

![/images/1.png](https://raw.githubusercontent.com/sergo2048/discord_covid_bot/master/images/small.png)


<h2 id='settings'> Настройка </h2>

Для того что бы бот нормально работал, необходимо создать файл **settings.py**, в котором нужно указать:

* **BOT_TOKEN**  = <токен который мы получили в личном кабинете>
* **INFO** = <То что будет выводится на экран при $info>

Например:

INFO = ''' Привет :innocent:, я создан что бы следить за ситуацией с covid-19 :microbe: в мире не выходя из твоего любимого discord.
Что бы узнать о ситуации в мире напиши $world :earth_asia:,
Что бы узнать о ситуации в России матушке напиши $Russia :flag_ru:,
Что бы узнать про другую страну напиши $country+<Название страны> :rainbow_flag:'''
