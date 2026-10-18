> Оформлено студенткою  
> групи КСМ-43б   
> Адаменко Є. В.  

<h1 align="center"> Лабораторна робота №5</h1>

## Завдання попередньої підготовки
### Завдання 1 - Прочитайте короткі теоретичні відомості до лабораторної роботи та зробіть невеликий словник базових англійських термінів з питань призначення команд та їх параметрів.
- Filesystem - структура каталогів Linux, яка має верхній рівень - кореневий каталог
- Root directory - верхній рівень файлової системи Linux, позначається символом `/`
- Directory - тип файлу, що використовується для зберігання інших файлів
- Home directory - унікальний каталог користувача, у якому він починає роботу, позначається символом `~`
- Parent directory - каталог на рівень вище поточного, позначається `..`
- Path - список каталогів, розділених символом `/`, "адреса" файлу у файловій системі
- Overwrite - замінити вміст наявного файлу
<br>
<br>

### Завданняя 2 - На базі розглянутого матеріалу дайте відповіді на наступні питання:
#### 2.1 Порівняйте файлові структури Windows-подібної та Linux-подібної системи.
##### У Windows верхній рівень структури каталогів називається My Computer, а у Linux - кореневий каталог `/`. Фізичні пристрої у Windows мають літери дисків, а у Linux літер немає - кожен пристрій доступний в одному з каталогів. Також у Linux все вважається файлами.
<br>

#### 2.2 Розкрийте поняття FHS. Як даний стандарт використовується в контексті файлових систем?
##### FHS (Filesystem Hierarchy Standard) - стандарт, на якому ґрунтуються загальноприйняті назви каталогів Linux. У файловій системі Linux поширені назви каталогів використовуються для типових функці. Наприклад, `/etc` - файли конфігурації системи, `/home` - домашні каталоги користувачів, `/var` - файли, що часто змінюються, як-от журнали. Багато дистрибутивів Linux дотримуються FHS, тому файли легко знайти в будь-якій FHS-сумісній системі Linux.
<br>

#### 2.3 Перерахуйте основні команди для роботи з файлами та каталогами в Linux: створення, переміщення, копіювання, видалення.

| Дія | Команда | 
|---|---|
| Створення порожнього файлу | `touch` | 
| Створення каталогу | `mkdir` | 
| Копіювання | `cp` | 
| Переміщення | `mv` | 
| Видалення файлів | `rm` | 
| Видалення каталогу з вмістом | `rm -r` |
| Видалення порожнього каталогу | `rmdir` |

<br>
<br>

### Завдання 4 - Пройдіть тестування у курсі NDG Linux Essentials за такими темами:
- Chapter 07 Exam
- Chapter 08 Exam
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/exams.png?raw=true)
<br>
<br>

## Хід роботи
### Завдання 1 - Початкова робота в CLI-режимі в Linux ОС сімейства Linux: запустіть віртуальну машину Ubuntu_PC 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/1.png?raw=true)
<br> 
<br>

### Завдання 2 - Опрацюйте всі приклади команд, що представлені у лабораторних роботах курсу NDG Linux Essentials - Lab 7: Navigating the Filesystem та Lab 8: Managing Files and Directories. Створіть таблицю для опису цих команд
| Команда | Опис | 
|---|---|
| pwd | Показує поточну робочу директорію | 
| echo $HOME | Виводить на екран шлях до домашнього каталогу користувача | 
| echo * | Виводить список усіх файлів поточного каталогу | 
| echo D* | Виводить усі файли, імена яких починаються з літери D | 
| echo *s | Виводить усі файли, імена яких закінчуються на s | 
| echo ?????? | Виводить файли, ім'я яких складається з кількості символів ? | 
| echo [DP]* | Виводить файли, ім'я яких починається з D та P | 
| echo [!DP]* | Виводить файли, ім'я яких не починається з D та P | 
| cd / | Переходить до кореневого каталогу | 
| cd ~ | Переходить до домашнього каталогу | 
| cd .. | Переходить на один рівень вище | 
| ls | Виводить список файлів і каталогів поточного каталогу | 
| ls -a | Виводить усі файли, включно з прихованими | 
| ls -R | Виводить вміст каталогу і всіх його підкаталогів | 
| mkdir | Створює новий каталог, наприклад | 
| rmdir | Видаляє каталог, але тільки порожній | 
| rm -r | Видаляє каталог разом з усім вмістом | 
| touch | Створює порожній файл розміром 0 байтів | 
<br>
<br> 

### Завдання 3 - Робота в в терміналі (закріплення практичних навичок) обов'язково представити свої скріншоти:
#### 3.1 Визначте ваш поточний робочий каталог;
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/31.png?raw=true)
<br> 

#### 3.2 Перейдіть до кореневого каталогу та визначте Ваш поточний робочий каталог (дві команди);
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/32.png?raw=true)
<br> 

#### 3.3 Перегляньте вміст поточного каталогу у довгому форматі (скористайтесь відповідним ключем команди ls);
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/33.png?raw=true)
<br> 

