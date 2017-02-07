# FaceDesign - CSS Material Design Framework

## Что это?

FaceDesign - это CSS фреймворк, который помогает создавать сайты в стиле Google Material Design. 

Сегодня, Material Design есть одним из самых популярных стилей визуализации сайтов. Он интересен тем, что создает дополнительное пространство тенями, которые выглядит как-будто объемными.

## Как с ним работать?

В FaceDesign уже описаны все классы, которые нужны для роботы с стилизацией. Подобраны лучшие цвета та собрано все самое лучшее с этой сферы.

## Классы

### fc-container	
	Блок, который нужен для правильного отображения колонок.

		<div class="fc-container">
			<div class="fc-l-6"></div>
			<div class="fc-l-6"></div>
		</div>

### fc-l-*
	Класс, который создает колонки больших размеров. Существует несколько размеров колонок. От fc-l-1 до fc-l-12. 

		<div class='fc-l-6'>
			Welcome
		</div>
		<div class='fc-l-6'>
			to our site
		</div>

### fc-m-*
	Повторяет то, что делает предыдущий класс, только рассчитан для меньших экранов. (до 1240)

		<div class="fc-m-4"></div>
		<div class="fc-m-4"></div>
		<div class="fc-m-4"></div>

### fc-sm-*
	Продолжает действия остальных елементов-колонок, только для экранов планшетов и телефонов. (до 720)


		<div class="fc-m-12"></div>


### fc-xs-*
	Последний вид колонок. Для экранов смартфонов и старых телефонов (до 480)


		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>
		<div class="fc-xs-3"></div>


### fc-mid
	Полноэкранный блок с фоном-картинкой, который сейчас в моде. Имеет эффект параллакса при добавлении класса 'parallax'


		//Без эффектов
		<div class="fc-mid">
			//.....
		</div>

		//Эффект параллакса
		<div class="fc-mid parallax">
			//.....
		</div>


### fc-btn, fc-btn *
	Класс, который стилизирует кнопки. Имеет уже заданые тени, цвета, хотя может меняться. 
	Список доступных цветов :
	* red
	* green
	* blue
	* yellow
	* yellow-white
	* purple

		<button class='fc-btn green'></button>



### fc-filter
	Обычно используется в блоке 'fc-mid'. Класс создает фильтр с цветом, который по стандарту является серым. Можно выбрать другой цвет с помощью классов: 
	* red
	* purple
	* green
	* blue
	* yellow
	* cyan


		<div class="fc-mid">
			<div class="fc-filter red">
				//......
			</div>
		</div>


### fc-header
	Чтобы создать заголовок страницы на фоне картинки с фильтром, можна использовать класс 'fc-header'. Он центрирует блок и стилизирует заголовок.

		<div class="fc-mid">
			<div class="fc-filter cyan">
				<div class="fc-header">
					<h1>Hello world</h1>
				</div>
			</div>
		</div>


### fc-block
	Блок, который служит для создания полноэкранных елементов.

		<div class='fc-block'></div>


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


		<p class='fc-color red'>Welcome to Face CSS Framework</p>


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

		<div class='fc-bgc orange'>Welcome to Face CSS Framework</div>
