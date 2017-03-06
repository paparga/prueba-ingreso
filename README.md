# Prueba de ingreso RocketAd 2017-03

Esta prueba contiene 3 preguntas y está pensada para ser contestada utilizando funciones en javascript (idealmente ES6). 
Los tópicos a evaluar son los siguientes

1. Funciones de alto orden
2. Control de flujo con promesas
3. Promesas y funciones de alto orden

## 1. Funciones de alto orden

Utilizando las funciones map, filter y/o reduce, calcular la edad promedio de los perros cuya raza sea "Pug". El arreglo a utilizar es el siguiente:

```javascript
const perros = [ {nombre: 'Boby', raza: 'Golden', edad: 7}
               , {nombre: 'Washington', raza: 'Terrier Chileno', edad: 3}
               , {nombre: 'Firulais', raza: 'Pug', edad: 1}
               , {nombre: 'Chip', raza: 'Pastor Alemán', edad: 8}
               , {nombre: 'Pluto', raza: 'Pug', edad: 5}
               ]

const edadPromPug = // aquí el código`
```

## 2. Control de flujos con promesas

El siguiente bloque de código tiene problemas:

```javascript

const autorizaLanza = (codigoAutorizacion, coordenadas) => {
  return autoriza(codigoAutorizacion, coordenadas)
    .then(() => {
      lanzaMisiles(coordenadas)
     })
    .then(() => console.log("Misiles lanzados en coordenadas: ",coordenadas))
    .catch(err => console.error("No se pudo lanzar los misiles por la siguiente razon: ", err))
}
```

Explicar el problema y como solucionarlo.

## 3. Promesas y funciones de alto orden

Utilizando la siguiente promesa:
```javascript
const traePerros = () => Promise.resolve(perros)
```
Crear una función que devuelve la promesa con la edad promedio de los perros cuya raza sea "Pug".
