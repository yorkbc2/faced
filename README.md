# FaceDesign - CSS Material Design Framework

[Классы] #Классы

## Что это?

FaceDesign - это CSS фреймворк, который помогает создавать сайты в стиле Google Material Design. 

Сегодня, Material Design есть одним из самых популярных стилей визуализации сайтов. Он интересен тем, что создает дополнительное пространство тенями, которые выглядит как-будто объемным. 
## Как с ним работать?

В FaceDesign уже описаны все классы, которые нужны для роботы с стилизацией. Подобраны лучшие цвета и собрано все самое лучшее с этой сферы. 
Все классы имеют префикс fc-*

### Установка
Для установки фреймворка, Вам необходимо скачать файл 'face.css'. Далее, нужно подключить его в Вашем HTML файле. 
```html
	<head>
		<link rel='stylesheet' href='face.css' />
	</head>
```

## Классы

## Колонки

### fc-container	
Блок, который нужен для правильного отображения колонок.
```html
		<div class="fc-container">
			<div class="fc-l-6"></div>
			<div class="fc-l-6"></div>
		</div>
```
### fc-*

Класс, который создает колонки. Имеет ряд доступных размеров колонок : от 1 до 12. 

```html
		<div class='fc-3'></div>
		<div class='fc-9'></div>
```

### fc-offset-*
Класс, который создает пространство слева от блока. Взаимодействует с колонками.

```html
<div class='fc-offset-2 fc-8'></div>
```

### fc-l-*
Класс, который создает колонки больших размеров. Существует несколько размеров колонок. От fc-l-1 до fc-l-12. 
```html
		<div class='fc-l-6'>
			Welcome
		</div>
		<div class='fc-l-6'>
			to our site
		</div>
```
### fc-m-*
Повторяет то, что делает предыдущий класс, только рассчитан для меньших экранов. (до 1240)
```html
		<div class="fc-m-4"></div>
		<div class="fc-m-4"></div>
		<div class="fc-m-4"></div>
```
### fc-sm-*
Продолжает действия остальных елементов-колонок, только для экранов планшетов и телефонов. (до 720)

```html
		<div class="fc-m-12"></div>
```

### fc-xs-*
Последний вид колонок. Для экранов смартфонов и старых телефонов (до 480)
```html

		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>
```

## Навигатор ( alpha version )

### fc-nav
Для создания навигатора, блоку необходимо указать класс .fc-nav. Он уже создаст стилизированый навигатор. Далее, в блоке нужно создать список, который сразу превратиться в ячейки навигатора. 
```html
<div class='fc-nav'>
<ul>
<li><a href='#'>Main</a></li>
<li><a href='#'>FAQ</a></li>
<li><a href='#'>Face</a></li>
</ul>
</div>
```

Также, навигатор можно менять с помощью уже созданных классов, например fc-bgc :


```html
<div class='fc-nav fc-bgc red'>
<ul>
<li><a href='#'>Main</a></li>
<li><a href='#' class='fc-color black'>FAQ</a></li>
<li><a href='#'>Face</a></li>
</ul>
</div>
```

### *.fc-fixed

Навигатор также можно фиксировать : 
```html
<div class='fc-nav fc-fixed'>/.../</div>
```

## Полноэкранные блоки

### fc-mid
Полноэкранный блок с фоном-картинкой, который сейчас в моде. Имеет эффект параллакса при добавлении класса 'parallax'
```html

		//Без эффектов
		<div class="fc-mid">
			//.....
		</div>

		//Эффект параллакса
		<div class="fc-mid parallax">
			//.....
		</div>
```





### fc-filter
Обычно используется в блоке 'fc-mid'. Класс создает фильтр с цветом, который по стандарту является серым. Можно выбрать другой цвет с помощью классов: 
* red
* purple
* green
* blue
* yellow
* cyan
```html

		<div class="fc-mid">
			<div class="fc-filter red">
				//......
			</div>
		</div>
```

### fc-header
Чтобы создать заголовок страницы на фоне картинки с фильтром, можна использовать класс 'fc-header'. Он центрирует блок и стилизирует заголовок.
```html
		<div class="fc-mid">
			<div class="fc-filter cyan">
				<div class="fc-header">
					<h1>Hello world</h1>
				</div>
			</div>
		</div>
```
## Доп. материал

### fc-item
Элемент, который создан для стилизации блоков с новостями, постами, прочем... Сам элемент имеет не статическую высоту

```html
<div class='fc-item'>/.../</div>
```

### fc-item-static
Элемент, который уже имеет набор свойств, которые неизменные

```html
<div class='fc-item-static'>/.../</div>
```

### fc-item-full
Элемент, который имеет ширину прородителя.

```html
<div class='fc-item-full'>/.../</div>
```

### fc-color
Класс, который задает цвет текста. Имеет список встроенных цветов :
* red
* green
* blue
* purple
* white
* black
* orange
* tr (transparent)
```html

		<p class='fc-color red'>Welcome to Face CSS Framework</p>
```

### fc-bgc
Класс, который задает фон елемента. Имеет список встроенных цветов : 
* red
* green
* blue
* white
* black
* orange
* yellow
* purple

```html
		<div class='fc-bgc orange'>Welcome to Face CSS Framework</div>
```

### fc-btn, fc-btn *
Класс, который стилизирует кнопки. Имеет уже заданые тени, цвета, хотя может меняться. 
Список доступных цветов :
* red
* green
* blue
* yellow
* yellow-white
* purple
* underline

```html
		<button class='fc-btn green'>Green Button</button>

```

#### .fc-btn underline

Эффект для кнопки. При наводке появляется нижнее подчеркивание, которое плавно уходит.

```html
<button class='fc-btn green underline'>Underline Button</button>
```

### fc-bq
Класс, который стилизирует текст как цитату
```html
		<div class='fc-bq'>To be or not to be...</div>
```

### fc-t*
Позиционирование текста с помощью text-aligin. Значения, которые принимает класс :
* fc-tr ( right )
* fc-tl ( left )
* fc-tc ( center )


## О фреймворке

#### Автор: Alex Yorke / yorkbc2 / <yorkbc2@gmail.com>
#### Версия: 0.3
#### Next beta version: 0.5
#### Next stable version: 0.2
#### Название: Face. Google Material Design CSS Framework
