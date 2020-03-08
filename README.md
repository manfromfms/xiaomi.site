<!DOCTYPE html>

<html lang="ru">
    <head>
        <meta charset="utf-8">
        <title>Сайт про чтото</title>
        </head>
    <body>
    <script src="javascript.js" defer>
    let cost = [2490, 2790, 2790, 3890, 3890, 3640, 4790, 4790, 6490, 7250, 9238, 7950, 11990, 7390];
let names = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14"];

function filter() {
    let minimum = document.getElementById("min").value;
    let maximum = document.getElementById("max").value;
    
    for (let i = 0; i < cost.length; i++) {
        if (cost[i]>=minimum && cost[i]<=maximum) {
            document.getElementById(names[i]).style = "display: table-row;";
        } else {
            document.getElementById(names[i]).style = "display: none;";
        }
    }
}</script>

<style>@media (min-width: 961px) {
    
    .start {
    background-image: url(stuff/Background/1479280611_Xiaomi-.jpg);
    color: black;
    border-radius: 10px;
    border: 4px solid;
    border-color: black;
}

html {
    background-image: url(stuff/Background/1200px-Xiaomi_logo.svg.png);
    background-size: 100%;
}

h1 {
    margin-left: 5px;
    padding-bottom: -10px;
    margin-bottom: 4px;
    background-color: rgba(255,255,255,0.5);
}

p {
    margin: 0px 10px 0px 10px;
}


.tablet {
    background-color: white;
    margin-top: 10px;
    border-radius: 10px;
    border: 4px solid;
    border-color: black;
}

.redmi {
    float: left;
}

td {
    border: solid;
    padding: 10px;
    text-align: center;
}

a {
    text-decoration: none;
}

.no_info {
    color: red;
    text-decoration:line-through;
}

.description {
    background-color: rgba(255,255,255,0.5);
    border: 4px solid;
    border-radius: 10px;
    border-color: black;
    margin-top: 10px;
}

.desc {
    margin: 10px;
}

tr {
    margin: 10px;
    width: 50%;
}

.header-p {
    width: 500px;
    background-color: rgba(255,255,255,0.5);
}

.menu {
    width: 200px;
    background-color: rgba(255,255,255,0.5);
    margin: 0;
}



.head-info {
    display: flex;
    width: 100%;
}

.mi {
    border: 3px solid;
    border-color: red;
    border-radius: 14px;
}

.head-img {
    border: 4px solid;
    border-color: black;
    border-radius: 15px;
    background: linear-gradient(to right, red , blue);
    margin: 20px;
}

.middle {
    margin-left: 25%;
    margin-right: 25%;
}

table {
    width: 100%;
}

.filter {
    display: flex;
}
}

@media (max-width: 960px) {
    
.start {
background-image: url(stuff/Background/1479280611_Xiaomi-.jpg);
color: black;
border-radius: 10px;
border: 4px solid;
border-color: black;
}

html {
    background-image: url(stuff/Background/1200px-Xiaomi_logo.svg.png);
    background-size: 100%;
}

h1 {
    margin-left: 5px;
    padding-bottom: -10px;
    margin-bottom: 4px;
    background-color: rgba(255,255,255,0.5);
}

p {
    margin: 0px 10px 0px 10px;
}


.tablet {
    background-color: white;
    margin-top: 10px;
    border-radius: 10px;
    border: 4px solid;
    border-color: black;
}

.redmi {
    float: left;
}

td {
    border: solid;
    padding: 10px;
    text-align: center;
}

a {
    text-decoration: none;
}

.no_info {
    color: red;
    text-decoration:line-through;
}

.description {
    background-color: rgba(255,255,255,0.5);
    border: 4px solid;
    border-radius: 10px;
    border-color: black;
    margin-top: 10px;
}

.desc {
    margin: 10px;
}

tr {
    margin: 10px;
    width: 50%;
}

.header-p {
    width: 500px;
    background-color: rgba(255,255,255,0.5);
}

.menu {
    width: 200px;
    background-color: rgba(255,255,255,0.5);
    margin: 0;
}



.head-info {
    display: flex;
    width: 100%;
}

.mi {
    border: 3px solid;
    border-color: red;
    border-radius: 14px;
}

.head-img {
    border: 4px solid;
    border-color: black;
    border-radius: 15px;
    background: linear-gradient(to right, red , blue);
    margin: 20px;
}

table {
    width: 100%;
}

.filter {
    display: flex;
}
}
.footer {
    margin-top: 10px;
    border: 4px solid;
    border-color: black;
    border-radius: 10px;
    padding: 10px;
    background-color: blue;
    color: white;
}

