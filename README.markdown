# onePageScroll
one page scroll jquery plugin

-------

#### Демо

[http://imdim.github.io/ops](http://imdim.github.io/ops/)

#### Установка

Необходимо подключить jq библиотеку, jq.mousewheel и ops.min.js из дистрибутиваа.

#### Подключение

```js
$(".container").onePageScroll({
            selector: ".frame",
            startPage: 1,
            duration: 300,
            easing: 'ease-out',
            horizontal: false,
            keyboard: true,
});
```

#### Настройки

```js
selector: класс, id селектора страницы
startPage: стартовая страница
duration: скорость перелистывания
easing: параметр анимации перелистывания
horizontal: если true, то страницы будут скролиться горизонтально
keyboard: если true, то можно будет перелистывать с клавиатуры PageUP, PageDown, Up, Down, Left, Right
onInit: callback функция, которая выполнится при инициализации плагина
onChange: callback функция, которая выполнится при перелистывании
```

#### API
```js
$(".container").onePageScroll('scrolled') - возвращает значение 
  scrollTop (для horizontal: false) или 
  scrollLeft (для horizontal: true)
  
$(".container").onePageScroll('current') - возвращает номер текущей страницы

$(".container").onePageScroll('prev') - предыдущая страница
$(".container").onePageScroll('next') - следующая страница

$(".container").onePageScroll('first') - перелистываем к первой странице
$(".container").onePageScroll('last') - перелистываем к последней странице

$(".container").onePageScroll('anchor', '#page2') - перелистываем к странице с id: page2
```
