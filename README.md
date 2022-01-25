# Lionic.
## Практика по продвинутому CSS.

## Разметка html.
------------
### Первоначальная разметка (Папка Start).

- Создана файловая система сайта
- Размечен header и меню навигации
- Добавлены блоки сеций и футер
- Реализована навигация по секциям

### Разметка секций hero и services.

- Выполнена разметка секции Hero.
- Размечена секция Services.
- Экспортированы фоновые картинки для карточек секции в формате svg.
- Картинки вставлены в карточки в виде svg кода.

### Разметка секций articles и clients.

#### Секция articles.

- Добавлен контейнер и заголовок блока articles.
- Добавлен список из четырех блоков в котором будут превью статей.
- Добавлен текстовый контент в превью.
- Добавлены изображения.

#### Секция clients.

- Добавлен контейнер и заголовок блока clients.
- Добавлен список из трех блоков с отзывами клиентов, их именами и фото.
- Экспортированы и добавлены картинки.

### Разметка секций contacts и footer.

#### Секция contacts.

-   Добавлен контейнер и заголовок блока contacts
-   Добавлен address, содержащий список из трех пунктов
-   Добавлены ссылки.

#### footer

- Сверстан [Из готового макета](https://disk.yandex.ru/d/Buhi7kFIlcpREA)
- Добавлены иконки соцсетей


## Стилизация Flexbox (папка Stylization).


### Подготовка стилей проекта и header.

#### Подготовка стилей.

- Подключен [normalize.css](https://necolas.github.io/normalize.css/8.0.1/normalize.css)
- Подключен style.css
- Добавлены глобальные стили box-sizing:    border-box;
- Добавлены вспомогательные классы:
    - list-reset
    - btn-reset
    - flex
- Назначена ширина контейнера.
- Назначены общие классы:
    - section-title
    - section-description
    - section-offset

#### header.

- Применены отступы к блоку header.
- К контейнеру хедера добавлены классы flex и свойство align-items:center;

##### ВАЖНО!

__Для стилизации хедера в дальнейшем может пригодиться вот это:__

- К блоку _logo_ применен _margin-right: auto_ .
- Следующий _margin-right_ применен к _nav_
- К списку навигации применен класс _flex_.
- Стилизация элементов меню:
    - Применение _margin-right_ (not last child) к элементам списка.
    - Применение стилей к ссылкам.
    
### Стилизация flexbox блоков Hero и Services.

#### Hero flexbox stylization.

- Назначение вертикального паддинга секции Hero.
- Назначение максимальной ширины в 50% контентной части блока.
- Блоку контента присвоен класс _flex_ и свойства _flex-direction: column;_ , _align-items: flex-start;_
- Примененны соответствующие нижние отступы ко всем элементам контента.

#### Services flexbox stylization.

- Центрирование заголовка и описания.
- Применение к списку с карточками класса _flex_.
- Применение класса _flex_ к элементам списка.
- Применение отступов справа к карточкам.
- Применение отступов к элементам карточек.

### Стилизация flexbox блоков Articles и Clients.

#### Articles flexbox stylization.

- Применение нижнего маргина к заголовку блока.
- Применение класса _flex_ и свойства _flex-wrap: wrap;_ к списку с карточками.
- Применение заданой ширины к карточкам.
- Применение отступов справа к карточкам.
- Стилизация карточек:
    - Применение к картинкам свойства _object-fit: cover;_ (хорошая практика на случай нестандартного размера картинки).
    - Применение паддинга к контентной части карточек.
    - Применение нижних маргинов к элементам карточки.

#### Clients flexbox stylization.

- Применение нижнего маргина к заголовку блока.
- Применение класса _flex_ к списку и к карточкам.
- Применение к карточкам свойства _flex-direction: column;_.
- Назначение паддингов для карточек.
- Применение отступов справа к карточкам.
- Стилизация элементов карточек.
- __ВАЖНО!__ к картинке клиента нужно применить свойство _flex-shrink: 0;_ во избежание ее сжатия.

### Стилизация flexbox блоков contacts и footer.

Стилизация секции contacts и footer осуществляется так же, как и предыдущих блоков.

## Окончательная стилизация сайта (Папка Stylization2).

### Добавление и подключение шрифтов.

- Создана папка _fonts_ в котороую помещены файлы шрифтов в форматах _woff_ и _woff-2_.
- Шрифты подключены в файле _style.css_ 

### Header, hero и services.


#### Header

- Применен нижний бордер ко всему блоку _header_ и назначен фоновый цвет #fff.
- Стилизация ссылок в меню.
- Стили для кнопки по умолчанию (класс _btn_).
- Стили для кнопки блока _header_

#### Hero

- Импортирован файл фонового рисунка (в масштабе x2).
- Назначение фона для блока _hero_ и его масштабирование.
- Стили заголовка.
- Стили описания.
- Стили кнопки.
- Стили нижнего спана.
- Фоновый рисунок нижнего спана.

#### Services

- Стилизация заголовка второго уровня по умолчанию.
- Стилизация подзаголовка.
- Бордер и паддинги для карточек.
- Нижний бордер для секции по умолчанию.

### Articles и Clients.

#### Articles.

- Применение бордера к тегам _article_.
- Применение _overflov: hidden;_ к тегам _article_ (позволяет реализовать бордер-радиус для картинок).
- Стилизация типографики контента в соответствии с макетом.

#### Clients.

- Применение бордера к тегам _section-clients__item__ .
- Стилизация текстового блока.
- Стилизация нижней части карточки:
    - Применение верхнего бордера к тегам _client-info_ .
    - Применение вернего паддинга к тегам _client-info_ .
    - Стилизация картинки:
        - к картинке применен следующий стиль:
        ```css
        .client-info__image  {
            width: 100%;
            height: 100%;
            border: 2px solid #3172B9;
            border-radius: 100%;
            }
        ```
    - Стилизация типографики нижней части карточки.
    
### Contacts и footer.

#### Contacts.

- Добавлены фоновые изображения иконок к карточкам.
- Верхний паддинг для блоков.
- Стилизация типографики и задание ```css max-width: 214px;``` текстовому блоку в первой карточке.

### Footer.

- Применение стиля к блоку копирайта.
- Применение стиля к ссылкам в списке.
- Применение стилей к ссылкам соцсетей.
    - Свойство ```css display: block;``` для класса ```social-link``` .
    - Задание горизонтальных и вертикальных размеров для ссылки.
    - Экспорт иконок соцсетей из макета.
    - назначение иконок соцсетей фоновым рисунком для ссылок (через уникальные классы).

## Создание блока формы (папка Stylization3(form)).

### HTML верстка блока.

- Создание блока и его структуры с соответствующими классами.
- Создание формы, с атрибутом ```action="https://jsonplaceholder.typicode.com/posts"```
- Создание Flexbox структуры формы.
- Создание элементов формы.
- Стилизация элементов.

## Эффекты анимации (папка Complete).

### Анимация ссылок в меню.

    ```css
            .header-nav__link {
        font-weight: 600;
        color: #1c1c1c;
        font-size: 15px;
        transition: color .3s ease;
        }

        .header-nav__link:hover  {
        color: #3172B9;
        }

        .header-nav__link:focus {
        color: #1c1c1c;
        outline: 1px solid #71A7E2;
        }

        .header-nav__link:active  {
        color: #3172B9;
        text-decoration:#3172B9  underline;
        }
    ```
### Анимация кнопок.

    ```css
            .btn  {
        padding: 15px;
        color: #fff;
        background-color: #3172B9;
        border-radius: 3px;
        font-weight: 600;
        font-size: 15px;
        text-transform: uppercase;
        transition: background-color .3s ease;
        }

        .btn:hover  {
        background-color: #71A7E2;
        ;
        }

        .btn:focus {
        background-color: #3172B9;
        outline: 1px #71A7E2;
        }

        .btn:active {
        background-color: #0E3B6C;
        }
    ```
### Анимация карточек в секции Сервисы:

```css
            .services-list__item  {
        transition-property: background-color, color;
        transition-duration: .3s;
        transition-timing-function: ease;
        }
        .services-list__item:hover  {
        cursor: pointer;
        color: #fff;
        background-color: #3172B9;

        }

        .services-list__item:hover .services-list__text  {
        color: #fff;
        }

        .services-list__item:hover path {
        fill: #fff;
        }

        .services-list__item:focus-within {
        color: #fff;
        background-color: #71A7E2;
        }

        .services-list__item:focus-within .services-list__text  {
        color: #fff;
        }

        .services-list__item:focus-within path  {
        fill: #fff;
        }

        .services-list__item:active {
        color: #fff;
        background-color: #0E3B6C;
        }

        .services-list__item:active .services-list__text  {
        color: #fff;
        }

        .services-list__item:active path  {
        fill: #fff;
        }


        .services-list__item path {
        transition: fill .3s ease;
        }
        
        .services-list__text  {
        transition-property: color;
        transition-duration: .3s;
        transition-timing-function: ease;
        }
            
```
### Анимация ссылок контактов.

```css 
    .contacts-item-link {
    font-weight: 400;
    font-size: 14px;
    line-height: 180%;
    color: #787878;
    border: 1 px solid #fff;
    transition-property: color, border;
    transition-duration: .3s;
    transition-timing-function: ease;
    }

    .contacts-item-link:hover {
    color: #71A7E2;
    }

    .contacts-item-link:focus:not(:active) {
    color: #787878;
    border: 1px solid #71A7E2;
    }

    .contacts-item-link:active  {
    border: 1 px solid #fff;
    color: #0E3B6C;
    }
``` 
### Анимация элементов формы:

- Инпуты:
    
    ```css
    .join-form__input {
    width: 251px;
    height: 60px;
    box-sizing: border-box;
    border: 1px solid #dadada;
    border-radius: 50px;
    outline: none;
    padding: 15px 28px;
    transition-property: background-color, color, border;
    transition-duration: .3s;
    transition-timing-function: ease;
    }

    .join-form__input:hover {
    border: 1px solid #71A7E2;
    }

    .join-form__input:focus:not(:active)  {
    border: 1px solid #71A7E2;
    color: #1c1c1c;
    background-color: rgba(113, 167, 226, 0.2) ;
    }
    ```

    
