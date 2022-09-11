##### Получение JSON через `request`

Присваиваем переменной ссылку
```js
const header = document.querySelector('header');

// Присваиваем ссылку
let requestURL = 'https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json';

// Создаем экземпляр обьекта запроса из конструктора
// Получение данных без перезагрузки
let request = new XMLHttpRequest();

// Открываем новый запрос использую метод опен
request.open('GET', requestURL);

// Преобразуем ответ json в обьект
request.responseType = 'json';
  
// Отправляем запрос и устанавливаем соединение
request.send();

request.onload = function () {
    // Сохраняем ответ на наш запрос доступный в свойстве response
    let superHeroes = request.response;

	// пердаем наш обьект в функцию
    populateHeader(superHeroes);
}
  
function populateHeader(jsonObj) {
    var myH1 = document.createElement('H1');
    myH1.textContent = jsonObj.squadName;
    header.appendChild(myH1);
}
```


##### Получение JSON через `fetch` и `async`
fetch это промисс

```js
async function go() {
    try {
        let url = 'https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json';
        
        // Получаем данные
        let response = await fetch(url);
        
        // Проверяем условием что ошибок нету
        if (response.ok) {
        
            // Преобразуем данные в обьект
            let data = await response.json();
            
            // Передаем в функцию что выше в примере
            populateHeader(data);
        }
    } catch (e) {
        console.error(e);
        console.error('Можно написать свою ошибку');
    }
}

go()
```


##### Получение json через `fetch` и `.then`
```js
let url = 'https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json';

fetch(url)
    .then(function (data) {
        if (data.ok) return data.json();
    })
    .then(function (data) {
        populateHeader(data);
    })
    .catch(
	function(error) {
		console.log(error);
		console.log('Можно написать свою ошибку');
	}
```