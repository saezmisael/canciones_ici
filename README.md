📖 Cancionero Web - Iglesia de Cristo Internacional

Aplicación web (Single Page Application) diseñada para visualizar, buscar y organizar las alabanzas e himnos de la iglesia. Construida con un diseño moderno, elegante y 100% responsivo para ser utilizada desde cualquier dispositivo (celular, tablet o PC).

🚀 Características Principales

Buscador Inteligente: Filtra canciones en tiempo real por título, número, autor o por fragmentos de la letra.

Ordenamiento Automático: Las canciones siempre se mostrarán en orden numérico ascendente (1, 2, 3...) sin importar en qué orden se hayan programado en el código.

Diseño Institucional: Uso de paleta de colores de la iglesia (Blanco, Rojo, Negro), tipografía cursiva elegante y un logotipo reconstruido con vectores (SVG) para evitar pérdida de calidad.

Modo Lectura Optimizado: Modal envolvente que adapta el tamaño de fuente según el dispositivo y respeta los saltos de línea de la letra.

Resaltado Inteligente: Detecta automáticamente la palabra CORO o CORO: en la letra de cualquier canción y la resalta en rojo y negrita para guiar a los músicos y cantantes.

Copiado Rápido: Botón integrado en la vista de lectura para copiar instantáneamente la letra al portapapeles del dispositivo.

🛠️ Tecnologías Utilizadas

HTML5

Tailwind CSS (vía CDN para estilos responsivos y modernos sin necesidad de archivos CSS adicionales).

Vanilla JavaScript (Toda la lógica de búsqueda, ordenamiento y renderizado sin dependencias pesadas).

FontAwesome (Íconos de la interfaz).

Google Fonts (Fuente Dancing Script para el logo).

📝 ¿Cómo añadir o modificar alabanzas?

Dado que este proyecto está pensado para alojarse de manera estática y gratuita (ej. GitHub Pages), la base de datos de alabanzas se encuentra inyectada directamente en el archivo index.html.

Para añadir una nueva canción:

Abre el archivo index.html.

Busca la sección que dice: // 1. AÑADE TUS ALABANZAS POR CÓDIGO AQUÍ

Copia y pega un bloque de canción existente, respetando esta estructura:

{
    id: 12, // ¡Muy importante! El número de la canción
    title: "12. Título de la canción",
    artist: "Alabanza o Himno Tradicional",
    lyrics: "Escribe aquí tu letra.\n\nUsa '\\n' para hacer saltos de línea.\n\nCORO:\nEsto se pondrá en rojo automáticamente."
}, // No olvides la coma al final si vas a poner más canciones abajo.


🤖 ¿Cómo seguir programando con Gemini a futuro?

Si vuelves en unas semanas o meses y quieres añadirle nuevas funciones al cancionero (por ejemplo, modo oscuro, separación de archivos, o conectarlo a una base de datos real como Firebase), simplemente mándale a Gemini este archivo README.md junto con el index.html y dile:

"Hola Gemini, aquí te comparto el código de mi cancionero actual (index.html) y su documentación (README.md). Quiero que le agreguemos la siguiente función..."

Con eso, la IA entenderá exactamente el contexto, la paleta de colores que elegimos y las reglas de diseño (como el logo y los colores rojo/blanco/negro) sin tener que empezar desde cero.