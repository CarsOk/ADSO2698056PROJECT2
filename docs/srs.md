# ESPECIFICACION DE REQUERIMIENTOS

## 1.Introducción

1.1 Propósito

El propósito del sitio web es crear una plataforma en línea para que los usuarios puedan acceder a información, servicios y productos del sitio web, describir lo acordado con el cliente y desarrollar el paso a paso para el software que servirá para ampliar el rango de venta de la farmacia, publicitar sus productos y generar mayores ganancias, generando un control y registro de las ventas.

1.2 Alcance

El sistema será un sitio ventas web accesible a través de internet. El cual brindara una interfaz de usuarios y productos para que los usuarios puedan interactuar. Este sistema aportara en:
•	Registro e inicio de usuarios
•	Administración de los productos disponibles del inventario
•	Generar factura electrónica 
•	Selección de productos y compra de los mismos 


1.3 Definiciones, Acrónimos, y Abreviaturas

HTML: Hypertext Markup Language (Lenguaje de marcas de hipertexto)

CSS: Cascading Style Sheets (Hojas de estilo en cascada)

PHP: Hypertext Preprocessor (Preprocesador de hipertexto)

CMS: Content Management System (Sistema de gestión de contenido)

UI: User Interface (Interfaz de usuario)
UX: User Experience (Experiencia de usuario)
SEO: Search Engine Optimization (Optimización para motores de búsqueda)
SSL: Secure Sockets Layer (Capa de sockets seguros)

1.4 Referencias

Se utilizarán las siguientes referencias:

HTML5 specification: https://www.w3.org/TR/html5/
CSS3 specification: https://www.w3.org/TR/css-2018/ 
PHP manual: https://www.php.net/manual/ 
Bootstrap framework: https://getbootstrap.com/ 
Wordpress CMS: https://wordpress.org/ 
Google Analytics: https://analytics.google.com/ 
Yoast SEO plugin: https://yoast.com/wordpress/plugins/seo/

1.5 Apreciación Global

El sitio web se desarrollará con el objetivo de proporcionar una experiencia de usuario atractiva y funcional para los visitantes del sitio. Se pondrá un gran énfasis en la seguridad y el rendimiento del sitio, así como en la optimización para motores de búsqueda y la accesibilidad.

### 2. Descripción General

2.1 Perspectivas del Producto

Con este proyecto se espera una mejora en las ventas de la farmacia, dicho sistema brindara facilidad al usuario en la compra de productos y obtención de la información de estos mismos. Ya que muchos negocios cuentan con sitios web que los promocionan, esta farmacia tendrá el suyo también.

2.2 Funciones del Producto

El sitio web tendrá las siguientes funciones:

·Página de inicio con información general sobre el sitio web y sus servicios/productos
·Páginas de contenido para información específica sobre los servicios/productos ofrecidos
·Formularios de contacto para consultas de clientes
·Integración con las redes sociales para compartir contenido
·Página de inicio de sesión para usuarios registrados
·Carrito de compras y página de pago para compras en línea
·Blog y sección de noticias para publicar contenido actualizado y relevan
.Generar factura electrónica de las compras que se realicen 
.Editar la cantidad y elección de los productos que estén en el carrito de compra 

2.3 Características de Usuario

Los usuarios que interactuaran con este sitio web serán las personas encargadas de la administración de dicho sitio, las personas que realizaran las compras, el administrador que velara del buen funcionamiento del sitio web.


2.4 Restricciones

Para este sistema las posibles restricciones son, el tiempo que tomara el desarrollo de este, recursos donde se implementara el sistema y el nivel de programación de los desarrolladores 

2.5 Atención y Dependencias

El sitio web dependerá del hosting y del proveedor de servicios de Internet para garantizar que el sitio sea accesible en todo momento. También se necesitará un equipo de desarrollo web para construir y mantener el sitio web, y un equipo de soporte técnico para resolver problemas técnicos que puedan surgir.

#### 3. Requerimientos Específicos 
        3.1 Requerimientos Funcionales.

| Código | Nombre                                      | Fecha        | Grado Necesidad |
|--------|---------------------------------------------|--------------|-----------------|
| REQ001 | Agregar-funciones prioritarias al carrito    | Sin especificar | ALTO             |

