# relogio

link : https://hilarious-zuccutto-9190d7.netlify.app

<h3>Principales funciones hechas</h3>
<ul>
<li>
Obtención de Elementos del DOM:

const horas = document.getElementById("horas");
const minutos = document.getElementById("minutos");
const segundos = document.getElementById("segundos");
Estas líneas de código obtienen referencias a elementos del DOM con los identificadores "horas", "minutos" y "segundos" respectivamente. Presumiblemente, estos elementos HTML se utilizan para mostrar la hora actual en la página.</li>

<li>Función time y setInterval:

const relogio = setInterval(function time() {...}, 1000);
Se utiliza setInterval para ejecutar la función time cada 1000 milisegundos (1 segundo). La función time se encarga de obtener la hora actual del sistema mediante el objeto Date y actualizar los elementos del DOM con los valores de horas, minutos y segundos formateados.</li>

<li>Obtención de la Hora Actual:

let dateToday = new Date();
let hr = dateToday.getHours();
let min = dateToday.getMinutes();
let s = dateToday.getSeconds();
Estas líneas de código crean un objeto Date para obtener la fecha y hora actual, y luego extraen las horas, minutos y segundos de ese objeto.</li>

<li>
Formateo de Números de un Solo Dígito:

if (hr < 10) hr = "0" + hr;
if (min < 10) min = "0" + min;
if (s < 10) min = "0" + s;
Estas líneas de código verifican si las horas, minutos o segundos son menores que 10, y si es así, les agrega un cero al principio para asegurar que siempre tengan dos dígitos.</li>

<li>Actualización de los Elementos del DOM:

horas.textContent = hr;
minutos.textContent = min;
segundos.textContent = s;
Estas líneas de código actualizan el contenido de los elementos HTML (probablemente etiquetas span o div) con los valores formateados de horas, minutos y segundos.</li>

</ul>
