![](/home/n.mendoza/Desktop/shuterstockimage.png) 
- Shutterstock (2020). JavaScript concept with hand on blue background. Recuperado de shutterstock.com


##Contenido
**1 Introducción**
**2 Variables**
**3 Estructuras condicionales**
**4 Bucles e Iteraciones**
**5 Links recomendados**


##1 . Introducción
Ejercicios Javascript para los estudiantes del grupo dwfs-bue-glob-4 de la carrera de Desarrollo web Full Stack. 

Este documento ha sido elaborado con markdown y su código fuente se encuentra en:
Última actualización: domingo, lunes, 25. mayo 2020 03:32 


Para la resolución de ejercicios pueden usar la consola del navegador || crear un documento HTML que incluya código javascript usando para ello la etiqueta *<script\>* o referenciandolo como un script externo.En  algunos casos le sugeriremos esta última opción. Ejemplo:

	<!DOCTYPE HTML>
	<html>
	
	<body>
		<p>Resolución ejercicio número x</p>
		
		<script>	
		   /* Dentro de estr bloque <*script*> escribimos todo nuestro código javascript*/
		   alert("Hola Mundo!");
		</script>
	</body>
	
	</html>
	


##2. Variables

![](/home/n.mendoza/Desktop/javascript_var.png) 
- Programminghunk(2020). Variables in Javascript. Imagen recuperada de: https://www.programminghunk.com/2020/02/variables-in-javascript.html


- Hemos aprendido a almacenar información utilizando variables. 
- Podemos imaginarnos la memoria de un ordenador como un panal enorme con millones y millones de cedas disponibles para almacenar información.

- En Javascript podemos almacenar diferentes tipos de valores en nuestras variables.
			
		var letra ="a"; // una letra;
		
		var frase = "No pienses que lo que se te dificulta es humanamente imposible; y si es humanamente posible, considéralo a tu alcance - Marco Aurelio"; // una frase
		
		var otraFrase = 'No hay nada que canse más a una persona que tener que luchar, no contra su propio espíritu, sino contra una abstracción. (todos los nombres -Saramago)'; // ¿comillas simples?
		
		var numeroFavorito = 7; // un número natural.
		
		var incrementoSalarial = 2.500; // un número decimal
		
		var deuda = -2334; // un número negativo
		
		var pi = 3.14159265358979323846; // número irracional "fixed"
		
		var buzzLightyear = Infinity;  // "Al infinito y más allá"
		
		var isAdmin = true; 
		
		var edad = null;
		

![](/home/n.mendoza/Desktop/Elementos/calentamiento.jpg) 

- Piense en una analogía de la vida real para explicar el concepto de variable en programación.
-  ¿Para qué sirve el operador **typeof**, **typeof()** en Javascript?
- ¿Para qué sirve **console.log() **?
¿Existe alguna diferencia entre declarar un **string** con comillas simples o dobles?
- Utilizando la consola del navegador imprima en consola el valor y el **tipo de dato** de cada una de las variables anteriores.


![](/home/n.mendoza/Desktop/Elementos/ejercicios.jpg) 

- Trabajando con variables.

1 - Declare dos variables: **writer** y **name**.
2 - Asigne el valor "Doris" a la variable **name**.
3 - Copie el valor de **name** en la variable **writer**
4 - Muestre el valor de **writer**, use una ventana emergente *alert*.  Esto deberìa mostar el nombre Doris.

- Eligiendo el nombre de nuestras variables.

 a - Declare una variable que almacene el nombre de su país. ¿qué nombre le pondria a esta variable?
 b - Declare una variable que almacene nuestro apellido. ¿qué nombre le pondríamos a nuestra variable?
 c - Declare una variable que almacene el estado de un producto, la variable solo debe indicarnos si hay stock o no. ¿qué tipo de dato nos conviene para esta situación?
 d - Crear una variable que almacene las ventas mensuales del supermercado cotto. ¿qué tipo de dato nos conviene para esta situación?
 
 - Realizando operaciones aritmeticas con variables.
 
 Dan tiene un ingreso fijo mensual de $5200 pesos + $2500 pesos que le aportan su familia. Adicionalmente, Dan se dedica a realizar eventos y cobra $1500 pesos por evento. 