#### 3.4 Перейдіть до каталогу /usr/share та визначте Ваш поточний робочий каталог (дві команди)
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/34.png?raw=true)
<br> 

#### 3.5 Перегляньте вміст поточного каталогу включаючи і приховані файли (hidden files) (скористайтесь відповідним ключем команди ls);
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/35.png?raw=true)
<br> 

#### 3.6 Перейдіть до каталогу /etc;
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/36.png?raw=true)
<br> 

#### 3.7 Перегляньте вміст даного каталогу, але щоб виводило тільки назви файлів, що починаються з літери вашого імені;
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/37.png?raw=true)
<br> 

#### 3.8 Перегляньте вміст даного каталогу, але щоб виводило тільки файли, назви яких складаються з 6 літер;
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/38.png?raw=true)
<br> 

#### 3.9 Перегляньте вміст даного каталогу, але щоб виводило тільки файли, назви яких закінчуються на літери ваших імен, наприклад якщо ваші імена Ivan, Anna, Maks, то вибірку робиму, щоб назви файлів закінчувались на літери [i,a,m];
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/39.png?raw=true)
<br> 

#### 3.10 Перейдіть до домашнього каталогу поточного користувача та перегляньте його вміст у рекурсивному (зворотному до алфавітного) форматі (виконати цю дію через конвеєр команд);
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/310.png?raw=true)
<br> 

#### 3.11 В поточній директорії створити директорію з назвою вашої групи;  
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/311.png?raw=true)
<br> 

#### 3.12 Переглянути оновлений вміст домашнього каталогу поточного користувача. Скористайтесь ключем -r команди ls, яку інформацію ви отримаєте?
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/312.png?raw=true)
<br> 

#### 3.13 Перейдіть у створену вами директорію з назвою Вашої групи та створіть у ній порожній файл lab5
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/313.png?raw=true)
<br> 

#### 3.14 Створити в даній директорії 3 директорії з прізвищами студентів вашої команди surname1, surname2, surname3 (команда mkdir мульти аргумента, тому всі три каталоги можна створити однією командою);
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/314.png?raw=true)
<br> 

#### 3.15 Перейдіть у перший підкаталог surname1 та створіть порожній файл з ім'ям першого студента name1;  
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/315.png?raw=true)
<br> 

#### 3.16 За допомогою команди echo "Hello, my name is Name1" > name1 внесіть у цей файл дані про студента (символ > дозволяє вивід команди echo перенаправити одразу у файл name1; 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/316.png?raw=true)
<br> 

#### 3.17 Перегляньте вміст файлу name1 за допомогою команди cat name1 (має містити щойно введену Вами інформацію) 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/317.png?raw=true)
<br> 

#### 3.18 Зробіть копію першого файлу name1 та перейменуйте її у файл з другим ім'ям студенту Вашої команди name2; 
> я працюю сама, тому вказала випадкове прізвище та ім'я

![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/318.png?raw=true)
<br> 

#### 3.19 Перегляньте вміст каталогу, обидва файли мають з'явитися;  
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/319.png?raw=true)
<br> 

#### 3.20 Перегляньте вміст другого файлу cat name2 (він має поки що містити повну копію вмісту файлу name1)   
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/320.png?raw=true)
<br> 

#### 3.21 Замініть зміст файлу name2, щоб він містив відповідне ім'я другого студента за допомогою команди echo "Hello, my name is Name2" > name2 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/321.png?raw=true)
<br> 

#### 3.22 Перегляньте вміст другого файлу cat name2 (він вже має містити оновлену інформацію) 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/322.png?raw=true)
<br> 

#### 3.23 Перемістіть файл name2 у директорію surname2; 
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/323.png?raw=true)
<br> 

> завдання 3.24 - 3.29 подібні до минулих і я працюю сама, тому я їх не виконувала

#### 3.30 Поверніться до домашнього каталогу користувача;
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/330.png?raw=true)
<br> 

#### 3.31 Перегляньте вміст даного каталогу, але щоб виводило тільки Ваш підкаталог з назвою групи та весь його вміст (підкаталоги surname1, surname2, surname3 та файли name1, name2, name3) до того ж файли та катлоги були відкоремлені кольорами (скористайтесь відповідним ключем -R команди ls та не забудьте використати спеціальний glob-шаблон [імя каталогу])
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork5/photos/331.png?raw=true)
<br> 
<br> 

### Завдання 4(5) - Опишіть дії, які виконують команди для переміщення по системі каталогів:
1. `cd /`	- переходить до кореневого каталогу
2. `cd /home` - переходить до каталогу /home
3. `cd ~`	- переходить до домашнього каталогу
4. `cd (без аргумента)` - аналог попередній команді, переходить до домашнього каталогу
5. `cd ..` - переходить на один рівень вище до батьківського каталогу
6. `cd ../..` - переходить на два рівні вище
7. `cd -` - повертає до попереднього каталогу

 
