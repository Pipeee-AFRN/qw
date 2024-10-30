# FC Barcelona Website

Este proyecto es una página web dedicada al FC Barcelona, diseñada para ofrecer información sobre el club, sus noticias y una galería de imágenes. La página utiliza HTML y CSS, implementando técnicas de diseño modernas como Grid y Flexbox.

<div align="center">![](assets/img/logo-FCB.png)</div>

## Características

- Información sobre el club
- Galería de imágenes
- Formulario de contacto
## Estructura del Proyecto

- **HTML:** Contiene la estructura básica de la página, incluyendo el menú de navegación, secciones de bienvenida, sobre nosotros, galería, servicios y contacto.
- **CSS:** Se encarga del estilo visual y del diseño responsivo.


## Uso de HTML Semántico

Se ha utilizado HTML semántico para mejorar la accesibilidad y la comprensión del contenido. Algunas de las etiquetas semánticas empleadas son:

- `<header>`: Define el encabezado de la página, incluyendo el menú de navegación.
- `<nav>`: Contiene los enlaces de navegación, ayudando a los motores de búsqueda y a los lectores de pantalla a identificar la estructura de navegación.
- `<section>`: Agrupa contenido relacionado, como la sección de bienvenida y la sección de sobre nosotros, facilitando la organización del documento.
- `<footer>`: Define el pie de página, que contiene información sobre derechos de autor y otros enlaces relevantes.

### Ejemplo de HTML Semántico

```html
<header class="main-header">
    <nav id="menu">
        <ul>
            <li><a href="#home">Inicio</a></li>
            <li><a href="#about">Sobre Nosotros</a></li>
            <li><a href="#gallery">Galería</a></li>
            <li><a href="#services">Noticias</a></li>
            <li><a href="#contact">Contacto</a></li>
        </ul>
    </nav>
</header>

<main>
    <section id="welcome">
        <spam class="title-back">MÁS QUE UN CLUB</spam>
    </section>
    <!-- Otras secciones -->
</main>

<footer class="main-footer">
    <p>&copy; 2024 FC Barcelona. Todos los derechos reservados.</p>
</footer>
```
## Uso de Grid y Flexbox

- **Grid:** Se utiliza en la sección de galería para organizar las imágenes en un diseño adaptable. Esto permite que las imágenes se ajusten automáticamente al tamaño de la pantalla, creando un diseño de columnas que se adapta a diferentes dispositivos. El CSS utilizado es:

-
<div align="center"> ![](assets/img/galeria.jpg)</div> 
```css
  
    .gallery-grid {
      display: grid; /* Activa el modelo de diseño de cuadrícula (grid) en el contenedor. */
    /* Define las columnas de la cuadrícula: 
       - Se crean tantas columnas como sea posible.
       - Cada columna tiene un ancho mínimo de 300px y un máximo de 1fr (una fracción del espacio disponible). */
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
    max-width: 1200px;
    margin: 0 auto;
    }
```

```
- **Flexbox:** Se aplica en el contenedor principal para centrar el contenido vertical y horizontalmente en la página. Esto es especialmente útil para la sección de bienvenida, asegurando que el título y el video de fondo estén correctamente alineados. El CSS utilizado es:

- 
<div align="center">![](assets/img/flex.jpg)</div>

```css
    .container {
          display: flex; /* Activa el modelo de diseño flexible (flex) en el contenedor. */
          /* Alinea los elementos hijos en el centro del contenedor a lo largo del eje horizontal. */
          justify-content: center;
          /* Alinea los elementos hijos en el centro del contenedor a lo largo del eje vertical. */
          align-items: center;
          height: 100vh;
          margin: auto; 
          padding: 3rem 1.5rem;
      }
```
