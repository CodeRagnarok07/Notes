
### Las funciones compose
son funciones que pueden combinar funciones,
es una function que recibe dos funciones y devuelve una function 

### funciones pura y funciones impuras
funciones puras son aquellas que son mandadas directamente al call stack ya que su retorno no cambia y son rápidas
funciones impuras son funciones tipo web api que pueden ser async 

### el shadowDOM
Es una caracteristica prinsipalmente usada por los web components, esta por encima del DOM, visualmente se muestra cuando se le señala y tapa el DOM original, Es un DOM que puede ser usado para modificarlo con js y CSS de manera cerrada y del resto del documento, 

### prototype

todos las variables son Objetos que heredan funciones de objeto Object
proto o prototype puede acceder a las funciones del elemento padre

```js
Object.prototype.newFunction = () => console.log("esta function puede ser usada en todos los elementos del js")

const newObjetoString = new Object("soy un string")

newObjetoString._proto_.newFunction()
newObjetoString._proto_.create_inline_for_this = ()=> console.log("function solo para este objeto string")
```
también prototype aguarda los métodos dependiendo del tipo de elemento


## Todo



Ámbito y Cierre (Scope and Closure):
Entender el alcance de las variables (local, global) y cómo los cierres permiten a las funciones acceder a variables fuera de su propio alcance.

Prototipos y Herencia:
Cómo funciona la herencia en JavaScript utilizando prototipos y cómo crear objetos y clases personalizados.

Manipulación del DOM:
Técnicas para seleccionar, modificar, y crear elementos en el Document Object Model (DOM).

Eventos del DOM:
Cómo manejar eventos en el DOM y cómo funcionan los eventos delegados.

Funciones de Orden Superior (Higher-Order Functions):
Funciones que toman otras funciones como argumentos o que devuelven funciones.

Asincronía y Promesas Avanzadas:
Profundizar en Promises, async/await, y patrones avanzados de manejo de asincronía.

 Módulos en JavaScript (ES6 Modules):
Cómo estructurar y organizar el código utilizando módulos en ES6.

Programación Funcional:
Principios de la programación funcional en JavaScript, incluyendo inmutabilidad, funciones puras, y composición de funciones.

Gestión de Estado:
Técnicas y patrones para manejar el estado de las aplicaciones, especialmente en aplicaciones de una sola página (SPA).

Testeo y Depuración:
Métodos y herramientas para probar y depurar el código JavaScript.

APIs del Navegador:
Uso de APIs nativas del navegador como Fetch, Local Storage, WebSockets, etc.

Seguridad en JavaScript:
Prácticas para asegurar el código JavaScript, incluyendo la prevención de ataques XSS y CSRF.

Optimizaciones de Rendimiento:
Técnicas para optimizar el rendimiento del código JavaScript y mejorar la eficiencia de las aplicaciones web.

JavaScript en el Servidor (Node.js):
Fundamentos de Node.js, incluyendo la creación de servidores, manejo de archivos, y comunicación con bases de datos.