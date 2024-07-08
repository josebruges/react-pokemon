# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

## Challenges to Resolve

### Reto 1: Corregir funcionamiento de la aplicación (5 mins)

**Descripción:** Busca por qué la aplicación no está funcionando y corrige el error.  
**Instrucciones:** Validar el manejo de promesas.

### Reto 2: Mejorar el Manejo de Errores (10 mins)

**Descripción:** Mejora el manejo de errores en las funciones `getPokemonInfo`, `getData` y `handleSearchPokemon`. Muestra mensajes de error al usuario usando un componente de notificación de Ant Design.  
**Instrucciones:**
- Añade un componente de notificación para mostrar errores.
- Modifica las funciones asincrónicas para manejar errores y mostrar un mensaje de error al usuario.

### Reto 3: Implementar un Paginador (15 mins)

**Descripción:** Corrige la renderización en “cargar más” e implementa un paginador que permita al usuario navegar entre diferentes páginas de la lista de Pokémon.  
**Instrucciones:**
- Utiliza el componente Pagination de Ant Design.
- Añade el paginador en la parte inferior de la lista de Pokémon.
- Modifica el estado y las funciones necesarias para que el paginador funcione correctamente.

### Reto 4: Refactorizar (5 mins)

**Descripción:** En el componente `PokemonList`, se ha implementado un renderizado condicional que muestra dos listas de Pokémon: una lista filtrada (`searchList`) y una lista completa (`pokemons`). Actualmente, el código presenta duplicación y podría optimizarse para mejorar la legibilidad y el rendimiento.  
**Instrucciones:** Refactoriza el código para eliminar la duplicación y mejorar la estructura del renderizado condicional de las listas de Pokémon. Asegúrate de mantener la funcionalidad existente de mostrar y cargar Pokémon, así como la funcionalidad de detalle de Pokémon (`PokemonDetail`).

**Consideraciones Adicionales:**
- Puedes modificar la estructura del código según consideres necesario, siempre y cuando mantengas la funcionalidad requerida.
- Asegúrate de mantener la estructura de filas y columnas (Row y Col) para el diseño.

### Reto 5: Mensaje de "No Encontrado" en Búsqueda de Pokémon (10 mins)

**Descripción:** En el actual componente `PokemonList`, la función de búsqueda (`handleSearchPokemon`) filtra la lista de Pokémon según el nombre proporcionado por el usuario. Sin embargo, cuando no se encuentran resultados para la búsqueda, no se muestra ningún mensaje al usuario.  
**Instrucciones:**
- Modificación de la Función de Búsqueda: Actualiza la función `handleSearchPokemon` para que, cuando la búsqueda no devuelva resultados (es decir, `filterPokemons` esté vacío), establezca el estado `searchEmpty` en `true`.
- Renderización del Mensaje de "No Encontrado": En el componente `PokemonList`, modifica el JSX para que, cuando `searchEmpty` sea `true`, muestre un mensaje indicando que no se encontraron Pokémon con el nombre buscado.

### Reto 6: Mostrar la información del Pokémon al darle click sobre la tarjeta (5 mins)

**Descripción:** Valida por qué al darle click encima del Pokémon no se muestra la información detallada.  
**Instrucciones:** Manejo de estados.
