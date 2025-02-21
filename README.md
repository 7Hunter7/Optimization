# Пояснения к изменениям в CSS:

1. **Переменные CSS**: Я оставил переменные CSS, так как они используются для кастомизации цветов, которые не предоставляются Bootstrap “из коробки”. Это позволяет легко менять цветовую схему сайта.

2. **Анимация fadeIn**: Оставил анимацию fadeIn, так как не имеет аналогов в Bootstrap.

3. **Активная вкладка (.browser-tab.active)**: Стили для активной вкладки оставлены, так как они требуют кастомного оформления, которое не предоставляется Bootstrap.

4. **Цвета**: Определил кастомные стили для цветов в заголовках и иконках, используя переменные CSS.

5. **Ширина (.w-85)**: Удалил, так как это можно сделать с помощью классов Bootstrap `w-\*`.

6. **Анимация Hover**: Улучшил анимацию hover, сделав ее более плавной и приятной для глаз. Применил ее ко всем карточкам, кроме `.card-service-item`.

7. **Удаленные стили**: Удалил стили, которые были заменены классами Bootstrap (например, `.browser-tab:focus`, `.browser-tab`, `.browser-tab:hover`, .`fs-7`, `.fs-8`, `.fs-ultra`, `.custom-card:hover`).

8. **Медиа-запросы**: Удалил все media queries, так как их функциональность будет заменена responsive классами Bootstrap в HTML.

# Пояснения к изменениям в HTML

## HTML (верхняя часть):

1. **Bootstrap 5.2**: Убедился, что подключен Bootstrap 5.2.3.

2. **my-4 заменен на py-4**: Изменил `my-4` на `py-4` в `<div class="content">`, чтобы контролировать вертикальный padding, а не margin.

3. **fs-8 заменен на fs-sm-8**: Для большей гибкости добавил класс `btn`, и заменил `fs-8` на `fs-sm-8`. Это позволит задать размер шрифта, начиная с breakpoint sm.

## Секция “Оформление заказа в AVITO”:

1. **tab-content, tab-pane**: Оставил классы `tab-content` и `tab-pane`, так как они необходимы для работы Bootstrap Tabs.

2. **fs-md-3**: Оставил `fs-md-3`, но можно пересмотреть, если нужно другое поведение.

3. **Использованы классы Bootstrap**: `text-center`, `text-md-start`, `mb-_`, `pb-_`, `ps-_`, `d-none`, `d-md-inline-block`, `gap-_`, `w-100`, `alert`, `alert-danger`, `p-3`, `rounded`.

4. **Удалены fs-7 и fs-8**: Заменены на классы `fs-\*` Bootstrap или адаптированы под существующие стили.

## Секция “Варианты доставки AVITO”:

1. **custom-card заменен на card**: Основной класс карточки теперь card Bootstrap. Добавлены классы `shadow`, `d-flex`, `justify-content-center`, `position-relative`, `overflow-hidden`, `rounded`.

2. **Использованы классы Bootstrap**: `col-md-6`, `py-4`, `px-2`, `d-flex`, `flex-column`, `text-center`, `card-title`, `fw-semibold`, `mb-2`, `px-lg-4`, `mb-1`, `btn`, `btn-primary`, `mt-auto`.

3. **Убрана фиксированная высота**: Удалена фиксированная высота для карточек, чтобы контент мог определять высоту.

4. **Добавлены**:

- **d-flex flex-column на .row**: Делает родительский элемент `.row` flex-контейнером и устанавливает направление flex-элементов в колонку;
- **h-100 на .card**: Устанавливает высоту каждой карточки на `100%` от высоты родительского элемента (в данном случае, `.row`).

## Секция “Заполнение заявки доставки”:

1. **fs-7 заменен на fs-6**: В основном контенте, где использовался `fs-7`, я заменил его на fs-6. Это было сделано, чтобы использовать стандартные классы размеров шрифтов Bootstrap.

2. **Сохранены классы Bootstrap**: Сохранены классы `d-none`, `d-md-inline-block`, `gap-\*`, `w-100`, `d-flex`, `flex-column`, `py-0`, `my-0`, `mb-2`.

## Секция “Часто задаваемые вопросы”:

1. **custom-card заменен на card**: Как и в предыдущей секции, `custom-card` заменен на `card` Bootstrap + добавлены необходимые классы.

2. **Удалена фиксированная высота**: Удалена фиксированная высота для `.faq-item`, чтобы контент определял высоту.

3. **Добавлены**:

- **d-flex flex-column на .row**: Делает родительский элемент `.row` flex-контейнером и устанавливает направление flex-элементов в колонку;
- **h-100 на .card**: Устанавливает высоту каждой карточки на `100%` от высоты родительского элемента (в данном случае, `.row`).

4. **fs-7 заменен на fs-6**: В основном контенте, где использовался `fs-7`, я заменил его на `fs-6`.

5. **Сохранены классы Bootstrap**: Сохранены классы `col-md-6`, `my-2`, `my-md-3`, `d-flex`, `flex-column`, `justify-content-center`, `shadow`, `card`, `h-md-auto`, `position-relative`, `text-center`, `p-4`, `rounded`, `bg-white`, `fs-5`, `fw-bolder`, `mb-1`, `mt-4`, `mt-md-0`.

# Итоги работы:

- Весь HTML код был просмотрен и отредактирован.
- Кастомные классы, которые можно было заменить на `Bootstrap`, были заменены.
- Фиксированные высоты были удалены.
- Медиа-запросы были заменены на `responsive` классы Bootstrap.
- Отступы были настроены с использованием `gap` и `margin`/`padding` утилит Bootstrap.
- Код был отформатирован для лучшей читаемости.
