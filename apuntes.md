###### display : flex-flow
usar flexbox

###### flex-flow : { flex-direction }{ flex-flow } = flex-direction y flex-wrap
* flex-wrap : { arg }
  * wrap : no ajusta el contenido respeta el ancho y crea filas
  * no-wrap : afecta width para adaptarlo al contenedor

manejo basico del contenido

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

##### flex-grow : { args }
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
