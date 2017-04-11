###### display : flex
usar flexbox

###### flex-direction : { arg }
el limite es el tamaño del contenedor
* row : una acomoda los elementos de izq a der por filas

| Header One     | Header Two     | Header Three   |
| :------------- | :------------- | :------------- |
| Item One       | Item Two       | item Tree      |
| Item four      | -              | -              |

* row-reverse
* column : acomoda de arriba hacia abajo por columnas

| Header One     | Header Two     |
| :------------- | :------------- |
| Item One       | Item Four      |
| Item Two       | -              |
| Item Three     | -              |

###### flex-wrap : { arg }
determina si se redimensiona para ajustar a una linea o no
* wrap : continua si no cabe en la siguiente linea
* no-wrap : redimensiona para que los elementos quepan en una linea

###### flex-flow : { flex-direction }{ flex-wrap }
Abreviación de direction y wrap recibiendo en ese orden los argumentos.

## Manejo basico del contenido

##### justify-content : { arg }  ---> (horizontal)
* flex-end : inicio de izq a der
* center : centra contenido horizontalmente
* space-around : crea espaciado entre los contenidos
* space-betwen : crea espaciado entre contenidos pero excluye inicio y fin del contenedor

##### align-items : { arg } ---> (vertical)
* flex-start : defecto
* flex-end : elementos al fondo del contenido
* center : centrado vertical
* stretch : (height auto) abarcar el 100% horizontal
* baseline : alinea con respecto a el texto

##### align-content : { arg }
mismos valores que align-items pero especializado para varias filas (flex-wrap : wrap)

##### flex-basis : { arg }
el argumento son pixeles y representa width o heigth dependiendo el flex-direction

##### flex-grow : { numero }
* numero : proporcion de crecimiento
al crecer este numero determina que tanto crece con respecto a su contenedor

##### flex-shrink : { numero }
inverso de grow. "encogimieto"

##### flex : { grow } { shrink } { basis }
forma de abreviar grow shrink y basis

##### order : { num }
altera el orden en el que aparecen de izq a der, solo es visual no se altera el DOM

##### align-self : { arg }
mismos que para align-items, funciona solo para un elemento. no afecta a los demas
