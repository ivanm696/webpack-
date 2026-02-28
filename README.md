логотип webpack

вебпак
API
Введение
Интерфейс командной строки
Интерфейс узла
Статистические данные
API webpack-dev-server
Замена модуля в горячем состоянии
Интерфейс загрузчика
Интерфейс регистратора
Методы модуля
Переменные модуля
Объект компиляции
Перехватчики компилятора
Компиляционные хуки
Хуки ContextModuleFactory
JavascriptParser Hooks
Хуки NormalModuleFactory
API плагинов
Резолверы
блог
Блог
Дорожная карта 2021 (08.12.2020)
Релиз Webpack 5 (10.10.2020)
Дорожная карта 2026 (04.02.2026)
Webpack 5.105 (2026-02-03)
концепции
Концепции
Точки входа
Выход
Погрузчики
Плагины
Конфигурация
Модули
Разрешение модуля
Федерация модулей
Граф зависимостей
Цели
Манифест
Замена модуля в горячем состоянии
Почему webpack?
Под капотом
конфигурация
Конфигурация
Языки конфигурации
Типы конфигурации
Вход и контекст
Режим
Выход
Модуль
Решать
Оптимизация
Плагины
DevServer
Кэш
Инструменты разработчика
Расширяет
Цель
Watch и WatchOptions
Внешние
Дотенв
Узел
Статистика
Эксперименты
Ведение журналов инфраструктуры
Производительность
Другие варианты
способствовать
Способствовать
Руководство для писателя
Написание загрузчика
Написание плагина
Шаблоны плагинов
Процесс выпуска
Отладка
Хартия
Ожидания участников
Политика модерации
Политика ИИ
Обзор системы управления
Рабочие группы
гиды
Гиды
Начиная
Управление активами
Управление выводом
Разработка
Разделение кода
Кэширование
Библиотеки для создания контента
Переменные окружающей среды
Производительность сборки
Политики безопасности контента
Развитие - Бродяга
Управление зависимостями
Установка
Замена модуля в горячем состоянии
Встряхивание деревьев
Производство
Ленивая загрузка
Модули ECMAScript
Мерцание
Машинопись
Веб-воркеры
Прогрессивное веб-приложение
Общественная тропа
Интеграции
Модули активов
Предварительный вход
Экспорт посылок
погрузчики
Погрузчики
babel-loader
кофе-загрузчик
экспорт-загрузчик
expose-loader
html-loader
импорт-загрузчик
загрузчик заметок
загрузчик потоков
css-loader
малогрузовый
postcss-loader
sass-loader
загрузчик стилей
загрузчик стилуса
мигрировать
Мигрировать
Переход с версии 4 на версию 5
Переход с версии 3 на версию 4
Переход с v1 на v2 или v3
плагины
Плагины
ChunksWebpackPlugin
HtmlWebpackPlugin
SvgChunkWebpackPlugin
AutomaticPrefetchPlugin
BannerPlugin
ContextExclusionPlugin
ContextReplacementPlugin
DefinePlugin
DllPlugin
EnvironmentPlugin
EvalSourceMapDevToolPlugin
HashedModuleIdsPlugin
HotModuleReplacementPlugin
IgnorePlugin
Внутренние плагины webpack
LimitChunkCountPlugin
ManifestPlugin
MinChunkSizePlugin
ModuleConcatenationPlugin
ModuleFederationPlugin
NoEmitOnErrorsPlugin
NormalModuleReplacementPlugin
PrefetchPlugin
Плагин профилирования
ProgressPlugin
ProvidePlugin
SourceMapDevToolPlugin
SplitChunksPlugin
VirtualUrlPlugin
WatchIgnorePlugin
CompressionWebpackPlugin
CopyWebpackPlugin
CssMinimizerWebpackPlugin
EslintWebpackPlugin
HtmlMinimizerWebpackPlugin
ImageMinimizerWebpackPlugin
JsonMinimizerWebpackPlugin
MiniCssExtractPlugin
StylelintWebpackPlugin
TerserWebpackPlugin
Сравнение
Потрясающий вебпак
Руководство по брендингу
Глоссарий
Лицензия
комплект ваш
ресурсы
скрипты
Напишите свой код
src/index.js