Dan tiene gastos mensuales: Internet $1000 pesos y otros gastos fijos por $4800 pesos.
 

| Egresos      | Ingresos |
| ----------- | ----------- |
| $1000     |    $5200  |
| $4500     |    $2500    |
|             |    x1500    |
	   
Dan te pide por favor hagas un programa que le permita ingresar un número de eventos x y que le retorne el total de dinero que le queda después de egresos, asì puede analizar diferentes posibles escenarios al mes.

 1- Utilice **prompt** como entrada de datos para el número de eventos que Juan realice en un mes y almacene ese valor en una variable.
 2 - Declare variables para: total de egresos, total ingresos fijos, costo eventos
 3 - Devuelva la diferencia entre el total de Ingresos menos el total de egresos, tenga en cuenta la variable *eventos*.
 4 - Utilice un **alert/ventana emergente** para retornar la información que Juan necesita. Si Juan realiza 0 eventos, el programa debe retornar $2200, si Juan realiza 15 eventos al mes el programa debe retornar: $24.700. Compruebe.
 

	
![](/home/n.mendoza/Desktop/Elementos/infinito.jpg) 
Hasta ahora hemos venido declarando nuestras variables con la palabra reservada **var**, esta forma de declarar variables es la manera de hacerlo en la "vieja escuela". Todavía encontramos en muchos scripts esta forma de declarar variables lo que hace necesario empezar a trabajar con ellas y conocer su comportamiento antes de estudiar **let**.

 En javascript tenemos tres formas de declarar variables usando las palabras reservadas:

- **var** 
- **let**
- **const**

		var name = 'Nicolás';  // declarando variable - estilo "olds school"
		let name = 'Nicolás'; // declarando variable - javascript moderno
		
		const COLOR_ORANGE = '#FF7F00';  // declarando una constante, generalmente se escriben en mayúscula
		COLOR_ORANGE = '#F00'; // Esto dará un error, las constantes no se pueden reasignar / cambiar su valor en tiempo de ejecución.

**var** y **let** son similares pero **var** generalmente no se usa en proyectos javascript modernos, **var** actua como una especie de variable global.

- Refactorizando nuestro código.

*En la programación de computadoras y el diseño de software, la refactorización de código es el proceso de reestructurar el código de computadora existente (cambiar la factorización) sin cambiar su comportamiento externo.* 

1 - Hagamos un poco de *code refactor* al programa de "Dan", reemplaemos nuestras declaraciones **var** por **let**. Comprobemos que efectivamente esto no cambia el comportamiento de nuestro programa.
2 - Investigue las diferencias entre **let** y **var**.
3 - Investigue el método **.toFixed()** y trate de aplicarlo en valores decimales, por ejemplo en las variables de egreso e ingreso del programa de "Dan".

	<!DOCTYPE HTML>
	<html>
	
	<body>
		<p>Resolución ejercicio número x</p>
		
		<script>	
		   let ingreso = 45.234521;
		   alert(ingreso.toFixed(2));
		</script>
	</body>
	
	</html>
4 - Utilice utlizar constantes para los valores fijos tales cómo los ingresos fijos mensuales y el precio de cada evento.

5 - Investigar el tipo de dato ** BigInt **y  qué navegadores lo soportan.

	/* 
         - En javascript el tipo de dato "number" no puede representar valores mayores a 2 elevado a 53. No más de 16 digitos decimales. 
         - Esto no es mayor problema trabajando de lado de front-End. 
         - En backend avanzado algunas veces necesitamos almacenar números realmente grandes, por ejemplo para cuestiones de criptografía, precisión, etc. */	
	   const bigInt = 1234567890123456789012345678901234567890n;


##3. Estructuras condicionales.	

