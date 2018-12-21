---
## VI. Структуры данных. Работа с файлами
---
### Теоретическая часть

**1. Работа с файлами в java. Сериализация:**  
+ [Потоки ввода-вывода](https://metanit.com/java/tutorial/6.1.php)  **(\*\*\*\*)**
+ [Закрытие потоков](https://metanit.com/java/tutorial/6.2.php)  **(\*\*\*\*)**
+ [Чтение и запись файлов. FileInputStream и FileOutputStream](https://metanit.com/java/tutorial/6.3.php)  **(\*\*\*\*)**
+ [Классы ByteArrayInputStream и ByteArrayOutputStream](https://metanit.com/java/tutorial/6.4.php)  **(\*\*)**
+ [Буферизуемые потоки. Классы BufferedInputStream и BufferedOuputStream](https://metanit.com/java/tutorial/6.5.php)  **(\*\*\*\*)**
+ [Чтение и запись текстовых файлов. FileReader и FileWriter](https://metanit.com/java/tutorial/6.8.php)  **(\*\*)**
+ [Буферизируемые символьные потоки. BufferedReader и BufferedWriter](https://metanit.com/java/tutorial/6.9.php)  **(\*\*)**
+ [Сериализация объектов](https://metanit.com/java/tutorial/6.10.php)  **(\*\*)**
+ [Класс File. Работа с файлами и каталогами](https://metanit.com/java/tutorial/6.11.php)  **(\*\*\*\*)**
+ [Работа с ZIP-архивами](https://metanit.com/java/tutorial/6.12.php)  **(\*\*)**

**2. JSON:**
+ [Понятие](https://ru.wikipedia.org/wiki/JSON)  **(\*\*\*\*)**
+ [Парсинг в Android](http://java-help.ru/android-json/)  **(\*\*\*)**
+ [Gson](https://habrahabr.ru/company/naumen/blog/228279/) **(\*\*\*\*)**

**3. Сохранение данных в файловую систему Android:**  
+ [SharedPreferences](https://developer.android.com/training/basics/data-storage/shared-preferences.html?hl=ru#GetSharedPreferences) **(\*\*\*\*)**
+ [Настройки через Preferences](https://developer.android.com/guide/topics/ui/settings.html?hl=ru) **(\*\*)**
+ [Android data storage](https://developer.android.com/training/basics/data-storage/files.html) **(\*\*\*\*)**
+ [FileProvider](https://developer.android.com/reference/android/support/v4/content/FileProvider.html) **(\*\*\*)**

**3. Работа с датой и временем:**  
+ [Date, Calendar](http://developer.alexanderklimov.ru/android/java/date.php) **(\*\*\*\*)**
+ [Date в Java 8](http://www.baeldung.com/java-8-date-time-intro) **(\*\*\*\*)**
+ [Работа со временем в java ](https://habrahabr.ru/post/274811/) **(\*\*)**

### Практическое задание
Работа должна производится в созданном ранее проекте.

Все изменения должны быть закоммичены, а названия коммитов должны коротко и исчерпывающе описывать содержащие изменения. Каждый коммит должен быть рабочим, отправка некомпилирующегося кода недопустима. Для работы над этим заданием необходимо переключится на ветку `data_structures` и все изменения пушить в нее. После завершения работы над задачей в gitlab необходимо создать merge request в ветку `develop`.
Код должен быть читабельным и написан согласно code-style. Верстка экранов должна быть выполнена по принципу pixel-perfect.

1. Создать task в PS с заголовком "VI. Структуры данных" и взять ее в работу.
2. Подключить к проекту [ThreeTenABP](https://github.com/JakeWharton/ThreeTenABP). Все операции с датой и временем должны быть реализованы через классы данной библиотеки.
3. Сверстать экран "Благотворительных событий" согласно [макету](https://zpl.io/brkm3we). Переход на этот экран осуществляется при выборе любой категории на экране "Категории помощи".
4. Сверстать экран "Детальное описание события" согласно [макету](https://zpl.io/adA93Z5). Переход на этот экран осуществляется при выборе любого события из списка, данный экран должен получить информацию о том, какое событие было выбрано на предыдущем шаге.
5. Необходимо создать два json'а. Содержащих в себе массивы категорий и благотворительных событий. Информация об объектах должна быть достаточной для формирования отображений на экранах, а также для корректного разделения по категориям помощи. Каждый объект должен обладать уникальным (среди объектов своего типа) идентификатором. Проверить корректность созданных json-ов через [online-parser](http://json.parser.online.fr/). Записать их в 2 файла и поместить в папку assets проекта.
6. Необходимо создать сущности соответствующие понятиям Категория и Событие.
7. Создать сервис, который будет читать созданные json из файлов, парсить их и преобразовывать в массивы.
8. Наполнить экраны полученными данными. В сервисе учесть возможность фильтрации по категориям.
9. Завершить task в PS и залогировать затраченное время