Копия
import bar from "./bar.js";

bar();
src/bar.js

Копия
export default function bar() {
  //
}
Объединить это
Начните без файла конфигурации или укажите собственный файл webpack.config.js :

Копия
const path = require("node:path");

module.exports = {
  entry: "./src/index.js",
  output: {
    path: path.resolve(__dirname, "dist"),
    filename: "bundle.js",
  },
};
Предпочитаете видеоинструкцию? Без настройки.

страница.html

Копия
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    ...
  </head>
  <body>
    ...
    <script src="dist/bundle.js"></script>
  </body>
</html>
Затем выполните команду webpackв командной строке для создания файла bundle.js.

Здорово, правда? Давайте начнём!
Начните работу быстро в разделе «Руководства» или углубитесь в раздел «Концепции» для получения более подробной информации об основных понятиях webpack.

Поддержите команду
Благодаря вашим взносам, пожертвованиям и спонсорской поддержке webpack процветает. Ваши пожертвования напрямую поддерживают консультации, дальнейшее совершенствование и, что наиболее важно, отличную документацию и учебные материалы!

Укажите спонсоров по среднему ежемесячному объему спонсорской поддержки за последний год.

Последние спонсоры
Следующие лица/организации сделали свое первое пожертвование за последние 14 дней (количество ограничено 10 крупнейшими ).

Аватар Czech Casinos
Аватар пользователя TopKasynoOnline PL
Аватар биткоин-казино
Аватар пользователя Best Online Pokies
Аватар лучшего биткоин-казино
Аватар лучшего онлайн-казино
Аватар онлайн-казино Новой Зеландии
Аватар онлайн-казино
Аватар Бетона
Лучшие онлайн-слоты в австралийском варианте
Станьте спонсором
Платиновые ежемесячные спонсоры
Платиновыми ежемесячными спонсорами считаются те, кто в настоящее время ежемесячно жертвует webpack 2500 долларов или более .

Аватар AG Grid
Станьте спонсором
Золотые ежемесячные спонсоры
Золотыми ежемесячными спонсорами считаются те, кто в настоящее время ежемесячно жертвует webpack от 500 до 2500 долларов .

Станьте спонсором
Серебряные ежемесячные спонсоры
Серебряными ежемесячными спонсорами считаются те, кто в настоящее время ежемесячно жертвует webpack от 100 до 500 долларов .

c19.cl - аватар Mejores Casinos Online
Аватар Airbnb
Аватар Elastic
Turtlebet - аватар Неттикасинот
Образ Parimatch India
Аватар Бластапа
Аватар NonGamstopCasinos.net
аватар пользователя luotettavat suomalaiset nettikasinot
Аватар Casivo.se
Купить подписчиков в Instagram, аватар Twicsy
Buzzoid - Купить аватар для увеличения числа подписчиков в Instagram
Аватар сайта Uudetkasinot.com
Аватар SocialBoosting
аватар казино без шведской лицензии
Аватар Швейца в онлайн-казино Ausländische
minsta insättning Casino Utan Свенск аватар лицензии
Аватар сайта Playfortuneforfun.com
Аватар Guidebook.BetWinner
Аватар Google Summer of Code
Аватар Fortune Games
аватар казино trygge norske
Купить аватар для подписчиков в Instagram
Аватар AUCrazyVegas
Аватар казино Wolf Winner
Аватар короля Джонни
Аватар Appfolio
Аватар WonderProxy
Аватар Ноя
Releaf – аватар Medizinischer Cannabis Shop
Станьте спонсором
Бронзовые ежемесячные спонсоры
Бронзовые ежемесячные спонсоры — это те, кто в настоящее время ежемесячно жертвует webpack от 10 до 100 долларов .

