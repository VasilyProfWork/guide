# JSON
----

>Это обьект или массив, который может передать свою инфу в другие языки программирование, проброзовав себя в строку.

Синтаксис:
```js
let json = '[1, 2, 3, 4, 5,]'; // неверно запятая в конце
let json = '[1, 2, 3, 4, 5]';  // верно
```

- `JSON.parse()` берет строку JSON и трансформирует ее в объект JavaScript. 
- `JSON.stringify()` берет объект JavaScript и трансформирует его в строку JSON.

>Чтобы изменить в строке JSON какие-либо данные, для начало нужно проброзовать в массивы или обьекты, изменить данные, затем пробразовать в строку JSON.

----

Объект JSON выглядит примерно так:
```js
{
  "first_name" : "Sammy",
  "last_name" : "Shark",
  "location" : "Ocean",
  "online" : true,
  "followers" : 987 
}
//двойные ковычки
//нет запятой в конце
```

----

Преобразование строки JSON в структуру данных (в массивы или обьекты):
```js
//Пусть у нас есть строка, содержащая массив в формате JSON:
let json = '[1, 2, 3, 4, 5, "a", "b"]';

//Преобразуем нашу строку в массив:
let arr = JSON.parse(json);
```

---

Преоброзование массивов или обьектов в формат JSON:
```js
let arr = [1, 2, 3, 4, 5, 'a', 'b'];

//Преобразуем наш массив в строку:
let json = JSON.stringify(arr);
```

---

json обьект
```json
{
  "squadName": "Super hero squad",
  "homeTown": "Metro City",
  "formed": 2016,
  "secretBase": "Super tower",
  "active": true,
  "members": [
    {
      "name": "Molecule Man",
      "age": 29,
      "secretIdentity": "Dan Jukes",
      "powers": [
        "Radiation resistance",
        "Turning tiny",
        "Radiation blast"
      ]
    },
    {
      "name": "Madame Uppercut",
      "age": 39,
      "secretIdentity": "Jane Wilson",
      "powers": [
        "Million tonne punch",
        "Damage resistance",
        "Superhuman reflexes"
      ]
    },
    {
      "name": "Eternal Flame",
      "age": 1000000,
      "secretIdentity": "Unknown",
      "powers": [
        "Immortality",
        "Heat Immunity",
        "Inferno",
        "Teleportation",
        "Interdimensional travel"
      ]
    }
  ]
}

superHeroes['members'][1]['powers'][2]
```


json массив
```json
[
  {
    "name": "Molecule Man",
    "age": 29,
    "secretIdentity": "Dan Jukes",
    "powers": [
      "Radiation resistance",
      "Turning tiny",
      "Radiation blast"
    ]
  },
  {
    "name": "Madame Uppercut",
    "age": 39,
    "secretIdentity": "Jane Wilson",
    "powers": [
      "Million tonne punch",
      "Damage resistance",
      "Superhuman reflexes"
    ]
  }
]

superHeroes[0]["powers"][0]
```