Muchas veces necesitamos realizar diferentes acciones basadas en condiciones, por ejemplo, podemos pensar en programar un juego de "adivinanza" en dónde:
 - SI el usuario adivina la edad del persona Homero Simpson mostramos un **alert** felicitandolo, caso contrario mostraremos un **alert** indicando que el usuario se ha equivocado. 
 
 
	<!DOCTYPE HTML>
	<html>
	
	<body>
		<p>Resolución ejercicio número x</p>
		
		<script>	
		   const homersAge = 39; //  Edad del personaje Homero Simpson
		   let response = prompt('¿Qué edad tiene Homero Simpson?');
		   
		   if(response === homersAge){
		   	alert('¡Muy bien! Homero tiene' + response + ' años.');
		   }
		   else {
		     alert('No, Homero no tiene ' + response + ' años.');
		   }
		</script>
	</body>
	
	</html>
	
- Además de **if** y la claúsula **else** también aprendimos a usar **switch**.  

- Imaginemos un escenario en dónde tengamos que aplicar más de tres condicionales **if**, por ejemplo tenemos un programa que dado el *nombre* de un *país* nos retorne el número de muertes a causa del COVID-19.

 
		<!DOCTYPE HTML>
		<html>
		
		<body>
			<p>Ejemplo usando If - Else If - Else</p>
			
			<script>			   
			  let pais = prompt('Escriba País a consultar'); // país ingresado por el usuario.
			  pais = pais.toUpperCase(); // normalizamos los datos ingresados por el usuario, pasamos todo a mayúsculas.
			   
			   if (pais ==="BRAZIL"){
			   	alert("22.666 deaths");
			   }
			   else if(pais ==="RUSSIA"){
			   	alert("3.633 deaths");
			   }
			   else if(pais ==="ITALIA"){
			   	alert("32.877 deaths");
			   }
			   else if(pais ==="FRANCIA"){
			   	alert("28.370 deaths");
			   }
			   else if(pais ==="CHINA"){
			   	alert("4.638 deaths");
			   }
			    else if(pais ==="ARGENTINA"){
			   	alert("456 deaths");
			   }
			     else if(pais ==="CHILE"){
			   	alert("761 deaths");
			   }
			   else {
			     alert('No tenemos datos para '+ pais + '. Consulte el sitio web: https://coronavirus.jhu.edu/map.html ');
			   }
			</script>
		</body>
		
		</html>
- Podemos ver en el ejemplo anterior un código difícil de leer y muy repetitivo, en la práctica existe una mejor forma de programar algo así pero de momento enfoquemonos a mejorarlo un poquito más usando la estructura **switch**
	
	<!DOCTYPE HTML>
			<html>
			
			<body>
			<p>Ejemplo usando switch</p>
			
			<script>
			    let pais = prompt('Escriba País a consultar').toUpperCase();
			
			    switch (pais) {
			        case 'BRAZIL':
			            alert("22.666 deaths");
			            break;
			            
			        case 'RUSSIA':
			            alert("3.633 deaths");
			            break;
			            
			        case 'ITALIA':
			            alert("32.877 deaths");
			            break;
			            
			        case 'FRANCIA':
			            alert("28.370 deaths");
			            break;
			            
			        case 'CHINA':
			            alert("4.638 deaths");
			            break;
			            
			        case 'ARGENTINA':
			            alert("456 deaths");
			            break;
			            
			        case 'CHILE':
			            alert("761 deaths");
			            break;
			            
			        default:
			            alert('No tenemos datos para ' + pais + '. Consulte el sitio web: https://coronavirus.jhu.edu/map.html');
			    }
			</script>
			</body>
			
			</html>

![](/home/n.mendoza/Desktop/Elementos/calentamiento.jpg) 

- En el primer ejercicio utilizamos una sentencia **else if** (else + if). Cambie las sentencias **else if** por simples **if** y explique qué pasa. ¿cuál es la diferencia en usar un **if** vs **else if** ? ¿por què **else if** depende siempre de una sentencia inicial **if**?

