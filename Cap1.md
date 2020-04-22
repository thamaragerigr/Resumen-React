React intro

> Diferencia entre libreria y framework

Una libreria se añade a tu proyecto y se moldea a el dependiendo de lo que necesites. Con un framework conectas tu app y esta se adapta al mismo. Son muy ligeras.

React es una **Libreria** de JS para UI. En principio no se categoriza como framework por si mismo, pero si se le agregan otras herramientas como React Router, Redux, Webpack.. es decir su ecosistema standar, 'el stack', si se puede considerar un equivalente a otros framworks (como Angular y Vue.js)

two types of components
Class
Function

Componentes Clase:

- Se resume como la manera 'tradicional' de escribir componentes de react
- Consta de un método render que devuelve JSX

Componentes Funcion:
-Componentes mas sencillos
-Consta de una funcion que devuelve un elemento. No necesita de un método render

Diferencias

- Ambas aceptan props y contenido renderizado
- Historicamente, los componentes funcion no podian utilizar features importantes como state y lifecycle methods.Ahora con los hooks se pueden integrar estos features.
- Los componentes class requieren de el render método, los function no


Core concepts 
- components 
  - building blocks of react
  - combines logic (JS) and presentation (JSX)

 - props
   - data passed to components
   - immutables, components cant change their ownw props

- state
  - internal data of a component
  - data that can change 