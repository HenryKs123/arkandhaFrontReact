Frontend React para API de Propiedades y Propietarios
Este proyecto es un frontend construido con React que se comunica con las APIs de Propiedades y Propietarios en tu backend Django. El frontend utiliza la librería Axios para realizar las peticiones HTTP a los endpoints mencionados en el README del backend.

Primeros pasos
Sigue estos pasos para configurar y ejecutar el frontend en tu máquina local:

Clona este repositorio en tu máquina:

bash
Copy code
git clone https://github.com/tu-usuario/tu-proyecto-frontend.git
cd tu-proyecto-frontend
Instala las dependencias del proyecto:

bash
Copy code
npm install
Configura los archivos de comunicación:

En la carpeta src/api, encontrarás dos archivos: apiPropiedad.js y apiPropietario.js. Cada archivo contiene funciones que utilizan Axios para realizar las peticiones a las APIs respectivas.

Ejecuta la aplicación:

bash
Copy code
npm start
Accede a la aplicación en tu navegador: http://localhost:3000

Componentes
El frontend consta de 8 componentes independientes que se reutilizan en todo el proyecto. Estos componentes se encuentran en la carpeta src/components.

Componente1.js: Descripción del primer componente.
Componente2.js: Descripción del segundo componente.
...
Componente8.js: Descripción del octavo componente.
Uso de los archivos de comunicación
Los archivos apiPropiedad.js y apiPropietario.js en la carpeta src/api contienen funciones que interactúan con las APIs de Propiedades y Propietarios respectivamente.

Ejemplo de uso:
javascript
Copy code
import { obtenerPropiedades } from './apiPropiedad';
import { obtenerPropietarios } from './apiPropietario';

// Obtener todas las propiedades
obtenerPropiedades()
  .then(respuesta => {
    console.log(respuesta.data);
  })
  .catch(error => {
    console.error('Error:', error);
  });

// Obtener todos los propietarios
obtenerPropietarios()
  .then(respuesta => {
    console.log(respuesta.data);
  })
  .catch(error => {
    console.error('Error:', error);
  });

