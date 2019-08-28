# MURD
*Программа-парсер СМИ разработана на языке Python 3.7 с использованием библиотек PyQt5, BeautifulSoup4, docx, urllib.

Создана для ведения мониторинговой базы данных СМИ по частному заказу. Работа программы подразумевала автоматический парсинг следующей информации по введенной вручную ссылке:
- Интернет-издание
- Дата создания статьи
- Название статьи
- Текст статьи
- Метки статьи

После парсинга программа использовалась для корректировки полученной информации, добавления пользовательских данных и создания SQL-инжектора, готового к последующей загрузке в БД. Автоматическая загрузка в БД заказчику не требовалась. 
Помимо этого, программа создает .docx файл с ID из инжектора, именем статьи, датой, названием и текстом статьи для последующей аналитики. 
У программы есть функция перехода в ручной режим, в котором функция парсинга заблокирована (актуально в случае невозможности парсинга страницы по какой-либо причине, включая бан пользователя).

Стандартные средства отлова ботов не блокируют работу программы.
