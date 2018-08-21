Начало
	display: grid - применяется к детям первого уровня

Ширина блока

	/*grid-template-columns: 300px 300px 300px;*/
	/*grid-template-columns: 1fr 2fr 1fr 200px;*/
	/*grid-template-columns: repeat(2, 1fr 2fr);*/
	/*grid-template-columns: 200px repeat(2, 1fr 2fr);*/
	/*grid-template-columns: minmax(100px, 300px) 1fr 1fr;*/
	/*grid-template-columns: repeat(auto-fill, minmax(300px, 2fr));*/
	/*grid-template-columns: repeat(auto-fit, minmax(100px, 2fr));*/
	/*grid-template-columns: repeat(4, 1fr);*/
_________________________________________________________________________________________________________________________

Высота ряда

	/*grid-template-rows: 100px 100px;*/
	/*grid-template-rows: 200px 100px 100px;*/

_________________________________________________________________________________________________________________________


Высота всех блоков

	/*grid-auto-rows: 50px;*/
	/*grid-auto-rows: minmax(100px, auto);*/
	
_________________________________________________________________________________________________________________________

	
Высота и ширина всех блоков (сокрашенно, grid-template-columns and grid-template-rows)

	grid-template: minmax(100px, auto) / repeat(4, 1fr);

_________________________________________________________________________________________________________________________

Отступы

	/*grid-column-gap: 10px;
	grid-row-gap: 10px;*/
	grid-gap: 10px;

_________________________________________________________________________________________________________________________

Расположение блоков

	/*grid-auto-flow: column;*/
	/*grid-auto-flow: row;*/
  
_________________________________________________________________________________________________________________________

Выравнивание блоков

	/*align-items: center;
	justify-items: center;*/

_________________________________________________________________________________________________________________________
		
Выравнивание блока (применяется к ребенку display:grid)

		/*align-self: start;
		justify-self: center;*/

_________________________________________________________________________________________________________________________

Задает блоку сдвиг и какое кол-во фракций он будет занимать
		/*grid-column-start: 1;
		grid-column-end: -1;*/
		grid-column: 1 / -1; 
		grid-row: 1 / -1;

_________________________________________________________________________________________________________________________

Меняем расположение блков, давая им оперделенные имена

	grid-template-areas:   /*Выведет все блоки в ряд*/
		"header"
		"section"
		"aside"
		"footer";

	grid-template-areas:  /*Выведет все блоки в расположение, котором указанно*/
			"header header"
			"aside section"
			"aside footer";