-  En el segundo ejercicio ¡qué ocure si omitimos las sentencias **break**? Intentelo. Ve alguna "parecido" entre **else if **y **break** ?
- ¿Sabías que puedes agrupar diferentes **cases** que compartan el mismo código a ejecutar? Intenta lo siguiente, fijate en los casos de "Argentina, Chile y Colombia'. Explica qué ocurre.
	
					    let pais = prompt('Escriba País a consultar').toUpperCase();
					
					    switch (pais) {
					        case 'BRAZIL':
					            alert("22.666 deaths");
					            break;
					            
					        case 'RUSSIA':
					            alert("3.633 deaths");
					            break;
					            
					        case 'ITALIA':
					            alert("32.877 deaths");
					            break;
					            
					        case 'FRANCIA':
					            alert("28.370 deaths");
					            break;
					            
					        case 'CHINA':
					            alert("4.638 deaths");
					            break;
					            
					        case 'ARGENTINA':
					        case 'CHILE':
					        case 'COLOMBIA':
					            alert("761 deaths en Argentina, Chile y COlombia");
					            break;
					            
					        default:
					            alert('No tenemos datos para ' + pais + '. Consulte el sitio web: https://coronavirus.jhu.edu/map.html');
					    }

![](/home/n.mendoza/Desktop/Elementos/ejercicios.jpg) 

-  Reescribe el siguiente programa reemplazando **switch** por condicionales **if**:

		<!DOCTYPE HTML>
		<html>
		
		<body>
		<p>Ejemplo usando switch</p>
		
		<script>
		    /*
		    El programa retorna el nombre del motor Javascript usado por el navegador. Recuerde el motor es el encargado
		    de leer / interpretar /ejecutar nuestro código Javascript.
		    * */
		    let browser = prompt('Escriba el browser a consultar').toLowerCase();
		
		    switch (browser) {
		        case 'edge':
		            alert( "Edge usa el motor JS: Chakra" );
		            break;
		        case 'chrome':
		            alert( "chrome usa el motor JS: V8" );
		            break;
		        case 'firefox':
		            alert('Firefox usa el motor JS: SpiderMonkey');
		            break;
		        case 'safari':
		            alert('Safari usa el motor JS: JavascriptCore');
		            break;
		        case 'opera':
		            alert( 'Opera hasta el 2010 tenía el mejor motor JS (carakan engine) y era el navegador más rápido de Internet. Actualmente usa V8' );
		            break;
		        default:
		            alert( 'Desconozco el motor JS para el navegador' + browser);
		    }
		</script>
		</body>
		
		</html>	
		
- Reescriba el siguiente programa, reemplaze los **if** por un **switch**:

		<!DOCTYPE HTML>
		<html>
		
		<body>
		<p>Ejemplo usando switch</p>
		
		<script>
			let vowel = prompt('vocal?', '').toLowerCase();
			    if (vowel == 'a') {
					alert('A');
			    }
			    if (vowel == 'e') {
					alert('E');
			    }
			    if (vowel === 'i' || vowel === 'o') {
					alert('I, O');
			    }
			    if (vowel === 'u') {
					alert('U');
			    }
			    if (vowel === '') {
					alert("No es una vocal");
			    }
		</script>
		</body>
		
		</html>	

- Adicional. ¿Para que sirve el segundo argumento en la función **prompt** ""? **prompt**("vocal", **"segundoArgumento"**);

![](/home/n.mendoza/Desktop/Elementos/infinito.jpg) 

- Una clínica privada de la ciudad de buenos aires, ha decidido usar pasillos independientes para cada una de las especialidades médicas basado en la edad del paciente, lo menores de edad necesitar ir acompañados de un adulto quién sera el que digite la fecha de nacimiento del menor.

Las condiciones son las siguientes:
- Si el paciente tiene menos o un año de vida debe ser remitido al pasillo de Neonatología.
- Si el paciente tiene más de un año de vida y menos de 16 años, remitir entonces al pasillo de Pediatría.
- Si el paciente tiene 16 o màs de 16 años pero menos de 70 años, entonces remitir al pasillo de clínica médica.
- Si el paciente tiene 70 años de vida o más, entonces remitirlo al pasillo geriátrico.