Аватар фонда JavaScript
Аватар пользователя utländska Casino с логом insättning
Аватар Rspack
Купить аватар «Подписчики в Твиттере»
Аватар https://casinobonuslord.com/
Аватар Daman Game
Купите просмотры на YouTube под аватаром Buzzoid.
Аватар Parik24
Аватар Practice Ignition
Аватар Фамиода
Аватар пользователя Vedonlyontiyhtiot.com
Аватар RelativeCI
аватар casinorevisor.com
Аватар GitBook
Аватар https://www.vso.org.uk/
аватар https://casinonotongamstop.uk/
Аватар Троллишли
Аватар BDG Win
Аватар Daman Game
Окей, аватар победы
Аватар iDealeCasinos
Аватар SoftOrbits
Аватар SidesMedia
Аватар Icons8
Аватар современного казначейства
Famety - Купить аватар для увеличения числа подписчиков в Instagram
Купить аватар YouTube Views
Аватар Slots City
Аватар казино Nove
аватар https://nogamstopcasinos.uk/
Аватар британских казино, не входящих в программу Gamstop.
Аватар игры Tiranga Game
Пройдите мой тест Praxis за меня - NoNEedToStudy.com Репетиторы по Praxis
Аватар для онлайн-казино Zonder Registratie
Аватар онлайн-казино iDEAL
Аватар 0+X
Аватар от Stiltsoft
Аватар пользователя DontPayFull
Аватар пользователя Social Followers
Аватар Frontend Masters
Аватар TestMu AI (ранее LambdaTest)
Аватар Mesh Payments
Аватар Barbados Bingo
Аватар Абеда Элезза
Аватар UpGrow
Купить подписчиков в Instagram, аватар MIXX
Купите подписчиков в Instagram, используя аватар SocialWick.
Аватар Fun88 Thailand
Аватар Fun88 Vietnam
Аватар от Daman Games
Аватар Affiliate.fm
Аватар игры Tiranga Game
Аватар Fun88
Аватар Чудово
Аватар сайта Kredittkorto.no
казино утан свенск аватар лицензии
Аватар Медиа-Мистера
Аватар Jspreadsheet
Аватар Тубиди
Аватар казино Magyar
Аватар Snaptik
Аватар Daman Game
Аватар онлайн-казино Buitenlandse
Аватар BDG Game
Аватар Kasino.page
казино утан свенск лицензии 10 евро аватар
утландское казино аватар 10 евро
Аватар Basant Club
Аватар Czech Casinos
Аватар пользователя TopKasynoOnline PL
Аватар Automatio AI
Аватар TaopaiC Tao
Аватар компании Waiterio LLC
Аватар Casinofox.se
Аватар Позита
Аватар Raider.IO
Аватар Extremely Heavy
Аватар NFI Cuatro
Люк Ян, аватар 顏浚原
Правильный аватар казино
Аватар компании MFB Technologies
Аватар Метори
Аватар онлайн-казино Австралии
Аватар Fast.Bet в Австралии
Аватар Материи
Аватар Greece Casinos
Аватар из Gokken Online
аватар М. С.
Аватар сайта ставок
Аватар казино Португалии
Аватар онлайн-казино Deutschland
Аватар Fast.bet Финляндии
Аватар казино RoboCat
Станьте спонсором
Спонсоры
Ниже представлены лица, внесшие различные суммы денег в поддержку webpack. Каждая мелочь имеет значение, и мы ценим даже самые небольшие пожертвования. В этом списке представлены 100 случайно выбранных спонсоров:

