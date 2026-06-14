
# Dashboard AJS

Dashboard AJS es una página de inicio personalizada (Custom Start Page) diseñada para centralizar tus accesos, tareas y el clima en una interfaz moderna con estilo Glassmorphism.

## 🛠 Instalación y Configuración

### 1. Preparación
1. Descarga el repositorio y descomprímelo en una carpeta.
2. Coloca tu imagen de fondo en la misma carpeta y asegúrate de que se llame `FONDO.jpg`.

### 2. Configuración Personalizada
Abre el archivo `index.html` en un editor de texto y busca la sección de configuración al inicio del script:

```javascript
const CONFIG = {
    apiKey: 'TU_API_KEY_AQUI', // Obtén tu clave en [https://openweathermap.org/api](https://openweathermap.org/api)
    city: '-------'       // Puedes cambiarla por tu ciudad
};

```

* **API Key:** Regístrate en OpenWeatherMap, genera tu clave gratuita y pégala entre las comillas.
* **Ciudad:** Cambia ------- por tu ubicación preferida (ej: Manizales,CO).

### 3. Configurar en el Navegador (Google Chrome)

1. Abre el archivo `index.html` en tu navegador.
2. Copia la ruta que aparece en la barra de direcciones (ej: `file:///C:/Users/.../index.html`).
3. En Chrome, ve a Configuración > Al iniciar > Abrir una página específica.
4. Pega la ruta y guarda los cambios.

## ⚙️ Tecnologías y Herramientas

* **APIs:** OpenWeatherMap API para el clima.
* **Almacenamiento:** LocalStorage API para persistencia de datos local.
* **Diseño:** CSS Glassmorphism.
* **Desarrollo:** Chrome DevTools para inspección y pruebas en tiempo real.

## 🔄 Transferencia de Datos entre Dispositivos

Si cambias de equipo, puedes migrar tus Tareas y Accesos ejecutando estos comandos en la consola de tu navegador (F12 > Console):

### Para Exportar (Copiar tus datos actuales)

```javascript
console.log("--- TAREAS ---");
console.log(localStorage.getItem("tasks"));
console.log("--- ACCESOS ---");
console.log(localStorage.getItem("myLinks"));

```

### Para Importar (Pegar datos en el nuevo equipo)

```javascript
localStorage.setItem("tasks", 'PEGA_AQUI_TUS_TAREAS_JSON');
localStorage.setItem("myLinks", 'PEGA_AQUI_TUS_LINKS_JSON');
location.reload();

```

```

```
