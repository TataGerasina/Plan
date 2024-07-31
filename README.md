# План тестирования возможности записаться на обучение профессии «Инженер по тестированию»

### Изучим сайт заказчика веб-сайт Нетологии и определим количество возможных сценариев действий пользователя для попадания на форму записи.

## Попасть на форму записи можно со страницы профессии двумя способами: 
- пролистать всю страницу профессии до формы записи,
- нажатием кнопки «Записаться» на странице профессии. (данные шаги применимы к каждому сценарию действий 9 рассмотренных ниже пользователей)

# 1. Перечень автоматизируемых сценариев: тестировать лучше в разных классах навигацию и заполнение заявки с персональными данными. Так же необходимо учесть, вошел ли пользователь в аккаунт, тогда у него возможно есть свой курс и он может оказаться на странице профессии «инженер по тестированию» через всплывающую рекламу или кнопку «персональная скидка на второй курс», нажать кнопку «Выбрать курс» и нажать кнопку «Записаться» - вероятно вводить личные данные не будет необходимости и авторизованный пользователь сразу получит уведомление об успешной записи на курс.

**По навигации**
# Попасть на страницу профессии с главной страницы сайта можно двумя способами:
**через кнопку «Каталог курсов» в верхней части страницы**
[![image.png](https://i.postimg.cc/43r1WF6h/image.png)](https://postimg.cc/B8BD6pwq)

### Сценарий действий пользователя 1:

- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- заполняем поле формы «Какой курс вам нужен?» необходимым названием «инженер по тестированию»;
- нажимаем на кнопку «найти курс»;
- нажать на карточку «инженер по тестированию» - оказаться на странице с формой заявки на обучение; 

### Сценарий действий пользователя 2:
- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- заполнение поля формы «Какой курс вам нужен?» необходимым названием «инженер по тестированию»; 
- нажимаем на найденный курс «инженер по тестированию» в специальном окне-подсказке— переходим на страницу профессии;

#### (В аналогичном сценарии необходимо проверить: что происходит при нажатии на новое поле «Все курсы по запросу «инженер по тестированию(1)»» - страница «Все курсы» обновляется, количество профессий на странице не меняется, остаётся 232 профессии для выбора! Переход на искомую страницу происходит только после нажатия кнопки «найти курс». Уточнить у руководителей баг или так и должно быть)

### Сценарий действий пользователя 3:

- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- заполняем поле формы «Какой курс вам нужен?» названием «инженер»; 
- нажимаем на кнопку «найти курс»; 
- листаем страницу вниз нажимаем на карточку «инженер по тестированию» - оказываемся на странице с формой заявки на обучение; 
(Проверить что происходит при нажатии на новое поле Все курсы по запросу «инженер» (7) — ничего).

### Сценарий действий пользователя 4:

- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- нажимаем на значок «Все курсы»;
- листаем страницу вниз и находим страницу профессии «Инженер по тестированию», переходим на неё с помощью нажатия на поле с профессией;

### Сценарий действий пользователя 5:

- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- нажимаем на значок «Все курсы»;
- выбираем в фильтрах Платное, Диплом о ПП, Специалистам, ставим галочки; 
- листаем профессии вниз — 15 карточка будет «Инженер по тестированию» - нажимаем, переходим на искомую страницу;

### Сценарий действий пользователя 6:

- переходим на страницу <https://netology.ru/>;
- нажимаем на кнопку «Каталог курсов»;
- нажимаем на значок «Все курсы»;
- выбираем и нажимаем на значок «Программирование» — листаем профессии вниз —8 карточка будет «Инженер по тестированию» - нажимаем, переходим на искомую страницу.

**через Иконку «Програмирование» в разделе «Направления обучения» - нажимаем (количество курсов 44)**
[![image.png](https://i.postimg.cc/bNBS0SHZ/image.png)](https://postimg.cc/1fDzstdS)

### Сценарий действий пользователя 1:

- переходим на страницу <https://netology.ru/>;
- нажимаем на иконку-кнопку «Программирование» в разделе «Направления обучения»;
- листаем вниз до «Инженер по тестированию», нажимаем и оказываемся на странице профессии;


### Сценарий действий пользователя 2:

- переходим на страницу <https://netology.ru/>;
- нажимаем на иконку-кнопку «Программирование» в разделе «Направления обучения»;
- с помощью строки поиска «Какой вам нужен курс», вводим название курса и нажимаем кнопку «найти курс»;

### Сценарий действий пользователя 3:

- переходим на страницу <https://netology.ru/>;
- нажимаем на иконку-кнопку «Программирование» в разделе «Направления обучения»;
- с помощью фильтра Платное, Диплом о ПП, Новичкам, Тестирование ПО.

## После каждого выше описанного положительного сценария пользователь попадает на страницу профессии и ему необходимо 
**заполнить форму заявки на обучение**.

**Позитивный сценарий тестирования полей формы**
##### все поля заполнены валидными данными, форма заявки отправляется и уведомление об успешной отправки отображается.

1. Заполнить Имя, реальное по паспорту: Мария
2. Ввести телефон:+7 900 000 00 00
3. Заполнить электронную почту: Masha@gmail.com
4. Нажать на кнопку «Записаться»
5. Получить уведомление об успехе «Ваша заявка успешно отправлена!»

**Негативный сценарий тестирования полей формы**

1. оставляем пустыми значения полей и нажимаем кнопку «Записаться». 

##### Ожидаем, что форма не отправляется, поля подсвечиваются красным и/или появляются подсказки «введите имя по паспорту», «телефон должен состоять только из цифр», «электронная почта должна содержать @»,
##### уведомление об отправке не приходит или приходит сообщение «Ваша заявка не может быть отправлена. Пожалуйста, заполните верно свои данные.»

##### В автотестах необходимо проверить поля Имя, Телефон, Эл.почта (если есть другие поля или галочка-согласие на обработку персональных данных/рассылку о новых курсах или акциях, то их тоже).

##### Ниже предлагаю варианты проверок по каждому полю. При написании тестов необходимо комбинировать данные проверки по всем полям, так же можно некоторые поля заполнять валидными данными, проверяя отправку формы.

**Проверяем поле Имя**
1. вводим имя на иностранном языке(«Albert», «Apple»),
2. вводим вместо имени слово «Петрушка», большими буквами через Caps Lock (DONNALD, ТАНЯ), 
3. двойное имя через дефис(Анна-Мария)
4. вводим набор буквенных символов с клавиатуры по порядку слева направо сверху вниз «йцукенгшщзхъфывапролджэячсмитьбю» - определяем максимальную границу, пока не выдаст ошибку,
5. вводим имя из 2 букв «Ия»
6. вводим спец символы или иероглиф
7. перемешаем буквы с цифрами: «Ваня1Иванов», «Иван13», «7Мира»
8. ввести вместо имени одну букву латинскую «А»

**Проверяем поле Телефон:**
### +7 900 - меньше символов в номер телефона
### +7ячс — ввести буквы в телефон
### +712345678912345678 — больше 11 цифровых символов
### +7900...__09 — ввести с точками, пробелами номер телефона

**Проверяем поле Эл. почта:**
### арбуз@непомню.ru
### @@@@stydent.ru
### 12345@gmail.com

# 2. Перечень используемых инструментов с обоснованием выбора.
## *IDEA Community Edition удобна для написания и прогона тестов
## *Java: OpenJDK 11 язык написания тестов
## зависимости Junit 5, Maven, Selenide, Lombok с библиотеками
# GutHub для работы в команде и возможности завести баг-репорты
# Allure для отчетности

# 3. Перечень необходимых разрешений, данных и доступов:
1. Разрешение на тестирование и автоматизацию,
2. тестовые данные, 
3. доступ к базе данных, 
4. тестовый стенд для прогона тестов.

# 4. Перечень и описание возможных рисков при автоматизации: можно уронить сайт, сорвать сроки, может потребоваться помощь разработчиков.

# 5. Перечень необходимых специалистов для автоматизации: специалист по автоматизированному тестированию; разработчик, если к кнопкам, иконкам, полям не прописаны логи, необходимые для автоматизации тестов

# 6. Интервальная оценка с учётом рисков в часах: несколько дней нужно закладывать для начинающего специалиста (мне вероятно потребуется 5дней*8 часов = 40 часов).