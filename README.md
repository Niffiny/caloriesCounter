# Проект «Счётчик калорий»
* Студент: [Николь Исмагилова](https://up.htmlacademy.ru/univer-js1/2/user/2241645).
Запуск:
- npm i
- npm run build
- npm run start

# Техническое задание проекта 

## Состояние по умолчанию:
- Выбран мужской пол.
- В полях ввода стоит 0.
- Выбрана «минимальная» физическая активность.
- Кнопка «Рассчитать» неактивна.
- Кнопка сброса данных из полей ввода неактивна.
- Блок с выводом информации о калориях скрыт.


## Кнопка «Рассчитать»:
- Становится активна только когда заполнены все поля ввода.
- По клику на кнопку появляется блок с информацией о калориях, если до этого он не был показан. Если блок уже находится на странице, клик по кнопке обновляет расчёты, выводится актуальная информация.

## Кнопка «Очистить поля и расчёт»:
- Становится активна, когда хотя бы одно числовое поле заполнено.
- При клике все элементы приложения сбрасываются до состояния по умолчанию: числовые поля очищаются (плейсхолдер 0), пол становится мужской, физическая активность «минимальная», блок с информацией о калориях скрывается.

# Формулы
## Поддержание веса:

### Для женщин:
N = (10 × вес в килограммах) + (6,25 × рост в сантиметрах) − (5 × возраст в годах) − 161

### Для мужчин:
N = (10 × вес в килограммах) + (6,25 × рост в сантиметрах) − (5 × возраст в годах) + 5

Полученное значение (N) умножаем на коэффициент активности. Результат и будет нормой калорий для поддержания веса.

## Коэффициенты активности:
- Минимальная: 1.2
- Низкая: 1.375
- Средняя: 1.55
- Высокая: 1.725
- Очень высокая: 1.9

## Формулы для набора и сброса веса:
- Набор веса: прибавляем 15% от нормы к этой норме
- Сброс веса: вычитаем 15% от нормы из этой нормы