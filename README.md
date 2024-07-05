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

Este proyecto consiste en el desarrollo de un componente `Card` para una aplicación web. El objetivo es crear un componente reutilizable que siga las especificaciones de diseño proporcionadas.

## Requisitos

- El componente debe ser desarrollado utilizando React.
- Debe ser completamente responsive y adaptarse a diferentes tamaños de pantalla.
- Deberá aceptar props para personalizar el contenido, incluyendo pero no limitándose a:
  - Título
  - Imagen de fondo
  - Logo
  - Ubicación
  - Horario
  - Enlace para más información
- Debe seguir las pautas de diseño proporcionadas en los mockups adjuntos.
- Implementar estados de hover donde sea aplicable, según el diseño.
- Asegurar la accesibilidad, incluyendo etiquetas ARIA donde sea necesario.

## Tecnologías Sugeridas

- React para el desarrollo del componente.
- CSS o Sass para estilos.
- Jest y React Testing Library para pruebas unitarias.

## Entrega

Tu entrega deberá incluir:

- Código fuente del componente `Card`.
- Documentación en el README sobre cómo utilizar el componente.
- Ejemplos de uso dentro de una aplicación React.
- Pruebas unitarias que demuestren la funcionalidad y robustez del componente.
- Capturas de pantalla o un enlace a un despliegue en vivo donde se pueda ver el componente en acción.

## Criterios de Evaluación

- **Calidad del Código**: El código debe ser limpio, bien organizado y seguir las mejores prácticas de desarrollo.
- **Funcionalidad**: El componente debe funcionar según lo especificado y ser libre de errores.
- **Diseño y UX**: El componente debe coincidir con el diseño proporcionado y ofrecer una buena experiencia de usuario.
- **Responsividad**: El componente debe verse y funcionar bien en una variedad de dispositivos y tamaños de pantalla.
- **Accesibilidad**: El componente debe ser accesible para usuarios con diferentes capacidades.

## Mockups

> Aquí deberías incluir imágenes o enlaces a los mockups de diseño que se deben seguir para el desarrollo del componente.

## Ejemplo de Uso

```jsx
import React from "react";
import Card from "./path/to/Card";

function App() {
  return (
    <div className="App">
      <Card
        title="Título de la Card"
        backgroundImageUrl="./path/to/image.jpg"
        logoUrl="./path/to/logo.png"
        location="Ubicación"
        schedule={{ day: "Lunes a Viernes", hours: "9:00 - 18:00" }}
        moreInfoLink="https://www.ejemplo.com"
      />
    </div>
  );
}

export default App;
```
