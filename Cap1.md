# React intro

## Diferencia entre librería 📚 y framework 🖼️

* Una libreria se añade a tu proyecto y se moldea a él dependiendo de lo que necesites. 
* Con un framework, sucede lo contrario. Tu app se adapta al mismo framework con el que haz decidido trabajar.

## ¿Y dónde entra React?

* React es una **Libreria** de JS para UI. 
* En principio no se categoriza como framework por si mismo, pero si se le agregan otras herramientas como **React Router, Redux, Webpack**.. es decir, su ecosistema standar, 'el stack', si se puede considerar un equivalente a otros framworks (como Angular y Vue.js)

## Algunos conceptos básicos

### Componentes

Son trozos de código que pueden ser reutilizados. Combinan la lógica (JS) t la presentación (JSX).

React cuenta con 4 tipos de componentes (pero solo veremos 2 por ahora):

#### Componentes Clase:

* Se resume como la manera 'tradicional' de escribir componentes de React.
* Consta de un método render que devuelve JSX.

        // Ejemplo de un componente Clase
        
        import React from 'react';
        class ComponenteClase extends React.Component {
          render() {
              return (
                <div>
                    <p>¡Un componente tipo Clase! 💃</p>
                </div>
              )
          }
        }
        export default ComponenteClase;

#### Componentes Función:

* Consta de una función que devuelve *JSX*. No necesita de un método render.
* Son usualmente usados para mostrar información.
* No tienen un estado o métodos de ciclos de vida (lifecycle methods), pero se pueden añadir implementando *React Hooks*
* Son fáciles de leer, debuggear y testear.

        // Ejemplo de Conponente función

        import React from 'react';
        const ComponenteFuncion = () => {
          return (
              <div>
                <p>Hello World!</p>
              </div>
          )
        }
        export default ComponenteFuncion;

#### Comparación entre ambos

* Ambos aceptan props y contenido renderizado.
* Los componentes class requieren de el render método, los function no.

### Props

* Es la información que se le pasa a los componentes
* Son inmutables, los componentes no pueden cambiar sus propias props

### State

* Es la información (data) interna del componente.
* Esta si puede cambiar/mutar.
