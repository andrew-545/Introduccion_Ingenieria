# Buscador de Tareas en Tiempo Real

## 1. Descripción de la idea
Aplicación web interactiva para buscar y filtrar tareas en tiempo real según su título o categoría, diseñada con una interfaz moderna en modo oscuro sin necesidad de recargar la página.

## 2. Característica elegida
Filtrado reactivo en el cliente y manipulación dinámica del DOM utilizando JavaScript Vanilla y Tailwind CSS.

## 3. Qué se hizo para demostrarla
Se implementó un evento de escucha (`input`) sobre el campo de texto que analiza el término ingresado, realiza un filtrado insensible a mayúsculas sobre un arreglo de objetos en memoria y actualiza la interfaz en milisegundos mediante `replaceChildren()`. Además, gestiona un estado visual accesible cuando no se hallan coincidencias.

## 4. Requisito comprobable
* **Instrucción de prueba:** Abre el archivo `index.html` en el navegador e ingresa un término en la barra de búsqueda (por ejemplo: "Diseño" o "Trabajo").
* **Resultado esperado:** La lista renderiza únicamente las tarjetas que contienen la coincidencia en su título o categoría sin recargar la página. Si se escribe un término sin coincidencias (ej. "XYZ"), muestra el mensaje *"No se encontraron resultados"*.

## Instrucciones de ejecución
1. Clonar o descargar el repositorio.
2. Abrir el archivo `index.html` directamente en cualquier navegador web moderno (no requiere Node.js ni servidor local).