| Descripción | Entradas                                   | Fuente                                | Salida                                    | Destino                                   | Restricciones                                                                                                                |
|-------------|--------------------------------------------|--------------------------------------|-------------------------------------------|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Agregar funciones prioritarias al carrito. Esto incluye la capacidad de agregar productos al carrito de compras, actualizar la cantidad de productos en el carrito y eliminar productos del carrito. | El ID del producto que se desea agregar    | Base de datos de productos del sitio web | Actualización del número de productos en el carrito | Base de datos de compras del sitio web | El usuario debe haber iniciado sesión para poder agregar productos al carrito. |
| Proceso     | Validación del ID del producto             | Actualización del número de productos en el carrito y de la base de datos de compras del sitio web |                                             |                                           |                                                                  |
| Efecto Colateral | El tiempo de carga del sitio web puede aumentar si hay muchos productos en el carrito. |                                          |                                          |                                           |                                                                  |
<br>
<br>


| Código | Nombre                | Fecha      | Grado Necesidad |
|--------|----------------------|------------|----------------|
| REQ002 | Gestión de pedidos    | Sin fecha  | ALTO           |

| Descripción | El sistema debe permitir a los usuarios realizar pedidos de productos disponibles en el sitio web. Los usuarios deben poder agregar productos a su carrito de compras, ver un resumen de su pedido y realizar el pago. |
|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|

| Entradas    | Fuente         | Salida                                       | Destino       | Restricciones                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|-------------|----------------------|----------------------------------------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Información del producto seleccionado, dirección de envío, información de pago | Usuario final | Confirmación de pedido realizado exitosamente | Usuario final | El sistema debe permitir a los usuarios realizar cambios en su pedido antes de confirmar el pago, y solo se realizará el cobro después de que se haya confirmado el pago por completo. Además, el sistema debe asegurarse de que el inventario de productos sea suficiente para procesar los pedidos antes de permitir a los usuarios realizar el pago. |

| Proceso                                             | El sistema debe procesar el pedido del usuario, verificar la disponibilidad del producto en el inventario, enviar una confirmación de pedido al usuario y actualizar el inventario de productos.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

| Efecto Colateral                                                     | Si el inventario de productos no es suficiente para procesar los pedidos, el sistema debe notificar al usuario que el producto está temporalmente agotado y proporcionar una estimación de la fecha de disponibilidad del producto. Además, si el pago no se realiza correctamente, el sistema debe notificar al usuario y proporcionar una explicación de por qué el pago no se pudo procesar.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|----------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

<br>
<br>

                                                                                                                        
| Código | Nombre                    | Fecha       | Grado Necesidad |
|--------|---------------------------|-------------|-----------------|
| REQ003 | Búsqueda de productos     | [Fecha aquí] | ALTO            |

| Descripción   | El sistema debe permitir a los usuarios buscar productos en el sitio web mediante palabras clave o categorías. Los resultados de la búsqueda deben mostrar una imagen del producto, su nombre y precio. |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

| Entradas        | Fuente      | Salida                                                | Destino      | Restricciones                                                                                                            |
|-----------------|-------------|-------------------------------------------------------|--------------|--------------------------------------------------------------------------------------------------------------------------|
| Palabras clave o categorías | Usuario final | Lista de productos que coinciden con la búsqueda. | Usuario final | Los usuarios deben tener una cuenta en el sitio web para poder realizar una búsqueda avanzada por categorías. |

| Proceso                                                                                                                    |
|----------------------------------------------------------------------------------------------------------------------------|
| El sistema debe buscar en la base de datos los productos que coincidan con las palabras clave o categorías ingresadas por el usuario. |

| Efecto Colateral                                                                                                                                                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Si el número de productos encontrados es muy grande, se deben paginar los resultados para evitar sobrecargar la página y reducir el tiempo de carga. |


##### Especificación de Requerimientos
        3.2 Requerimientos No Funcionales

| Código  | Nombre                  | Fecha     | Grado Necesidad |
| ------- | -----------------------| ---------| --------------- |
| RNF-001 | Usabilidad del sitio web | -        | Alto            |

| Descripción                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- |
| El sitio web debe ser fácil de usar y navegar para los usuarios, permitiendo realizar compras de manera rápida y sencilla. |


<br>
<br>