.footer-back {
    color: white;
}
</style>
    <div class="middle">
        <div class="start">
            <h1>Таблица сравнения всех смартфонов Xiaomi<br>(сайт находится в разработке)</h1>
            <div class="head-info">
                <p class="header-p">
                    Чем славится компания  Xiaomi? Многие ответят что дешовыми и одновременно качественными смартфонами, и будут правы. И да, если сравнить смартфоны Xiaomi с конкурентами, то победитель будет очевиден. Давайте рассмотрим все сматфоны Xiaomi и выявим лучший выгодный и доступный смартфон.
                </p>
                <ol class="menu" id="menu">
                <li><a href="#Redmi-top" title="Посмотреть телефоны xiaomi redmi">Redmi</a></li>
                </ol>            
            </div>
        </div>
        <div class="tablet" id="Redmi-top">
            <h1>Redmi</h1>
            <p>
                Начнём с бюджетников компании Xiaomi - модели redmi.
            </p><br>
            <div class="filter">
                Установить фильтр: цена <input type="text" id="min" placeholder="min cost" value="0">-
                <input type="text" id="max" placeholder="max cost" value="100000">
                <button id="filter" onclick="filter();">Применить фильтр</button>
            </div><br>
            <table>
                <tr>
                    <td>Название</td>
                    <td>Фоточка</td>
                    <td>Небольшое описание</td>
                </tr>
                
                <tr id="1">
                    <td><a href="#Redmi" title="Ссылка отсутствует">Redmi (2490 р.)</a></td>
                    <td><img src="stuff/redmi/redmi.png" class="redmi" width="100px"></td>
                    <td class="no_info">Информация отсутствует</td>
                </tr>
                
                <tr id="2">
                    <td><a href="#Redmi-2">Redmi 2 (2790 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-2.jpg" width="100px"></td>
                    <td>Xiaomi подтвердила звание одного из самых популярных мировых производителей смартфонов, выпустив даже в самом нижнем сегменте настолько качественный продукт, что так и хочется сказать: «Я бы за него больше заплатил!»</td>
                </tr>
                
                <tr id="3">
                    <td><a href="#Redmi-2a">Redmi 2A (2790 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-2a.jpg" width="100px"></td>
                    <td>Устройство является практически полной копией модели Redmi 2S, который оценивается в $115. Естественно, отличие заключается в платформе.</td>
                </tr>
                
                <tr id="4">
                    <td><a href="#Redmi-3">Redmi 3 (3890 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-3.jpg" width="100px"></td>
                    <td>Даже для смартфона за 150 долларов Redmi 3 имеет отличную камеру, оболочку и производительность. </td>
                </tr>
                
                <tr id="5">
                    <td><a href="#Redmi-3-pro">Redmi 3 pro (3890 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-3-pro.jpg" width="100px"></td>
                    <td> Плюсы Redmi 3 Pro смело записываем: дизайн, компактность, плавность работы, очень уверенную автономность, хорошие камеры и звук в наушниках.</td>
                </tr>
                
                <tr id="6">
                    <td><a href="#Redmi-3s">Redmi 3S (3640 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-3s.jpg" width="100px"></td>
                    <td>Аппарат идеально ложится в руку, отличное олеофобное покрытие на стекле и приятный холод от металла на задней части.</td>
                </tr>
                
                <tr id="7">
                    <td><a href="#Redmi-4">Redmi 4 (4740 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-4.jpg" width="100px"></td>
                    <td>Сбалансированный смартфон, который можно было бы назвать идеальным, если бы не одно «но» — возможные мелкие баги в прошивке. В остальном с Xiaomi Redmi 4 пока не может конкурировать ни один крупный бренд.</td>
                </tr>
                
                <tr id="8">
                    <td><a href="#Redmi-4a">Redmi 4A (4790 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-4a.jpg" width="100px"></td>
                    <td>Внешний вид у гаджета от Xiaomi относительно примитивный, однако Redmi 4A не выглядит дешево: классическая форма корпуса, плавные очертания, минималистичный дизайн, аккуратное оформление. C обратной стороны есть две бороздки, они декоративные, поскольку корпус неразборный и бесшовный. Лицевая панель без закругления стекла типа 2.5D.</td>
                </tr>
                
                <tr id="9">
                    <td><a href="#Redmi-5">Redmi 5 (6490 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-5.jpg" width="100px"></td>
                    <td>Недорого, надёжно, а теперь ещё и широкоэкранно — нельзя просто взять и пройти мимо Xiaomi Redmi 5,</td>
                </tr>
                
                <tr id="10">
                    <td><a href="#Redmi-6">Redmi 6 (7250 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-6.jpg" width="100px"></td>
                    <td>Xiaomi Redmi 6 получился неоднозначным. Практически все характеристики хуже, чем у прошлогодней модели. Вместо металла в корпусе пластик, снизилась игровая производительность и общая скорость системы, упало время автономной работы.</td>
                </tr>
                
                <tr id="11">
                    <td><a href="#Redmi-6-pro">Redmi 6 pro (9238 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-6-pro.jpg" width="100px"></td>
                    <td>Это как Xiaomi Redmi 6a, нo с Mediatek и в пластике. При этом с двойной камерой и сканером отпечатков пальцев. Оригинальный аппарат. Возможно, лучший бюджетный смартфон — еще и фотографировать нормально умеет. Для своей цены, конечно.</td>
                </tr>
                
                <tr id="12">
                    <td><a href="#Redmi-6a">Redmi 6A (7950 р.)</a></td>
                    <td><img src="stuff/redmi/redmi-6a.jpg" width="100px"></td>
                    <td>Xiaomi обновила свой самый доступный смартфон — очень популярный в прошлом сезоне Xiaomi Redmi 5A. Ему на смену пришел новый бюджетный мобильный аппарат компании, Xiaomi Redmi 6A, и у него есть все шансы побить рекорд своего предшественника. По крайней мере, в категории «до $120» это одно из самых интересных предложений.</td>
                </tr>
                
                <tr id="13">
                    <td><a href="#Redmi-7">Redmi 7 (11990 p.)</a></td>
                    <td><img src="stuff/redmi/redmi-7.jpg" width="100px"></td>
                    <td>Redmi 7, безусловно, очень привлекателен своей ценой: в фирменном магазине Xiaomi за смартфон просят от 11,5 до 14 тысяч рублей в зависимости от конфигурации, а у иных продавцов эту модель можно приобрести и того дешевле.</td>
                </tr>
                
                <tr id="14">
                    <td><a href="#Redmi-7a">Redmi 7A (7390 p.)</a></td>
                    <td><img src="stuff/redmi/redmi-7a.jpg" width="100px"></td>
                    <td>Если ищите простой, недорогой смартфон — Redmi 7A однозначно стоит внимания.</td>
                </tr>
            </table>
        </div>
        
        <div class="description" id="Redmi-2">
            <div class="char">
                <h2>Redmi 2</h2>
                <p class="desc">Смартфон Xiaomi Redmi 2 совершенно не обременен каким-либо выразительным дизайном. Некрупный аппарат имеет невзрачный пластмассовый корпус, большую часть которого составляет пластиковое корытце, склеенное со стеклом передней панели. Никаких украшающих элементов или хотя бы бокового ободка здесь нет. Прямоугольный моноблочный корпус имеет практические прямые плоские грани и едва закругленные углы.</p>
                <ul>
                    <li>Экран: 4.7", IPS</li>
                    <li>Разрешение: 1280х720, 312 ppi</li>
                    <li>Процессор: Qualcomm Snapdragon 410 (4 ядра ARM Cortex-A53 @1,2 ГГц)</li>
                    <li>Флэш-память: 8/16 ГБ</li>
                    <li>Операционная система: Google Android 4.4</li>
                    <li>Аккумулятор: 2200 мА·ч</li>
                    <li>Камера: Tыльная (8 Мп; видео 1080p), фронтальная (2 Мп)</li>
                    <li>Габариты и вес: 134×67×9,4 мм, 132 г</li>
                </ul>
                
                <p>Размеры Xiaomi Redmi 2 практически минимальны. На сегодняшний день, пожалуй, трудно сыскать более миниатюрный смартфон такого же уровня. По размерам он оказывается нисколько не крупнее других аналогичных современных аппаратов с экраном 4,7 дюйма.</p>
            </div>
            <br>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-2a">
            <h2>Redmi 2A</h2>
            <p>Первые слухи о самом дешёвом смартфоне Xiaomi были о шестиядерной платформе с поддержкой LTE, дисплее HD и стоимости $65. В дальнейшем данные были скорректированы в сторону четырёхъядерной системы. Вскоре Xiaomi наконец-то представила данное устройство. Называлась новинка Redmi 2A и стоила 600 юаней, что соответствует примерно $95. Таким образом, никакого сверхдешёвого смартфона Xiaomi не выпустила и пока не собирается.</p>
            <ul>
                <li>Экран: 4.7", IPS</li>
                <li>Разрешение: 1280 х 720, 312 ppi</li>
                <li>Процессор: Qualcomm Snapdragon 410 (4 ядра ARM Cortex-A53 @1,2 ГГц)</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система: Google Android 4.4 с оболочкой MIUI6</li>
                <li>Аккумулятор: 2200 мА·ч</li>
                <li>Камера: Tыльная (8 Мп; видео 1080p), фронтальная (2 Мп)</li>
                <li>Габариты и вес: 134х67,2х9,4 мм, 132 г</li>
            </ul>
            <p>К слову купить Redmi 2A в начале продаж можно было за $80</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-3">
            <h2>Redmi 3</h2>
            <p>С недавних пор компания также начала подписывать прошивки уникальными ключами, а впоследствии и вовсе по умолчанию заблокировала загрузчик в своих смартфонах, из-за чего установить локализованное умельцами ПО стало достаточно сложно. Свою лепту вносят и нерадивые китайские продавцы предустанавливая либо частично локализованное ПО в котором исключена возможность обновлений «по воздуху», либо прошивку с тоннами вредоносных программ, которые сводят всю прелесть большого аккумулятора на нет. </p>
            <ul>
                <li>Экран: 5", IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: Snapdragon 616, 8 ядер Cortex-A53, 4 ядра работают на частоте 1.2 ГГц, а еще 4 на 1.5 ГГц</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система: MIUI v7 на основе Android 5.1 Lollipop</li>
                <li>Аккумулятор: 4000 мА·ч</li>
                <li>Камера: 13 МП с апертурой f/2.0, автофокус, светодиодная вспышка; фронтальная камера 5 МП (f/2.2), запись FullHD видео</li>
                <li>Габариты и вес: 139.3 x 69.6 x 8.5 мм, 144 г</li>
            </ul>
            <p>Сейчас смартфон можно приобрести в китайских интернет магазинах за 140-150 долларов со скидкой в 4-8% за счет использования какого-либо кешбек-сервиса.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-3-pro">
            <h2>Redmi 3 pro</h2>
            <ul>
                <li>Экран: 5", IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: Система на чипе Qualcomm Snapdragon 616 включает в себя восемь ядер Cortex-A53 и видеоядро Adreno 405.</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система: MIUI v7 на основе Android 5.1 Lollipop</li>
                <li>Аккумулятор: 4100 мА·ч</li>
                <li>Камера: Разрешение основной камеры составляет 13 мегапикселей. Сенсор с гибридным фазовым автофокусом прикрыт пятикомпонентным объективом с апертурой F2.0 и эквивалентным фокусным расстоянием равным примерно 30 мм., запись FullHD видео</li>
                <li>Габариты и вес: 139.3 x 69.6 x 8.5 мм, 144 г</li>
            </ul>
            <p>В плюсы Redmi 3 Pro смело записываем: дизайн, компактность, плавность работы, очень уверенную автономность, хорошие камеры и звук в наушниках. К минусам можно отнести зернистость экрана и низкую производительность в играх. Xiaomi обновила один из своих самых интересных смартфонов, но хочет за это 200 юаней ($30) сверху, при этом стоимость новинки сравнялась со стоимостью младшей модификации Redmi Note 3. Последний мощнее и имеет лучший экран, но хуже автономность, больше габариты и вес. Новинка проигрывает оригинальному Redmi 3 по соотношению цена/качество – очень важному для бюджетного телефона параметру. И все же Xiaomi Redmi 3 Pro – это один из лучших смартфонов от Xiaomi.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-3s">
            <h2>Redmi 3S</h2>
            <ul>
                <li>Экран: 5", IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: Qualcomm Snapdragon 430 1.4 Ггц 8 ядер ARM Cortex-A53</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система: Android v6, MIUI 7, (Marshmallow)</li>
                <li>Аккумулятор: 4100 мА·ч</li>
                <li>Камера: Фронтальная камера: 5 MP f/2.2 Основная камера: 13 MP f/2.0</li>
                <li>Габариты и вес: 139.3 x 69.6 x 8.5 мм, 144 г</li>
            </ul>
            <p>Скажу честно, качеством Xiaomi RedMi 3s можно восхищаться, очень много датчиков и все работает просто великолепно. Сканер отпечатка пальца — срабатывает моментально, производительности хватает даже для очень тяжелых игр, батарея — просто сказка, все это подано под соусом качественных фото и приправлено металлическим корпусом.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-4">
            <h2>Redmi 4</h2>
            <ul>
                <li>Экран: 5", IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: Qualcomm Snapdragon 625</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система: Android v6, MIUI 7, (Marshmallow)</li>
                <li>Аккумулятор: 4100 мА·ч</li>
                <li>Камера: Фронтальная камера: 5 MP f/2.2 Основная камера: 13 MP f/2.0</li>
                <li>Габариты и вес: 139.3 x 69.6 x 8.5 мм, 144 г</li>
            </ul>
            <p>Xiaomi Redmi 4 на сегодняшний день — самый честный смартфон. Он не накручивает цену за бренд, предлагает достаточную для большинства пользователей производительность, качественный дисплей и высокую автономность вкупе со стабильностью и предсказуемостью.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-4a">
            <h2>Redmi 4A</h2>
            <ul>
                <li>Экран: 5", IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: 4 ядра, Qualcomm Snapdragon 425 (MSM8917)</li>
                <li>Флэш-память: 8/16 ГБ</li>
                <li>Операционная система:  Google Android 6.0.1, MIUI 8.1.4.0</li>
                <li>Аккумулятор: 3120 мАч</li>
                <li>Камера: 13 МП (f=2.2) c автофокусом + 5 МП, вспышка</li>
                <li>Габариты и вес: 139 x 70 x 8.5 мм, 131 г</li>
            </ul>
            <p>Средняя стоимость Redmi 4A на китайских интернет-полках составляет около 7 000 рублей, можно найти чуть дешевле или дороже. В России официальная цена – 9 990 рублей, на 14 февраля была 8 600. На 1 000 рублей дороже есть Meizu M5 – такой же пластиковый, характеристики почти один в один, чуть шустрее процессор и есть сканер отпечатков пальцев. В этом же районе продается Lenovo Vibe P1m – слабенький процессор, но зато батарейка на 4000 мАч.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-5">
            <h2>Redmi 5</h2>
            <ul>
                <li>Экран: 5,7", TFT-IPS</li>
                <li>Разрешение: 1280 х 720</li>
                <li>Процессор: Qualcomm Snapdragon 450, 8х1,8 ГГц (Cortex-A53)</li>
                <li>Флэш-память: 2/3/4 ГБ</li>
                <li>Операционная система: Android 7.1.2</li>
                <li>Аккумулятор: 3300 мАч</li>
                <li>Камера: основная — 12 Мп (вспышка, автофокус, f/2,2), фронтальная — 5 Мп (вспышка, f/2,2)</li>
                <li>Габариты и вес: 151,8х72,8х7,7 мм, 157 г</li>
            </ul>
            <p>Смартфон Xiaomi Redmi 5 смело можно назвать одним из лучших доступных смартфонов для потребления контента. Компактный размер, отличный экран широкого формата 18:9, приятный звук в наушниках и через динамик, продолжительное время работы и достойный уровень производительности. Да, камеры тут средние по бюджетным меркам, но в остальном смартфон оставляет сугубо положительные впечатления.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
            
        <div class="description" id="Redmi-6">
            <h2>Redmi 6</h2>
            <ul>
                <li>Экран: 5,45’’, IPS</li>
                <li>Разрешение: 1440х720, 18:9, 295 ppi</li>
                <li>Процессор: Mediatek Helio P22, до 2,0 ГГц</li>
                <li>Флэш-память: 3/4 ГБ</li>
                <li>Операционная система: Android 8.1 Oreo</li>
                <li>Аккумулятор: 3000 мАч, несъёмный</li>
                <li>Камера: Основная камера: 12 Мп + 5 Мп, f/2.2 Фронтальная камера: 5 Мп</li>
                <li>Габариты и вес: 147,5х71,5х8,3 мм, 146 г</li>
            </ul>
            <p>Плюсы:большой объём встроенной памяти;быстрый сканер отпечатков;удобные жесты управления.Минусы:пластиковый корпус;нет Wi-Fi 5 ГГц и NFC;средняя автономность.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        
        <div class="description" id="Redmi-6-pro">
            <h2>Redmi 6 pro</h2>
            <ul>
                <li>Экран: 5,45’’, IPS</li>
                <li>Разрешение: 1440×720, 18:9, 295 ppi</li>
                <li>Процессор: Mediatek Helio A22 с видеоядром PowerVR Rogue GE8320</li>
                <li>Флэш-память: 3/4 ГБ</li>
                <li>Операционная система: Android 8.1 Oreo</li>
                <li>Аккумулятор: 3000 мАч, несъёмный</li>
                <li>Камера: Основная камера: 12 Мп + 5 Мп, f/2.2 Фронтальная камера: 5 Мп</li>
                <li>Габариты и вес: 147,5х71,5х8,3 мм, 146 г</li>
            </ul>
            <p>На момент написания сайта базовая модификация Redmi 6a с 2 Гб оперативной и 16 Гб постоянной памяти стоит $106 (7 тыс. руб.), версия 2/32 Гб — $115 (7600 руб.).В свою очередь, за Xiaomi Redmi 6 со сканером отпечатков пальцев и Helio P22 обойдется в $120 за 3/32 (7900 руб.) и $140 за 4/64 Гб (9200 руб.).Все это говорит о том, что металлический Redmi 5 пусть и относится к предыдущему поколению, все еще остается отличным приобретением.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        <div class="description" id="Redmi-6a">
            <h2>Redmi 6A</h2>
            <ul>
                <li>Экран: IPS 5,45″</li>
                <li>Разрешение: 1440×720, 18:9, 295 ppi</li>
                <li>Процессор: SoC MediaTek Helio A22, 4 ядра ARM Cortex-A53 @2,0 ГГц</li>
                <li>Флэш-память: 2 ГБ</li>
                <li>Операционная система: Android 8.1, MIUI</li>
                <li>Аккумулятор: 3000 мАч, несъёмный</li>
                <li>Камера: Основная камера 13 Мп, f/2,2, автофокус; видео 1080р Фронтальная камера 5 Мп, f/2,0, фикс. фокус</li>
                <li>Габариты и вес: 148×72×8,3 мм, 180 г</li>
            </ul>
            <p>Xiaomi Redmi 6A сейчас представлен в официальной российской рознице по цене от 7 тысяч рублей, что является крайне привлекательным вариантом, если сравнивать цены сертифицированных аппаратов. Более того, с 8 октября интернет-магазин TMall готов предложить младшую модификацию смартфона за 6 тысяч. Это один из самых доступных смартфонов производителя первого эшелона, коим Xiaomi безусловно является.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        
        <div class="description" id="Redmi-7">
            <h2>Redmi 7</h2>
            <ul>
                <li>Экран: IPS, 6,26″</li>
                <li>Разрешение: 1520×720 (19:9), 269 ppi</li>
                <li>Процессор: SoC Qualcomm Snapdragon 632, 8 ядер Kryo 260 @1,8 ГГц</li>
                <li>Флэш-память: 2 ГБ</li>
                <li>Операционная система: Android 9, MIUI 10</li>
                <li>Аккумулятор: 4000 мАч, несъёмный</li>
                <li>Основная камера 12 Мп (f/2,2) + 2 Мп (сенсор глубины), автофокус, видео 1080р (60 fps) Фронтальная камера 8 Мп, f/2,0</li>
                <li>Габариты и вес: 159×76×8,5 мм, 180 г</li>
            </ul>
            <p>При такой цене и учитывая более чем адекватные возможности аппаратной платформы, которая справляется даже с требовательными играми, а также выдающуюся автономность и отличные для бюджетника камеры, смартфон Redmi 7 просто обречен на успех.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        
        <div class="description" id="Redmi-7a">
            <h2>Redmi 7A</h2>
            <ul>
                <li>Экран: TFT-IPS, 5,45 дюйма″</li>
                <li>Разрешение: 720 × 1440 точек</li>
                <li>Процессор: SoC Qualcomm Snapdragon 439</li>
                <li>Флэш-память: 2 ГБ</li>
                <li>Операционная система: Android 9, MIUI 10</li>
                <li>Аккумулятор: 4000 мАч, несъёмный</li>
                <li>Основная камера: 13 Мп, f/2.2, HDR, запись видео 1080p 30fps; фронтальная камера 5 Мп;</li>
                <li>Габариты и вес: 146,3 × 70,4 × 9,5 мм, 165 г</li>
            </ul>
            <p>Бывают удачные примеры вроде этого Redmi 7A, где всё при нём, и телефон честно выполняет возложенные на него функции, отрабатывая свою скромную цену. Определённо это хит продаж всего 2019 и грядущего 2020 года, пока Redmi не покажет что-то взамен этой модели.</p>
            <div class="back">
                <a href="#menu">Вернуться в меню</a>
            </div>
        </div>
        
        <div class="footer">
            <p>Текст и информация были взяты из головы и некоторых сайтов:</p>
            <ol>
                <li>www.iphones.ru</li>
                <li>4pda.ru</li>
                <li>market.yandex.ru</li>
                <li>wikipedia.ru</li>
                <li>www.ixbt.com</li>
            </ol>
            <p>Выражаем им огромную благодарность</p>
        </div>
        <div class="footer-back">
            <a href="#menu">Вернуться в меню</a>
        </div>
    </div>
    </body>
</html>
