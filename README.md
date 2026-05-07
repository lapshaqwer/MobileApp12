<div align="center">

## Отчет

</div>

<div align="center">

## Практическая работа 12

</div>

<div align="center">

## Типы активностей. Шаблоны Android Studio. Сохранение настроек с SharedPreferences.

</div>

---

**ФИО:** Лапшин Никита Евгеньевич  
**Курс:** 2
**Группа:** ИНС-б-о-24-1  
**Направление:** 09.03.02 «Информационные системы и технологии»  

---
### Вариант 9
### Цель работы

Изучить различные типы шаблонов активностей, предоставляемых Android Studio. Научиться создавать многоэкранные приложения с использованием разных видов окон. Освоить механизм сохранения простых пользовательских настроек с помощью SharedPreferences.

### Ход работы

<div align=center>
  
![Скриншот 1](images/1.png)

Рисунок 1 - Инициализация 

![Скриншот 2](images/2.png)

Рисунок 2 - Инициализация UI

![Скриншот 3](images/3.png)

Рисунок 3 – Окно настроек

![Скриншот 4](images/4.png)

Рисунок 4 – Сброс рекорда

![Скриншот 5](images/5.png)

Рисунок 5 – Инициализация в GameActivity

![Скриншот 6](images/6.png)

Рисунок 6 – Инициализация UI

![Скриншот 7](images/7.png)

Рисунок 7 – Настройки, старт игры и обновление UI

![Скриншот 8](images/8.png)

Рисунок 8 – Обработка логики игры

![Скриншот 9](images/9.png)

Рисунок 9 – Обработка победы, поражения и вывод подсказки

![Скриншот 10](images/10.png)

Рисунок 10 – Окончание игры

![Скриншот 11](images/11.png)

Рисунок 11 - Обновление рекорда

![Скриншот 12](images/12.png)

Рисунок 12 - Окно рекордов

![Скриншот 13](images/13.png)

Рисунок 13 - Формирование наилучших результатов

![Скриншот 14](images/14.png)

Рисунок 14 - Главное меню

![Скриншот 15](images/15.png)

Рисунок 15 - Окно игры

![Скриншот 16](images/16.png)

Рисунок 16 - Окно рекордов

## Контрольные вопросы
1. Empty Views Activity (пустая основа), Settings Activity (готовый экран настроек с PreferenceFragment), Fullscreen Activity (полноэкранный режим, скрывает панели), Login Activity (форма входа/регистрации)
2. SharedPreferences — хранилище простых данных в виде пар "ключ-значение", можно хранить int, long, float, boolean, String, Set<String>.
3. getPreferences() создаёт файл для конкретной Activity, getSharedPreferences(name) — для указанного файла, PreferenceManager.getDefaultSharedPreferences() — единый файл по умолчанию.
4. Запись через editor.put...() и apply() (асинхронно) или commit() (синхронно, возвращает boolean) — apply() быстрее и не блокирует поток.
5. Чтение через prefs.getТип("key", defaultValue); значение по умолчанию нужно чтобы избежать NullPointerException, если ключ отсутствует.
6. New → Activity → Settings Activity, элементы настройки описываются в res/xml/preferences.xml (EditTextPreference, SwitchPreference и др.).
7. Intent intent = new Intent(CurrentActivity.this, TargetActivity.class); startActivity(intent);
8. FloatingActionButton — круглая плавающая кнопка действия, присутствует в шаблонах Scrolling Activity и Navigation Drawer Activity.
