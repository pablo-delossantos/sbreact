# Inicio rápido

Etiquetas de componentes: `<MyButton />` empieza con mayúscula. Así es como sabes que es un componente de React. Los nombres de los componentes de React siempre deben comenzar con mayúscula, mientras las etiquetas HTML deben estar minúsculas.

Las palabras clave `export default` especifican el componente principal en el archivo.

La sintaxis de marcado se llama JSX. JSX es más estricto que HTML. Tienes que cerrar etiquetas como `<br />`. Tu componente tampoco puede devolver múltiples etiquetas de JSX. Debes envolverlas en un padre compartido, como `<div>...</div>` o en un envoltorio vacío `<>...</>`.



## Mostrar datos

JSX te permite poner marcado dentro de JavaScript. Las llaves te permiten «escapar de nuevo» hacia JavaScript de forma tal que puedas incrustar una variable de tu código y mostrársela al usuario. Por ejemplo, esto mostrará `user.name`

```
return (
  <h1>
    {user.name}
  </h1>
);
```

### Renderizado condicional

> En React, no hay una sintaxis especial para escribir condicionales.

## El uso de los Hooks

Las funciones que comienzan con use se llaman _Hooks_. `useState` **es un Hook nativo dentro de React**. Puedes encontrar otros Hooks nativos en la referencia de la API de React. También puedes escribir tus propios Hooks mediante la combinación de otros existentes.

Los Hooks son más restrictivos que las funciones regulares. **Solo puedes llamar a los Hooks en el primer nivel de tus componentes** (u otros Hooks). Si quisieras utilizar `useState` en una condicional o en un bucle, extrae un nuevo componente y ponlo ahí.

### Props

Las props son la **colección de datos** que un componente recibe del contenedor padre, y que pueden usarse para definir los elementos de React que retornará el componente.

En términos prácticos, si un componente necesita recibir información para funcionar, la recibe vía props.

## Compratir datos entre componentes

> Ver: «levantar el estado». Al mover el estado hacia arriba, lo compartimos entre componentes.
