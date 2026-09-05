# M2.-Actividad-de-aprendizaje-para-RA2
Taller práctico implementado CSS3, flexbox y Grid
# Dashboard Administrativo de Inventario

## Descripción
Este proyecto consiste en el desarrollo de un **dashboard administrativo para la gestión de inventario**. Su objetivo es presentar de manera clara y organizada información relacionada con productos, ventas, pedidos y disponibilidad del inventario.
El dashboard cuenta con una interfaz moderna y adaptable a diferentes tamaños de pantalla. Desde la pantalla principal se pueden visualizar diferentes indicadores, un gráfico de ventas mensuales, el estado general del inventario y una tabla con los productos registrados recientemente.
El diseño fue pensado para facilitar la visualización rápida de la información más importante de un sistema administrativo.
## Tecnologías utilizadas
Para el desarrollo del proyecto se utilizaron las siguientes tecnologías:
* **HTML5:** utilizado para construir la estructura y contenido del dashboard mediante etiquetas semánticas.
* **CSS3:** utilizado para los estilos visuales, colores, tipografías, animaciones y diseño responsive.
* **CSS Grid:** utilizado para organizar la estructura principal del dashboard mediante áreas de navegación, encabezado, contenido y pie de página.
* **Flexbox:** utilizado para organizar los elementos internos de las tarjetas, menús, encabezado, perfil de usuario y otros componentes.
* **JavaScript:** utilizado para implementar la interacción del menú lateral colapsable.
* **Media Queries:** utilizadas para adaptar la interfaz a computadores, tablets y dispositivos móviles.
## Estructura del proyecto
## Componentes principales
El dashboard está compuesto por diferentes elementos administrativos:
### Barra lateral de navegación
Contiene las diferentes secciones del sistema, como:
* Dashboard
* Productos
* Ventas
* Clientes
* Reportes
* Configuración
* Ayuda
También incluye la información básica del usuario administrador.
### Tarjetas de resumen
En la parte superior del contenido se presentan cuatro tarjetas con información importante:
* Total de productos.
* Ventas del mes.
* Pedidos realizados.
* Productos con stock bajo.
Estas tarjetas permiten consultar rápidamente los principales indicadores del inventario.
### Gráfico de ventas
Se incorporó un gráfico de barras para representar visualmente el comportamiento de las ventas durante los diferentes meses del año.
Esto facilita la interpretación de los datos sin necesidad de revisar únicamente valores numéricos.
### Estado del inventario
Se incluye un indicador visual que muestra la distribución de productos disponibles, productos con stock bajo y productos agotados.
### Tabla de productos
La tabla permite visualizar información de los productos registrados, incluyendo:
* Nombre.
* Categoría.
* Precio.
* Cantidad disponible.
* Estado.
* Acciones.
## Decisiones de diseño
Para el diseño se utilizó una interfaz limpia y sencilla, utilizando un fondo claro y tarjetas blancas para separar visualmente las diferentes secciones.
Se utilizó un color principal azul/morado para destacar elementos importantes como:
* Botones.
* Elementos activos del menú.
* Indicadores.
* Barras del gráfico.
También se utilizaron diferentes colores para representar estados del inventario. Por ejemplo, el verde representa productos disponibles, el naranja indica productos con stock bajo y el rojo representa productos agotados.
Las tarjetas tienen bordes redondeados y sombras suaves para generar una separación visual entre los diferentes componentes.
Además, se agregaron efectos hover y transiciones para proporcionar una respuesta visual cuando el usuario interactúa con botones, tarjetas, enlaces y elementos de la tabla.
## Uso de CSS Grid y Flexbox
El layout principal se construyó utilizando **CSS Grid**. Se utilizaron áreas nombradas mediante "grid-template-areas" para organizar:
Por otro lado, **Flexbox** se utilizó para organizar los elementos internos de los componentes, por ejemplo:
* Elementos de navegación.
* Información del usuario.
* Encabezado.
* Tarjetas.
* Botones.
* Indicadores de inventario.
* Elementos del gráfico.
De esta manera, Grid se encarga principalmente de la distribución general de la página y Flexbox de la alineación de los elementos dentro de cada componente.
## Responsividad
El dashboard fue diseñado para adaptarse a diferentes dispositivos mediante **media queries**.
Se establecieron diferentes comportamientos para:
* **Escritorio:** se muestra el sidebar completo y se aprovecha el espacio horizontal.
* **Tablet:** las tarjetas y contenidos se reorganizan para adaptarse al menor ancho disponible.
* **Móvil:** el contenido se presenta principalmente en una sola columna y el sidebar se convierte en un menú lateral desplegable.
Esto permite que el dashboard mantenga una estructura funcional independientemente del dispositivo utilizado.
## Accesibilidad
Se tuvieron en cuenta diferentes buenas prácticas de accesibilidad durante el desarrollo.
Se utilizaron etiquetas semánticas de HTML5 como:
```html
<header>
<aside>
<nav>
<main>
<section>
<article>
<footer>
```
También se incorporaron atributos ARIA en elementos interactivos, por ejemplo:
```html
aria-label
aria-expanded
aria-controls
aria-current
```
Los botones y enlaces cuentan con estados focus y focus-visible, permitiendo identificar visualmente el elemento seleccionado mediante navegación por teclado.
Los iconos utilizados como elementos decorativos incluyen:
```html
aria-hidden="true"
```