Аватар компании CasinoTest Ltd.
Аватар Пистолоказино
Аватар Инкогнито
Аватар Бенто (обратная ссылка)
Аватар Джони
Аватар BonusetuCom
Аватар Say Yup
Аватар Паркера Бонда
аватар беттинг онлайн казино
Аватар Владимира Старкова
Аватар Лайнаневоса
Аватар Вегаса
Аватар Бэтча
Аватар Дэвида Анга
Аватар Тиары Родни
Аватар VanguardNGR Франции
Аватар Intevation
Аватар Андреса Альвы
Аватар для Игровые автоматы
Аватар Аркирахи
Аватар Нгуен Чыонг Суана
Аватар Jackpot Rabbit Social Casino
Аватар Майкла Лафри
Аватар видеокассеты VHS в DVD
Аватар Оуэна Бакли
Аватар EscortA.com
Купить аватар Google Reviews
Аватар казино без верификации
Казино с быстрыми выплатами: аватар Канады
Аватар Романа Назаренко
Аватар Monarch Air Group
Аватар Мистера 7
Аватар Socialfollowers.io
Аватар Betking на YouTube
Аватар австралийских казино
Аватар Эрика Хендерсона
Аватар Holion ApS
Аватар Open Source Collective
Автор аватара — Заим.
аватар Яакаито
Аватар Эрики Свенссон
Аватар сайта www.interviewpal.com
MagicUGC – аватар лучшего AI UGC Video Generator
Аватар сайта Forexbrokerz.com
Аватар Райана Таллмаджа
Аватар пользователя Lainojen-yhdistäminen
Аватар Driven Coffee Roasters
Аватар Iranshartbandi.com
Аватар Reach Digital
Аватар Гэвина Могана
Аватар Nikotiinipussit.com
Аватар Булана
Аватар Clean Green Compare
Аватар Джереми Тайса
Аватар Нордиклендера
Аватар сайта buzzvoice.com
Аватар Скотта Вольфа
Аватар Ивана Лагуновского
Аватар Фьорда Финанса
Аватар Роберта Найта
Аватар Ника Дандакиса
Аватар OurCoordinates
Аватар GraphCommerce
Аватар Тревора Ричардсона
Аватар Content Camel
Аватар Y8
Аватар Дьюри Лайоша
Аватар стандартного резюме
Аватар https://betking.com.ua/games/all-slots/
Аватар Лотто Тулоксета
Аватарка для Украинского онлайн казино
Аватар компании Linden Photonics
Аватар JDLT
аватар techzjc
Аватар Tescort.com
Аватар Bonuskoodit
Купить подписчиков в Твиттере. Посетите аватар TweSocial.
Аватар Nopeustesti
Бонус: аватар Koodit
Аватар Казино Бонуси
Аватар CEOBuySell
Аватар Pika-kasinot.com
Аватар BuySocialMediaMarketing
Аватар ДеКонтрабаса
Новые сайты казино в Великобритании (2025) Аватар Help Direct
аватар ingatbola88
аватар Самиуллы Станикзая
Аватар Стратегизатора
Аватар казино Swiper
Купите X (Twitter) подписчиков у аватара Bulkoid.
Аватар Trash Nothing
Аватар BuyTikTokFollowers.co
Аватар IT-Manuals
аватар maltidsbarometeret
Аватар Кореллия
Аватар, полученный подбрасыванием монеты.
Аватар для Игровые автоматы
аватар анонима
Аватар Джонаса Фроста
Аватар Криса Ниенхейса
Станьте спонсором
Логотип фонда OpenJS
Авторские права принадлежат OpenJS Foundation и участникам проекта webpack. Все права защищены. OpenJS Foundation имеет зарегистрированные товарные знаки и использует товарные знаки. Список товарных знаков OpenJS Foundation можно найти в нашей Политике в отношении товарных знаков и Списке товарных знаков . Товарные знаки и логотипы, не указанные в списке товарных знаков OpenJS Foundation, являются товарными знаками™ или зарегистрированными® товарными знаками соответствующих владельцев. Их использование не подразумевает какой-либо связи с ними или одобрения с их стороны.

Фонд OpenJS | Условия использования | Политика конфиденциальности | Устав | Кодекс поведения | Политика в отношении товарных знаков | Список товарных знаков | Политика использования файлов cookie

Начать
Сравнение
политика конфиденциальности
Магазин сувениров
Потрясающий вебпак
Глоссарий
Брендинг
Discord
Список изменений
Лицензия Creative CommonsЛицензия Creative Commons
