🚀 Dashboard AJS
Dashboard AJS es una página de inicio personalizada (Custom Start Page) diseñada para centralizar accesos, tareas y el clima en una interfaz moderna con estilo Glassmorphism.

🛠 Instalación y Configuración
Sigue estos pasos para tener tu Dashboard funcionando en tu computadora:

1. Descarga y Preparación
Descarga este repositorio como un archivo .zip y descomprímelo en una carpeta de tu preferencia.

Coloca tu imagen de fondo favorita en la misma carpeta y asegúrate de que se llame FONDO.jpg (o ajusta el nombre en el archivo CSS).

2. Configuración Personalizada
Abre el archivo index.html con un editor de texto (como el Bloc de notas o VS Code) y busca la sección de configuración al principio del script:

JavaScript
const CONFIG = {
    apiKey: 'TU_API_KEY_AQUI', // Obtén tu clave en https://openweathermap.org/api
    city: 'Cuidad_de_Prefencia'       // Puedes cambiarla por tu ciudad
};
API Key: Crea una cuenta gratuita en OpenWeatherMap, genera tu API Key y pégala donde dice 'TU_API_KEY_AQUI'.

Ciudad: Cambia 'Manizales,CO' si deseas ver el clima de otro lugar.

3. Configurar en el Navegador (Google Chrome)
Para que esta página sea tu página de inicio cada vez que abras el navegador:

Obtener la ruta: Abre el archivo index.html en tu navegador. Copia la dirección completa que aparece en la barra superior (ejemplo: C:\Users\Nombre\Desktop\Dashboard-AJS\index.html).

Configuración de Chrome:

Ve a los tres puntos (⋮) en la esquina superior derecha > Configuración.

En el menú izquierdo, haz clic en "Al iniciar".

Selecciona la opción "Abrir una página específica o un conjunto de páginas".

Haz clic en "Añadir una nueva página" y pega la ruta que copiaste.

⚙️ Tecnologías y Herramientas
APIs: OpenWeatherMap API para el reporte meteorológico.

Almacenamiento: LocalStorage API para guardar tus tareas y links directamente en tu navegador.

Diseño: CSS Glassmorphism.

Debug/Test: Google Chrome DevTools (para realizar inspecciones y pruebas de código).

💡 ¿Cómo transferir mis datos a otro equipo?
Si cambias de computadora y quieres llevarte tus tareas y links, puedes extraer tus datos desde la consola (F12 > Console) usando:

JavaScript
// Para exportar:
console.log("Tareas:", localStorage.getItem("tasks"));
console.log("Links:", localStorage.getItem("myLinks"));
Proyecto diseñado para mejorar la productividad y estética del entorno de navegación
