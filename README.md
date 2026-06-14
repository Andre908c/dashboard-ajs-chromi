# Dashboard AJS

Dashboard AJS es una página de inicio personalizada (Custom Start Page) diseñada para centralizar accesos, tareas y el clima en una interfaz moderna y minimalista.

## ✨ Características
- **Quick Links:** Gestión de accesos rápidos con detección automática de iconos.
- **Task Tracker:** Sistema de tareas persistentes (no se borran al cerrar el navegador).
- **Live Weather:** Integración en tiempo real con OpenWeatherMap para obtener el clima actual.
- **Glassmorphism Design:** Diseño estético con efectos de desenfoque y transparencia.
- **Persistencia:** Todos tus datos se guardan de forma local en tu navegador usando la API de LocalStorage.

## 🛠 Tecnologías Utilizadas
- **HTML5:** Estructura web.
- **CSS3:** Diseño y efectos visuales.
- **JavaScript:** Lógica funcional y consumo de APIs.

## 🚀 Cómo usarlo
1. Descarga el repositorio o clona el proyecto.
2. Abre el archivo `index.html` en cualquier navegador moderno.
3. ¡Personaliza tus accesos y comienza a organizar tu día!

## ⚙️ Instalación (Para transferir a otro dispositivo)
Si deseas mover tu Dashboard a otro equipo, puedes transferir los datos siguiendo estos comandos en la consola (F12 > Console) de tu navegador:

**Para exportar tus datos:**
```javascript
console.log("Tareas:", localStorage.getItem("tasks"));
console.log("Links:", localStorage.getItem("myLinks"));
