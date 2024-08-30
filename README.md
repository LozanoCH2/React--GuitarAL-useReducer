# Proyecto GuitarAL - Migración a useReducer

Este proyecto consiste en la migración de GuitarAL, originalmente construido con un hook personalizado, a utilizar el hook `useReducer` de React. El objetivo principal de esta migración fue profundizar en el uso de `useReducer` y aprovechar sus ventajas, especialmente en la simplificación y mejora del código mediante el uso de acciones.

Puedes ver la aplicación en acción [aquí](https://react-carritocompras-typescript.netlify.app).

## Tabla de Contenidos

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Instalación](#instalación)
- [Funcionalidades](#funcionalidades)
- [Ventajas de useReducer](#ventajas-de-usereducer)
- [Créditos](#créditos)
- [Conclusión](#conclusión)

## Descripción del Proyecto

GuitarAL es una aplicación que permite a los usuarios agregar guitarras a un carrito de compras. El proyecto incluye las siguientes funcionalidades:

- **Listado de Guitarras**: Los usuarios pueden seleccionar guitarras y agregarlas al carrito de compras.
- **Carrito de Compras**: El carrito muestra un resumen de las guitarras seleccionadas, la cantidad de cada una, y el total a pagar.
- **Gestión del Carrito**: Los usuarios pueden incrementar o decrementar la cantidad de guitarras (hasta un máximo de 5 por guitarra), eliminar una guitarra específica o limpiar todo el carrito.
- **Persistencia con Local Storage**: Las guitarras seleccionadas se guardan en el local storage para mantener el estado incluso al recargar la página.

## Tecnologías Utilizadas

- **React**: Biblioteca de JavaScript para construir interfaces de usuario.
- **useReducer**: Hook de React utilizado para gestionar el estado del carrito de manera eficiente.
- **Local Storage**: Para la persistencia de datos en el navegador.

## Instalación

Para ejecutar este proyecto localmente, sigue estos pasos:

1. Clona el repositorio:
    ```bash
    git clone https://github.com/tuusuario/guitarl-migracion-usereducer.git
    ```
2. Navega al directorio del proyecto:
    ```bash
    cd guitarl-migracion-usereducer
    ```
3. Instala las dependencias:
    ```bash
    npm install
    ```
4. Inicia el servidor de desarrollo:
    ```bash
    npm run dev
    ```

## Funcionalidades

- **Agregar Guitarras al Carrito**: Los usuarios pueden seleccionar guitarras para añadirlas al carrito.
- **Incrementar/Decrementar Cantidad**: Ajusta la cantidad de guitarras en el carrito (máximo 5 unidades por guitarra).
- **Eliminar Guitarra del Carrito**: Remueve una guitarra específica del carrito.
- **Limpiar el Carrito**: Elimina todas las guitarras del carrito.
- **Calcular Total**: Calcula el total a pagar basado en las guitarras seleccionadas.

## Ventajas de useReducer

Al migrar GuitarAL a `useReducer`, obtuve varias ventajas clave sobre el uso del hook personalizado anterior:

- **Manejo Centralizado del Estado**: `useReducer` permite centralizar la lógica del estado, lo que facilita su gestión y mantenimiento.
- **Acciones Definidas**: Al utilizar acciones (`add`, `remove`, `increment`, `decrement`, `clear`), se puede manejar el estado de manera predecible y organizada.
- **Escalabilidad**: A medida que el proyecto crece, `useReducer` proporciona una estructura más escalable en comparación con un hook personalizado.
- **Mejora en la Legibilidad del Código**: Al utilizar `useReducer`, el código se vuelve más limpio y fácil de seguir, especialmente en proyectos con lógica compleja.

## Créditos

Este proyecto fue realizado como parte del curso de React y TypeScript de [codigoconjuan](https://codigoconjuan.com). Agradezco profundamente la enseñanza y los recursos proporcionados durante el curso, que me permitieron adquirir las habilidades necesarias para desarrollar esta aplicación.

## Conclusión

Migrar GuitarAL a `useReducer` fue una experiencia valiosa que me permitió comprender mejor las capacidades de este hook en la gestión del estado de aplicaciones React. Las ventajas obtenidas en términos de simplificación del código, escalabilidad y mantenimiento destacan la importancia de `useReducer` en proyectos que manejan un estado complejo. Este aprendizaje me prepara para enfrentar desafíos más grandes en el desarrollo de aplicaciones web.
