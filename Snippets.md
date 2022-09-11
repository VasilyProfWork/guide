{

    // Place your GLOBAL snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and

    // description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope

    // is left empty or omitted, the snippet gets applied to all languages. The prefix is what is

    // used to trigger the snippet and the body will be expanded and inserted. Possible variables are:

    // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders.

    // Placeholders with the same ids are connected.

    // Example:

    "Основная структура компонента": {

        "prefix": "vb",

        "body": [

            "<template lang=\"pug\">",

            "div",

            "   include ./$1.pug",

            "</template>",

            "",

            "<script>",

            "export default {",

            "   name: \"$1\",",

            "};",

            "</script>",

            "",

            "<style lang=\"scss\">",

            "@import \"$1.scss\";",

            "</style>"

        ],

        "description": "Основная структура компонента"

    },

    "Print to console": {

        "scope": "javascript,typescript",

        "prefix": "log",

        "body": [

            "console.log('$1');",

            "$2"

        ],

        "description": "Log output to console"

    },

    "Внешний отступ сверху снизу": {

        "prefix": "mtb",

        "body": [

            "margin: $1px 0px;"

        ],

        "description": "Внешний отступ сверху снизу"

    },

    "Внешний отступ слева справо": {

        "prefix": "mrl",

        "body": [

            "margin: 0px $1px;"

        ],

        "description": "Внешний отступ слева справа"

    },

    "Внутренний отступ сверху снизу": {

        "prefix": "ptb",

        "body": [

            "padding: $1px 0px;"

        ],

        "description": "Внутренний отступ сверху снизу"

    },

    "Внутренний отступ слева справа": {

        "prefix": "prl",

        "body": [

            "padding: 0px $1px;"

        ],

        "description": "Внутренний отступ слева справа"

    },

    "Медиа запрос any-hover": {

        "prefix": "any",

        "body": [

            "@media (any-hover: hover) {",

            "    &:hover {$0}",

            "}"

        ],

        "description": "Медиа запрос any-hover"

    },

    "Транзишин": {

        "prefix": "tr",

        "body": [

            "transition: all 0.3s ease 0s;"

        ],

        "description": "Транзишин"

    },

    "Flex увел. 0 и умен. 1": {

        "prefix": "fl",

        "body": [

            "flex: 0 1 auto;"

        ],

        "description": "Flex запрещает увеличиться и разрешает уменьшаться"

    },

    "Flex колонка": {

        "prefix": "fdc",

        "body": [

            "flex-direction: column;"

        ],

        "description": "Flex колонка"

    },

    "Flex выравнивание по центру": {

        "prefix": "fc",

        "body": [

            "justify-content: center;",

            "align-items: center;"

        ],

        "description": "Flex выравнивание по центру"

    },

    "Flex wrap": {

        "prefix": "fwr",

        "body": [

            "flex-wrap: wrap;"

        ],

        "description": "Flex wrap"

    },

    "background": {

        "prefix": "bgu",

        "body": [

            "background: url('../img/$1') 0px 0px/auto 100% no-repeat;"

        ],

        "description": "background"

    },

    "not last child": {

        "prefix": "no",

        "body": [

            "&:not(:last-child){margin-bottom: $1px}"

        ],

        "description": "not last child"

    },

    "grid-template-columns List": {

        "prefix": "gis",

        "body": [

            "display: grid;",

            "grid-template-columns: repeat(auto-fit, minmax($1px, 1fr));",

            "grid-auto-rows: 1fr;"

        ],

        "description": "grid template columns"

    },

    "grid-template Item": {

        "prefix": "gi",

        "body": [

            "display: grid;",

            "grid-auto-flow: row;",

            "grid-template: auto 1fr minmax($1px, auto) / 1fr;"

        ],

        "description": "grid template Одной карточки"

    },

    "media min setting": {

        "prefix": "mmg",

        "body": [

            "@media (min-width: $1px){\n\t $0 \n}"

        ],

        "description": "mms"

    },

    "media max setting": {

        "prefix": "mg",

        "body": [

            "@media (max-width: $1px){\n\t $0 \n}"

        ],

        "description": "ms1"

    },

    "md1 pc containerWidth": {

        "prefix": "md1",

        "body": [

            "@media (max-width:\\$pc){\n\t $0 \n}"

        ],

        "description": "md1"

    },

    "mmd1 min pc containerWidth": {

        "prefix": "mmd1",

        "body": [

            "@media (min-width:\\$pc){\n\t $0 \n}"

        ],

        "description": "md1"

    },

    "md2 tablet 991.98": {

        "prefix": "md2",

        "body": [

            "@media (max-width:\\$tablet){\n\t$0\n}"

        ],

        "description": "md2"

    },

    "mmd2 min tablet 991.98": {

        "prefix": "mmd2",

        "body": [

            "@media (min-width:\\$tablet){\n\t $0 \n}"

        ],

        "description": "md1"

    },

    "md3 mobile 767.98": {

        "prefix": "md3",

        "body": [

            "@media (max-width:\\$mobile){\n\t $0 \n}"

        ],

        "description": "md3"

    },

    "mmd3 min mobile 767.98": {

        "prefix": "mmd3",

        "body": [

            "@media (min-width:\\$mobile){\n\t $0 \n}"

        ],

        "description": "md1"

    },

    "md4 mobileSmall 479.98": {

        "prefix": "md4",

        "body": [

            "@media (max-width:\\$mobileSmall){\n\t $0 \n}"

        ],

        "description": "md4"

    },

    "mmd4 min mobileSmall 479.98": {

        "prefix": "mmd4",

        "body": [

            "@media (min-width:\\$mobileSmall){\n\t $0 \n}"

        ],

        "description": "md1"

    },

    "Rating": {

        "scope": "html",

        "prefix": "rating",

        "body": [

            "<div class=\"rating rating_set\">\n\t<div class=\"rating__body\">\n\t\t<div class=\"rating__active\"></div>\n\t\t<div class=\"rating__items\">\n\t\t\t<input type=\"radio\" class=\"rating__item\" value=\"1\" name=\"rating\">\n\t\t\t<input type=\"radio\" class=\"rating__item\" value=\"2\" name=\"rating\">\n\t\t\t<input type=\"radio\" class=\"rating__item\" value=\"3\" name=\"rating\">\n\t\t\t<input type=\"radio\" class=\"rating__item\" value=\"4\" name=\"rating\">\n\t\t\t<input type=\"radio\" class=\"rating__item\" value=\"5\" name=\"rating\">\n\t\t</div>\n\t</div>\n\t<div class=\"rating__value\">3.6</div>\n</div>"

        ],

        "description": "Добавляет базовый HTML код рейтинга"

    },

    "Spollers": {

        "scope": "html",

        "prefix": "spollers",

        "body": [

            "<div data-spollers class=\"spollers\">\n\t<div class=\"spollers__item\">\n\t\t<button type=\"button\" data-spoller class=\"spollers__title\">Заголовок спойлера</button>\n\t\t<div class=\"spollers__body\">Контент спойлера</div>\n\t</div>\n</div>"

        ],

        "description": "Добавляет базовый HTML код спойлеров"

    },

    "Tabs": {

        "scope": "html",

        "prefix": "tabs",

        "body": [

            "<div data-tabs class=\"tabs\">\n\t<nav data-tabs-titles class=\"tabs__navigation\">\n\t\t<button type=\"submit\" class=\"tabs__title _tab-active\">Таб №1</button>\n\t\t<button type=\"submit\" class=\"tabs__title\">Таб №2</button>\n\t\t<button type=\"submit\" class=\"tabs__title\">Таб №3</button>\n\t</nav>\n\t<div data-tabs-body class=\"tabs__content\">\n\t\t<div class=\"tabs__body\">\n\t\t\t1 Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore odio exercitationem, excepturi similique nulla, voluptatem reprehenderit neque a minima eaque tenetur? Quos fugit voluptate enim quo sed, minima error molestias!\n\t\t</div>\n\t\t<div class=\"tabs__body\">\n\t\t\t2 Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore odio exercitationem, excepturi similique nulla, voluptatem reprehenderit neque a minima eaque tenetur? Quos fugit voluptate enim quo sed, minima error molestias!\n\t\t</div>\n\t\t<div class=\"tabs__body\">\n\t\t\t3 Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore odio exercitationem, excepturi similique nulla, voluptatem reprehenderit neque a minima eaque tenetur? Quos fugit voluptate enim quo sed, minima error molestias!\n\t\t</div>\n\t</div>\n</div>"

        ],

        "description": "Добавляет базовый HTML код табов"

    },

    "Swiper": {

        "scope": "html",

        "prefix": "swiper",

        "body": [

            "<div class=\"${1:имя-блока}__slider swiper\">\n\t<div class=\"${1:имя-блока}__wrapper swiper-wrapper\">\n\t\t<div class=\"${1:имя-блока}__slide swiper-slide\"></div>\n\t</div>\n</div>"

        ],

        "description": "Добавляет базовый HTML код слайдера Swiper"

    },

    "Swiper Full": {

        "scope": "html",

        "prefix": "swiperfull",

        "body": [

            "<!-- Оболочка слайдера -->\n<div class=\"${1:имя-блока}__slider swiper\">\n\t<!-- Двигающееся часть слайдера -->\n\t<div class=\"${1:имя-блока}__wrapper swiper-wrapper\">\n\t\t<!-- Слайд -->\n\t\t<div class=\"${1:имя-блока}__slide swiper-slide\"></div>\n\t</div>\n\t<!-- Если нужна пагинация -->\n\t<div class=\"swiper-pagination\"></div>\n\t<!-- Если нужна навигация (влево/вправо) -->\n\t<button type=\"button\" class=\"swiper-button-prev\"></div>\n\t<button type=\"button\" class=\"swiper-button-next\"></button>\n\t<!-- Если нужен скролбар -->\n\t<div class=\"swiper-scrollbar\"></div>\n</div>"

        ],

        "description": "Добавляет базовый HTML код слайдера Swiper"

    },

    "Quantity HTML формы с кол-вом": {

        "scope": "html",

        "prefix": "quantity",

        "body": "<div class=\"quantity\">\n\t<button type=\"button\" class=\"quantity__button quantity__button_plus\"></button>\n\t<div class=\"quantity__input\">\n\t\t<input autocomplete=\"off\" type=\"text\" name=\"form[]\" value=\"1\">\n\t</div>\n\t<button type=\"button\" class=\"quantity__button quantity__button_minus\"></button>\n</div>",

        "description": "Добавняет HTML формы с кол-вом"

    },

    "Add tooltip Tippy": {

        "scope": "html",

        "prefix": "tip",

        "body": [

            "data-tippy-content=\"Подсказка\""

        ],

        "description": "Добавляет текст-подсказку (Tippy)"

    },

    "Add data-required": {

        "scope": "html",

        "prefix": "req",

        "body": [

            "data-required"

        ],

        "description": "Добавляет атрибут к полю формы"

    },

    "Add dynamic adapt": {

        "scope": "html",

        "prefix": "da",

        "body": [

            "data-da=\".${1:имя блока}, 768\""

        ],

        "description": "Добавляет атрибут динамического адаптива"

    },

    "Add image IBG": {

        "scope": "html",

        "prefix": "ibg",

        "body": [

            "<div class=\"${1:имя блока}__image-ibg\"><img src=\"@img$2\" alt=\"\"></div>"

        ],

        "description": "Добавляет объект с картинкой и классом IBG"

    },

    "Добавляет ссылку с картинкой и классом IBG": {

        "scope": "html",

        "prefix": "ibga",

        "body": [

            "<a href=\"\" class=\"${1:имя блока}__image-ibg\"><img src=\"@img$2\" alt=\"\"></a>"

        ],

        "description": "Добавляет ссылку с картинкой и классом IBG"

    },

    "Добавляет input со настройками": {

        "scope": "html",

        "prefix": "inp",

        "body": "<input autocomplete=\"off\" type=\"text\" name=\"form[]\" data-error=\"Ошибка\" placeholder=\"\" class=\"input\">",

        "description": "Добавляет input со настройками"

    },

    "Ограничивающий контейнер": {

        "scope": "html",

        "prefix": "cnt",

        "body": "<div class=\"${1:имя блока}__container\">\n\t$2\n</div>",

        "description": "Добавляет ограничивающий контейнер"

    },

    "Adaptiv Value": {

        "scope": "scss",

        "prefix": "av",

        "body": [

            "@include adaptiveValue(\"${1:font-size}\", $2, $3);"

        ],

        "description": "Адаптивное свойство: CSS-свойство, начальное значение, конечное значение, ширина начальная, ширина конечная"

    },

    "EM": {

        "scope": "scss",

        "prefix": "em",

        "body": [

            "em($1,$2)"

        ],

        "description": "Вызов миксина перевода в EM"

    },

    "REM": {

        "scope": "scss",

        "prefix": "rem",

        "body": [

            "rem($1)"

        ],

        "description": "Вызов миксина перевода в REM"

    },

    "Percent": {

        "scope": "scss",

        "prefix": "prc",

        "body": [

            "percent($1,$2)"

        ],

        "description": "Вызов миксина перевода в %"

    },

    "Добавляет трибут для открытия попапа": {

        "scope": "html",

        "prefix": "pl",

        "body": [

            "data-popup=\"$1\""

        ],

        "description": "Добавляет трибут для открытия попапа"

    },

    "position absolute whtl": {

        "prefix": "ps",

        "body": [

            "position: absolute;width: 100%;height: 100%;top: 0;left: 0;"

        ],

        "description": "position absolute"

    },

    "After": {

        "prefix": "a",

        "body": [

            "&::after{\n\tcontent:'';\n\t$0\n}"

        ],

        "description": "after"

    },

    "Before": {

        "prefix": "b",

        "body": [

            "&::before{\n\tcontent:'';\n\t$0\n}"

        ],

        "description": "before"

    },

    "kf": {

        "prefix": "kf",

        "body": "@keyframes ${1:name} {\n\t0% {\n\t\t$2\n\t}\n\t100% {\n\t\t$3\n\t}\n}",

        "description": "kf"

    },

    "qa": {

        "scope": "html,kit",

        "prefix": "qa",

        "body": "<div class=\"quantity\"><div class=\"quantity__button quantity__button_plus _icon-plus\"></div><div class=\"quantity__input\"><input autocomplete=\"off\" type=\"text\" name=\"form[]\" value=\"1\"></div><div class=\"quantity__button quantity__button_minus _icon-minus\"></div></div>",

        "description": "qa"

    },

    "Textarea": {

        "scope": "html,kit",

        "prefix": "txta",

        "body": "<textarea autocomplete=\"off\" name=\"form[]\" placeholder=\"$1\" data-error=\"Ошибка\" class=\"input\"></textarea>",

        "description": "txta"

    },

    "Select": {

        "prefix": "sel",

        "body": "<select name=\"form[]\" class=\"form\">\n\t<option value=\"1\" selected>Пункт №1</option>\n\t<option value=\"2\">Пункт №2</option>\n\t<option value=\"3\">Пункт №3</option>\n\t<option value=\"4\">Пункт №4</option>\n</select>",

        "description": "sel"

    },

    "Radio buttons": {

        "prefix": "opt",

        "body": "<div class=\"options\">\n\t<div class=\"options__item\">\n\t\t<input hidden id=\"o_1\" class=\"options__input\" checked type=\"radio\" value=\"1\" name=\"option\">\n\t\t<label for=\"o_1\" class=\"options__label\"><span class=\"options__text\">${1:Текст}</span></label>\n\t</div>\n\t<div class=\"options__item\">\n\t\t<input hidden id=\"o_2\" class=\"options__input\" type=\"radio\" value=\"2\" name=\"option\">\n\t\t<label for=\"o_2\" class=\"options__label\"><span class=\"options__text\">${2:Текст}</span></label>\n\t</div>\n</div>",

        "description": ""

    },

    "CheckBox": {

        "prefix": "chk",

        "body": "<div class=\"checkbox\">\n\t<input id=\"c_1\" data-error=\"Ошибка\" class=\"checkbox__input\" type=\"checkbox\" value=\"1\" name=\"form[]\">\n\t<label for=\"c_1\" class=\"checkbox__label\"><span class=\"checkbox__text\">${1:Текст}</span></label>\n</div>",

        "description": ""

    },

    "Button": {

        "prefix": "btn",

        "body": "<button type=\"submit\" class=\"button\">${1:Отправить}</button>",

        "description": ""

    },

    "Button Item": {

        "prefix": "bbtn",

        "body": "<button type=\"button\" class=\"${1:class}\">${2:Текст}</button>",

        "description": ""

    },

    "Button Link": {

        "prefix": "abtn",

        "body": "<a href=\"\" class=\"button\">${1:Текст}</a>",

        "description": ""

    },

    "menu": {

        "prefix": "menu",

        "body": "<div class=\"header__menu menu\">\n\t<button type=\"button\" class=\"menu__icon icon-menu\"><span></span></button>\n\t<nav class=\"menu__body\">\n\t\t<ul class=\"menu__list\">\n\t\t\t<li class=\"menu__item\"><a href=\"\" class=\"menu__link\"></a></li>\n\t\t</ul>\n\t</nav>\n</div>",

        "description": "menu"

    },

    "last-child margin-bottom": {

        "prefix": "ll",

        "body": "&:last-child{\n\t margin-bottom: 0px; \n}$0",

        "description": "last-child margin-bottom"

    },

    "last-child margin-right": {

        "prefix": "l",

        "body": "&:last-child{\n\t margin-right: 0px; \n}$0",

        "description": "last-child margin-right"

    },

    "margin-top-right-left": {

        "prefix": "mmm",

        "body": "margin: -$1px -$2px 0px;$0",

        "description": "margin-top-right-left"

    },

    "padding-top-right-left": {

        "prefix": "ppp",

        "body": "padding: $1px $2px 0px;$0",

        "description": "padding-top-right-left"

    },

    "Splide js": {

        "prefix": "splide",

        "body": "<div class=\"splide\" role=\"group\" aria-label=\"Splide Basic HTML Example\">\n\t<div class=\"splide__track\">\n\t<ul class=\"splide__list\">\n\t<li class=\"splide__slide\">Slide 01</li>\n\t<li class=\"splide__slide\">Slide 02</li>\n\t<li class=\"splide__slide\">Slide 03</li>\n\t</ul>\n\t</div>\n\t</div>",

        "description": "splide"

    },

}