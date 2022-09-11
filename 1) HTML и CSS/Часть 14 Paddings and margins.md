# Работа с padding и margin
---

Правильный кроссбраузерный отступ справа и снизу:
```scss
.menu__item {
	margin-right: 10px;
	&:last-child {
		margin-raight: 0;
	}
}
```

----

Отступы по бокам в 6 карточках:
```scss
.cards__row {
    display: flex;  
    flex-wrap: wrap;
    margin: 0 -8px;
    margin-top: -8px;
}

.cards__column {
    flex: 1 1 30%;
    padding: 0 8px;
    padding-top: 8px;
}

.cards__item {
    border: 1px solid red;
}
```
