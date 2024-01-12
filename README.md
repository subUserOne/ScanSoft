<h1>SCAN soft</h1>

<img src="img/Screenshot_20240111-233940.png" width=30%><img src="img/Screenshot_20240111-180252.png" width=30%><img src="img/Screenshot_20240111-180300.png" width=30%>

<h2>Назначение</h2>
<p>Приложение позволяет использовать мобильный телефон как терминал сбора данных (ТСД).<br>
  
Доступны два режима работы:
<li>offline режим (локальная база номенклатуры)</li>
<li>online режим (подключение к серверу 1С)</li>
</p>
<p>
В offline режиме приложение использует локальную базу данных для хранения справочника номенклатуры.<br>
Сканирование маркировки товаров выполняет поиск по локальной базе и предлагает добавить номенклатуру.<br>
В карточке номенклатуры можно ввести данные по товару, сделать и прикрепить фотографию.<br>
  <img src="img/Screenshot_20240112-181207.png" width=30%><br>
Последующее сканирование маркировки сможет найти товар в базе данных и добавить его в корзину.
  
</p>
<br>

<h2>Настройка работы online режима</h2>
<p>
  До начала работы с приложением следует установить расширение одной из типовых конфигураций: <a href="https://github.com/subUserOne/ScanSoft/tree/main/Extensions" target="_blank">ERP, Торговля, Розница, Комплексная автоматизация</a>
</p>
<p>Для работы расширения понадобится установить web server и опубликовать сервис расширения с настройками:
  <img src="img/public.png" width=50%><br>
Имя указанное в публикации должно быть в настройке "Адрес подключения сервера"<br>
<b>http://&lt;XXX.XXX.XXX.XXX&gt;/&lt;baseName&gt;/hs/mi</b><br>
где &lt;XXX.XXX.XXX.XXX&gt; - адрес сервера 1С, локальный или в интернет.<br>
  &lt;baseName&gt; - имя публикации
</p>
<p>
Далее, на каждый подключаемый терминал необходимо создать собственного пользователя в 1С и авторизоваться на ТСД с помощью логина и пароля.
</p>
<br><br>

<h2>Работа приложения и сценарии использования</h2>
<p>
  Сканирование маркировки осуществляется с помощью аппаратных кнопок громкости или нажатием на экран.
  В обоих сценариях работы (offline/online) по данным маркировки выполняется поиск номенклатуры в базе данных, после чего появляется возможность добавить товар в корзину.<br><br>
  <img src="img/Screenshot_20240112-011509.png" width=30%><br><br>
  Содержимое корзины можно просмотреть и отредактировать нажав на изображение корзины.<br><br>
  <img src="img/Screenshot_20240112-011532.png" width=30%><br>
</p>

<p>
По кнопке записать произойдет передача данных ТСД на сервер 1С.<br>
Просмотреть корзину в разрезе терминалов можно в регистре сведений<br><br>
<img src="img/basket.png" width=100%><br>

Возможны любые сценарии использования данных, такие как:
<li>Создание и наполнение документов</li>
<li>Выполнение инвентаризации</li>
<li>Печать чеков ККМ</li>
<li>Формирвание отчетов и т.д.</li>
  
</p>
