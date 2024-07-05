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

# Prueba Técnica: Componente Card

Este proyecto consiste en el desarrollo de un componente `Card` para una aplicación web.
En la `Card` se debe mostrar el estado (Abierto, cerrado, cierra pronto) que se considera según la hora del navegador.
Se debe seguir las reglas de horario: - Abierto: si la hora actual es mayor que el inicio del horario. - Cierra pronto: si la hora actual es mayor que el inicio y el menor por '1 hora' que el fin del horario. - Cerrado: si la hora actual es mayor que el fin del horario.

El objetivo es crear un componente reutilizable que siga las especificaciones de diseño proporcionadas.

## Requisitos

- El componente debe ser desarrollado utilizando React.
- Debe ser completamente responsive y adaptarse a diferentes tamaños de pantalla.
- Deberá aceptar props para personalizar el contenido, incluyendo pero no limitándose a:
  - id
  - banner
  - logo:
  - title
  - ubicación
  - horario:
    - dia
    - inicio
    - fin
  - labelLink
  - link
- Debe seguir las pautas de diseño proporcionadas en los mockups adjuntos.
- Implementar estados de horario (Abierto, Cierra pronto, Cerrado) donde sea aplicable, según el diseño.

## Tecnologías

- React para el desarrollo del componente.
- CSS o Sass para estilos.

## Entrega

Tu entrega deberá incluir:

- Código fuente del componente `Card`.
- Ejemplos de uso dentro de una aplicación React App.js .
- Superar la prueba unitaria que demuestren la funcionalidad y robustez del componente.

## Criterios de Evaluación

- **Calidad del Código**: El código debe ser limpio, bien organizado y seguir las mejores prácticas de desarrollo.
- **Funcionalidad**: El componente debe funcionar según lo especificado y ser libre de errores.
- **Diseño y UX**: El componente debe coincidir con el diseño proporcionado y ofrecer una buena experiencia de usuario.
- **Responsividad**: El componente debe verse y funcionar bien en una variedad de dispositivos y tamaños de pantalla.

## Mockups

> ![Descripción de la imagen](src/assets/card.png) > ![Descripción de la imagen](src/assets/status.png) > ![Descripción de la imagen](src/assets/view.png)

## Ejemplo de Uso

```jsx
import cardData from "./data/cardData";
import Card from "./components/Card/Card";

function App() {
  return (
    <div className="App">
      {cardData.map((card) => {
        return <Card {...card} key={card.id} />;
      })}
    </div>
  );
}

export default App;
```
