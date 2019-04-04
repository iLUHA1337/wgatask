Сборка для Windows:
====
1. Установить Cmake (3.12+), SFML(sfml-dev.org) (2.5+): внимательно прочитайте туториал по установке(про MinGW(sjlj)).
2. Открыть консоль в директории с проектом.
	cd build 
	cmake -G "MinGW Makefiles" ../src
	mingw32-make	
3. Если всё сделано верно, то в каталоге build появится исполняемый файла WGA_TASK.exe
4. При желании перенести исполняемый файл в иное место, это следует делать толко со всеми файлами, находящимися в исходной директории.
5. Приложение готово к запуску.
5.1 Возможные ошибки: неподходящая версия комплятора/SFML, пути к последним не указаны в переменной среды PATH, не установлен mingw32-make(это делается в mingw-setup), отсутствую библиотеки/каталог с ресурами в build.
----
Использование:  
====
	Подробное описание задания можно прочитать здесь: https://wgacademy.ru/forums/forum/15-тестовые-задания/
	Над полем расположены 3 кружка разных цветов, требуется переместить блоки на поле так,  
	чтобы под каждым кругом определенного цвета находились только блоки того же цвета, что и круг. 
**Размер окна можно масштабировать.**   



Управление:
====
	Для того чтобы выбрать блок нажмите по нему ЛКМ, при нажатии на соседнюю* свободную клетку данный блок переместиться в неё. 
	Если вы передумали перемещать блок, то чтобы отменить свой выбор:
		*А. Нажмите ЛКМ на свободное место за пределами поля.
		*Б. Нажмите ЛКМ на сам блок. 
		*В. Нажмите ЛКМ на соседний* занятый блок.
		*Г. Нажмите ПКМ в любое место. 
	*Соседний - по вертикали или горизонтали (не по диагонали).
	При завершении игры появляется спрайт со следующей информацией:
	Для выхода нажмите ESCAPE.
	Чтобы начать игру заново нажмите R.
