# DW_Ejecitacion_Modulos-Requerimientos
  En este repositorio propio de las actividades de desarrollo web del club de programacion de la EPET N°14, Neuquen (Argentina).
  Contendra una serie de modulos propios de un proyecto JS, muchos estaran incompletos y tendran indicaciones acerca de su funcionalidad.
  Tener a bien que las descripciones de cada modulo estaran comentadas, y seran parte del esquema de requerimientos:
  
  Modulo (requiere) => (es requerido) Modulo (require) => (es requerido) Modulo
  
  De manera que al indicar "de este modulo sera requerida la funcionalidad, bajo el nombre de suma, para operar matematicamente una suma algebraica de dos parametros, retornando el resultado de esta." se debera interpretar que el modulo en el que se encuentra dicha leyenda, se debera generar una funcion exportable modular, que toma dos parametros y retorna el resultado.
  
  module.exports.suma = function(parametro1, parametro2){
   return parametro1 + parametro2;
  }
  //o su equivalente en ES6
  module.exports.suma = (parametro1, parametro2) => parametro1 + parametro2;
  
  Y en el caso de que se indique "este modulo requerira la funcionalidad suma, del modulo 'operaciones.js', imprimiendo en consola el resultado de dicha operacion tomando como parametros al entero 5 y entero 2" se interepretara que el mismo no es un Built-in de NodeJS.
  
  let op = require('./operaciones.js');
  console.log(op.suma(5,7));                    //imprimira en consola 7
  
  De indicarse que un modulo pertenece a los Built-in (nativos) de NodeJS la sintaxis difiere ligeramente:
  
  let math = require('math');
  console.log(math.log(10));                    //imprimira en consola 1
  
  Para la resolucion de los modulos se recomienda consultar:
    https://www.tutorialsteacher.com/nodejs/nodejs-module-exports
    https://developer.mozilla.org/es/docs/Web/JavaScript
    https://www.w3schools.com/nodejs/ y https://www.w3schools.com/js/default.asp
    https://nodejs.org/dist/latest-v10.x/docs/api/
  
  