| Código  | Nombre                          | Fecha     | Grado Necesidad |
|---------|--------------------------------|-----------|-----------------|
| RNF-002 | Velocidad de carga de la página | [Fecha]   | Alto            |

### Descripción
El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga.


<br>
<br>


| Código  | Nombre                    | Fecha | Grado Necesidad |
| ------- | ------------------------ | ----- | --------------- |
| RNF-003 | Seguridad de la información |       | Alto           |
|         | **Descripción:**          |       |                 |
|         | El sitio web debe garantizar la confidencialidad, integridad y disponibilidad de la información de los usuarios y de la propia empresa, protegiéndola de accesos no autorizados, robo o pérdida de datos. |       |                 |

<br>
<br>


# Especificación de Requerimientos.
## 
        Requerimientos de interfaz de usuario

| Código  | Nombre                                  | Fecha       | Grado Necesidad | Descripción                                                                                                                                                                                                                                                                                                                                                                           |
| ------- | --------------------------------------- | -----------| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| RUI-001 | Diseño de la página de inicio            | Sin definir | Alto            | Este requisito implica la creación de un diseño atractivo y llamativo para la página de inicio del sitio web, con una organización clara y fácil de navegar para los usuarios. Este diseño debe reflejar la marca y el propósito del sitio web. Se espera que el diseño tenga una apariencia profesional y coherente con la imagen de la marca. También debe ser fácil de usar y navegar, lo que puede implicar la implementación de funciones como menús de navegación, enlaces a páginas importantes y llamados a la acción para guiar a los usuarios hacia el contenido más relevante. |

<br>
<br>

| Código   | Nombre                                            | Fecha       | Grado Necesidad |
| :------: | :----------------------------------------------- | :---------: | :-------------: |
| RUI-002  | Botones de navegación claros y fáciles de usar    | -           | MEDIO           |

### Descripción
Este requisito implica la creación de botones de navegación claros y fáciles de usar, que permitan a los usuarios moverse por el sitio web de manera intuitiva. Los botones deben ser visibles y fácilmente identificables para el usuario.

<br>
<br>

| Código | Nombre                               | Fecha      | Grado Necesidad |
| ------ | ------------------------------------ | ----------| ----------------|
| RUI-03 | Funcionalidad de búsqueda en la página|         | Alto            |

**Descripción:**

Este requisito implica la incorporación de una función de búsqueda en el sitio web, que permita a los usuarios buscar contenido específico dentro del sitio. La función de búsqueda debe ser fácil de encontrar y utilizar, y debe proporcionar resultados precisos y relevantes.

<br>
<br>

# Especificación de Requerimientos.

###     
      4.0  Determinación de las tecnologías de hardware, software y servicios requeridos 
<br>
4.1 Software

    Lenguaje de programación: PHP
    Base de datos: MySQL
    Framework de desarrollo web: Laravel
    CMS: WordPress
    Plataforma de comercio electrónico: WooCommerce
    Servidor web: Apache
    Herramientas de desarrollo: Git, Visual Studio Code

4.2 Hosting

    Tipo de alojamiento: Hosting compartido o VPS
    Espacio de almacenamiento: 10 GB
    Ancho de banda: 50 GB/mes
    Proveedor de hosting: por determinar

4.3 Computador

    Procesador: Intel Core i7
    RAM: 8 GB
    Disco duro: 256 GB
    Sistema operativo: Windows 10 Pro

4.4 Escáner Lector Código de Barras Automático USB Soporte Base

    Marca: Honeywell
    Modelo: Voyager 1200g
    Conexión: USB

4.5 Router (Router Inalámbrico/Repetidor WiFi N300Mbps, Tp-Link TL-WR840N)

    Marca: TP-Link
    Modelo: TL-WR840N
    Tipo de conexión: Inalámbrica y por cable
    Velocidad de transmisión: N300Mbps

4.6 Presupuesto

El presupuesto estimado para la creación del sitio web es de 65.841.300 de pesos, incluyendo el diseño, la programación, el alojamiento web y la configuración del servidor. El presupuesto también incluye la compra de hardware necesario, como el escáner lector de códigos de barras y el router inalámbrico. Se estima que el tiempo de desarrollo del sitio web sea de aproximadamente 27 meses.