# TRABAJO EN CASA PHP
****
****
****
**_INVESTIGAR ACERCA DE LAS FUNCIONES EN PHP_**  
1. **Desarrollo de sitios web** dinámicos PHP permite crear páginas 
web dinámicas que pueden interactuar con bases de datos y adaptar 
su contenido según las necesidades del usuario.  
2. **Manejo de formularios** PHP facilita la recopilación y procesamiento 
de datos enviados a través de formularios HTML.
3. **Conexión con bases de datos** PHP se integra fácilmente con sistemas de 
gestión de bases de datos como MySQL, PostgreSQL, SQLite, Oracle, 
entre otros, permitiendo almacenar y recuperar información.
4. **Manipulación de archivos** PHP puede crear, leer, escribir y modificar archivos 
en el servidor, lo que es útil para la gestión de contenido y logs.
5. **Envío de correos electrónicos** PHP incluye funciones para enviar correos
electrónicos, lo que es útil para notificaciones, confirmaciones y 
newsletters.
6. **Seguridad** PHP incluye funciones para validar y sanitizar datos, 
proteger contra inyecciones SQL, y gestionar la seguridad en general.
7. **Frameworks y CMS PHP** es la base de muchos frameworks populares 
(como Laravel, Symfony, y CodeIgniter) y sistemas de gestión de 
contenido (CMS) como WordPress, Joomla, y Drupal.
****
**_¿CUAL ES SU ESTRUCTURA?_**  
R/= La estructura básica de PHP incluye etiquetas, variables, 
funciones, operadores, estructuras de control, tipos de datos, 
constantes, y comentarios.  
- **Estructuras de control:** Permiten que el script de PHP responda de 
manera diferente a distintas entradas o situaciones. Permiten 
crear condicional en el código y ejecutar diferentes bloques de código 
en función de las expresiones que evalúan. Ejemplos de estructuras 
condicionales son if, if else y elseif.
- **Sentencias:** Un script PHP está construido según una serie de sentencias. 
Una sentencia puede ser una asignación, una llamada de función, un ciclo, 
una sentencia condicional o incluso una sentencia que no hace nada 
(una sentencia vacía). Las sentencias generalmente finalizan con un 
punto y coma.
- **Scripts PHP:** Un script PHP comienza con <?php y termina con ?>. 
La extensión de archivo predeterminada para los archivos PHP es 
" .php ". Un archivo PHP normalmente contiene etiquetas HTML y 
algún código de script PHP.
****
**_SINTAXIS CORRECTA_**
* Para definir una variable, se antepone el signo $$$ seguido del nombre de la variable. Por ejemplo, $$nombre, $edad. 
* Para imprimir un mensaje en pantalla, se puede usar echo. 
* Para hacer un salto de línea, se escribe \n al final del texto. 
* Para concatenar, se pueden colocar las variables dentro del mensaje que se quiere imprimir, pero esto solo funciona si se usan comillas dobles. 
* Para definir un string puro (cadena de texto), se debe especificar el valor entre comillas simples. 
* Para indicar un número o un valor booleano, se hace sin comillas. 
* Un script de PHP se puede colocar en cualquier parte de un documento y empieza con <? php y termina con ?>.
****
**_CUANDO USARLAS_**   
R/=  La estructura de PHP se basa en sentencias, que pueden ser asignaciones, 
llamadas de funciones, ciclos, sentencias condicionales, entre otras. 
La sintaxis básica de PHP incluye: 
* Uso de llaves ({} ) para estructurar el código.  
Ejemplo: < ?php if (true) { echo "Dentro de las llaves."; } ? >   


* Nombres de variables que comienzan con un signo (DOLLAR).   
  Ejemplo: < ?php $$nombre = "Juan"; echo $nombre; ? >  
  

* Declaraciones que terminan con un punto y coma (;).  
Ejemplo: < ?php echo "Hola, mundo!"; ? >  
  

* Uso de etiquetas HTML para encerrar el código PHP en páginas web.   
Ejemplo: < !DOCTYPE html>
< html >
< body >
    < p > < ?php echo "Hola desde PHP"; ?>< / p >
< / body >
< / html >

****
****  
****
## ARRAY'S  
### INVESTIGACIÓN ACERCA DE LOS ARRAY

`TIPOS DE ARRAY, CON EJEMPLO DE CADA UNO`
1. Array Indexado: Los elementos se acceden mediante un índice numérico. Se accede mediante el índice numérico.  
Ejemplo: $$frutas = array("Manzana", "Banana", "Cereza");
   echo $frutas[0); // Salida: Manzana  

2. Array Asociativo: Los elementos se acceden mediante una clave de tipo string. Se accede mediante la clave.  
Ejemplo: $$edades = array("Juan" => 25, "Ana" => 30, "Carlos" => 35);
echo $edades["Ana"); // Salida: 30     

3. Array Multidimensional: Un array que contiene otros arrays. Se accede mediante múltiples índices o claves.   
Ejemplo: $$personas = array(
   "Juan" => array("edad" => 25, "ciudad" => "Madrid"),
   "Ana" => array("edad" => 30, "ciudad" => "Barcelona")
   );
   echo $personas["Juan")["ciudad"); // Salida: Madrid

`COMO  MODIFICAR ARRAY, AGREGAR ELEMENTOS Y ELIMINARLOS`
- Agregar Elementos:   
  $frutas[] = "Durazno"; // Agrega al final del array
  $$edades["Pedro") = 40; // Agrega un nuevo elemento al array asociativo
- Elimnar Elementos:  
  unset($$frutas[1)); // Elimina el elemento con índice 1 unset($edades["Ana")); // Elimina el elemento con clave "Ana"
  

`COMO RECORRER ARRAYS USANDO FOREACH, FOR, ARRAY ASOCIATIVO`  
**Foreach**   
- Ejecuta una función para cada elemento de un array. 
- Recorre cada par clave-valor de un array asociativo. 
- En cada iteración, el valor del elemento actual se asigna a una variable. 
- En PHP 5, el puntero interno del array se coloca automáticamente en el primer elemento.  

**For**   
- Se puede usar para recorrer matrices asociativas 

**Arrays asociativos** 
- Son arrays cuyos keys son strings con valores personalizados. 
- Las keys son sensibles a mayúsculas, minúsculas y acentos. 
- Se puede acceder a los arrays asociativos utilizando comillas dentro de los corchetes o sin utilizarlas.  

`COMO BUSCAR ELEMENTOS  EN UN ARRAY`
* **arr.indexOf(item, from)** Busca el elemento item a partir del índice from y devuelve el índice donde se encuentra. Si no se encuentra, devuelve -1.
* **arr.includes(item, from)** Busca el elemento item a partir del índice from y devuelve true si se encuentra.
* **filter** Devuelve un nuevo array con los elementos que cumplen con la función callback.
* **includes()** Verifica si un elemento existe dentro de un arreglo o si un substring existe dentro de una cadena de texto.
* **Puedes usar el método filter** para buscar un elemento en un array de arrays. También puedes recorrer cada array dentro del array padre usando un for.
  

`COMO MEZCLAR VARIOS ARRAY`  
* Se puede usar la función array_merge() para anexar los valores de un array al final de otro. 
* También se puede usar el operador de unión de arrays (+) para anexar elementos de un array al final de otro sin sobrescribir los elementos del primero.

****
****
****
### TAREA HECHA POR: MARTHÍN JOSÉ CONTRERAS RODRÍGUEZ