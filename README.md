# Dashboard AJS

Dashboard AJS es una página de inicio personalizada (Custom Start Page) diseñada para centralizar tus accesos, tareas y el clima en una interfaz moderna con estilo *Glassmorphism*.

## 🛠 Instalación y Configuración

Sigue estos pasos para configurar tu Dashboard:

### 1. Preparación
1. Descarga el repositorio y descomprímelo en una carpeta.
2. Coloca tu imagen de fondo en la misma carpeta y asegúrate de que se llame `FONDO.jpg`.

### 2. Configuración Personalizada
Abre el archivo `index.html` en un editor de texto y busca la sección de configuración al inicio del script:

```javascript
const CONFIG = {
    apiKey: 'TU_API_KEY_AQUI', // Obtén tu clave en [https://openweathermap.org/api](https://openweathermap.org/api)
    city: 'Manizales,CO'       // Puedes cambiarla por tu ciudad
};