1 -  El input debe ser la fecha de nacimiento del paciente.
2- El output debe ser un Alert con el nombre de el pasillo al que debe ir el paciente.

- Bonus: En la práctica la sub especialidad de neonatología se encarga de recién nacidos o niños hasta un mes de vida.  Te animas a hacer un programa que sea capaz de difenciar este caso especifico? - Necesitaràs trabajar con objetos date.
##5. Links recomendados	

Esta lista de links puede ayudarle en su proceso de aprendizaje. La mayoría de links apuntan a temas que aún no hemos visto, asi que no se preocupen. La información está organizada de manera que puedan consultarla a medida que vayan avanzando en su proceso de aprendizaje.


##Conocimiento básico
| Modalidad      | Oportunidad de Aprendizaje |
| ----------- | ----------- |
| Lectura      |    [Javascript básico](https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/JavaScript_basics)    |
| Lectura      |    [Programación orientada a objetos en Javascript](https://developer.mozilla.org/es/docs/Learn/JavaScript/Objects/Object-oriented_JS)    |
| Lectura      |    [Herencia y Prototypes JS](https://developer.mozilla.org/es/docs/Web/JavaScript/Herencia_y_la_cadena_de_protipos) 
| Lectura      |    [Async programming: Promises](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Promise)    |
| Lectura      |    [Async Functions](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Sentencias/funcion_asincrona)    |
| Lectura      |    [Tipos de datos y estructuras en javascript](https://developer.mozilla.org/es/docs/Web/JavaScript/Data_structures)    |
| Lectura      |    [Closures](https://developer.mozilla.org/es/docs/Web/JavaScript/Closures)    |
| Lectura      |    [Closures and references](https://bonsaiden.github.io/JavaScript-Garden/#function.closures)    |
| Lectura      |    [Tipos de datos y estructuras en javascript II](https://bonsaiden.github.io/JavaScript-Garden/#types)    |
| Udemy      |    [Javascript Avanzado](https://globant.udemy.com/course/javascript-advanced/)    |
| Lectura      |    [Expresiones regulares](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)    |
| Udemy      |    [Regular expresions course with exercises](https://globant.udemy.com/course/the-complete-regular-expressions-course-with-exercises-for-beginners/)    |
| Udemy      |    [Javascript básico](https://globant.udemy.com/course/modern-javascript/)    |
| Libro      |    [Javascript Avanzado](https://leanpub.com/javascriptallongesix/read)     |	   
		   
##Programación orientada a objetos

| Modalidad      | Oportunidad de Aprendizaje |
| ----------- | ----------- |
| Lectura      |    [Proramación orienta a objetos Principiantes](https://developer.mozilla.org/es/docs/Learn/JavaScript/Objects/Object-oriented_JS)    |
| Lectura      |    [Herencia y Prototypes JS](https://developer.mozilla.org/es/docs/Web/JavaScript/Herencia_y_la_cadena_de_protipos) 
| Udemy      |    [Javascript Avanzado](https://globant.udemy.com/course/javascript-advanced/)    |

		   
##Programación estructurada
| Modalidad      | Oportunidad de Aprendizaje |
| ----------- | ----------- |
| Lectura      |    [Javascript básico](https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/JavaScript_basics)    |
| Udemy      |    [Javascript Avanzado](https://globant.udemy.com/course/javascript-advanced/)    |
| Libro      |    [Javascript Avanzado](https://leanpub.com/javascriptallongesix/read)     |	   

##Programación funcional
| Modalidad      | Oportunidad de Aprendizaje |
| ----------- | ----------- |
| Lectura      |    [Programación funcional](https://github.com/MostlyAdequate/mostly-adequate-guide)    |
| Libro      |    [Javascript Avanzado](https://leanpub.com/javascriptallongesix/read)     |	   

##Programación reactiva
| Modalidad      | Oportunidad de Aprendizaje |
| ----------- | ----------- |
| Lectura      |    [Async programming: Promises](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Promise)    |




#Desarrollo web Full Stack

Mentores:

- Julian Drets
- Nicolás Mendoza: https://github.com/nicolasmendoza


