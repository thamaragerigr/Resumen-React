# Conceptos básicos de JSX

JavaScript Syntax Extansion
o
JavaScript XML

### Características

- Tiene que ser 'transpilado' a JS (Babel)
- Permite combinar el UI con la lógica de JS en un mismo archivo
- No es necesario utilizar JSX para que las aplicaciones de React funcionen, pero si es recomendado.

### Reglas

Es más estricto que HTML

- Necesita tener una etiqueta de cierre. 

        <div></div>

- Ser explicitamente cerrado si es una 'single tag'

        <input />

- Puedes integrar JS dentro de JSX utilizando '{ }'

        class Hello extends React.Component {
        render() {
            return (
            <div>
               <h1>Estoy {getMood()}</h1>
            </div>
            );
          }
        }

 > Aqui hace refetencia a una función (getMood())

 #### Ejemplo usando condicionales

    function getNum() {
        return Math.floor(Math.random() * 10) + 1;
    }
    class Hello extends React.Component {
        render() {
            const num = getNum();
            return (
            <div>
               <h1>Number: { num }</h1>
               <p>{ num === 7 ?'Congrats' : 'Not Lucky'}</p>
            </div>
            );
          }
        }

       function getNum() {
        return Math.floor(Math.random() * 10) + 1;
    }
    class Hello extends React.Component {
        render() {
            const num = getNum();
            return (
            <div>
               <h1>Number: { num }</h1>
               <p>{ num === 7 ?'Congrats' : 'Not Lucky'}</p>
               {
                   num === 7 
                   ? <img src="...">
                   : null
               }
            </div>
            );
          }
        }
-------------------------

              {
                   num === 7 
                   && <img src="...">
               }
