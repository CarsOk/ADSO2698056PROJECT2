# ESPECIFICACION DE REQUERIMIENTOS

## 1.Introducción

1.1 Propósito

El propósito del sitio web es crear una plataforma en línea para que los usuarios puedan acceder a información, servicios y productos del sitio web, describir lo acordado con el cliente y desarrollar el paso a paso para el software que servirá para ampliar el rango de venta de la farmacia, publicitar sus productos y generar mayores ganancias, generando un control y registro de las ventas.

1.2 Alcance 

El sistema será un sitio ventas web accesible a través de internet. El cual brindara una interfaz de usuarios y productos para que los usuarios puedan interactuar. Este sistema aportara en:
• Registro e inicio de usuarios
• Administración de los productos disponibles del inventario
• Generar factura electrónica
• Selección de productos y compra de los mismos

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

<br>
<br>
 
| Código | Nombre | Fecha | Grado | Necesidad |
| -------- | --------------------- | -------------- | ------ | ------------------------------------------------------- |
| REQ001 | Registro de usuario | Sin especificar| ALTO | |

| **Descripción** |                                                                                                                                                                                                                                                                      |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 | El sistema debe permitir que los usuarios se registren en la plataforma proporcionando su información personal.                                                                                                                                                      |
|                 |                                                                                                                                                                                                                                                                      |
|                 | **REQ001.1-CREACION DE CUENTA:** El sistema debe permitir a los visitantes registrarse como usuarios de la farmacia online. El usuario debe digitar sus datos personales como: ID, nombre, apellido, correo electrónico, contraseña, dirección y número de contacto. |
|                 |                                                                                                                                                                                                                                                                      |
|                 | **REQ001.2-VEREFICACION DE CORREO ELECTRONICO:** Después de que el usuario ha registrado sus datos personales, el sistema debe enviar un correo de verificación para confirmar el correo electrónico dado por el usuario.                                            |
|                 |                                                                                                                                                                                                                                                                      |
|                 | **REQ001.3-INICIO DE SESION:** El sistema debe permitir a los usuarios registrados iniciar sesión en la plataforma utilizando su ID y contraseña.                                                                                                                    |
|                 |                                                                                                                                                                                                                                                                      |
|                 | **REQ001.4-PERFIL DE USUARIO:** Los usuarios deben tener acceso a un perfil de usuario para que puedan editar su información personal, como dirección, número de contacto u otros datos de información.                                                              |

| **Entradas**                           | **Fuente** | **Salida**               | **Destino**         | **Restricciones**                                                                                             |
| -------------------------------------- | ---------- | ------------------------ | ------------------- | ------------------------------------------------------------------------------------------------------------- |
| Identificación, Contraseña del usuario | Usuario    | Confirmación de registro | Interfaz de usuario | Validación de correo (Si el usuario no confirma la verificación del correo electrónico, no podrá registrarse) |

| **Proceso**                                                                                                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| El usuario debe acceder a la página de registro de la plataforma, digitar sus datos personales, proporcionar una contraseña y confirmar el correo de verificación. Los datos del usuario se almacenan en la base de datos de la farmacia y se confirma su registro. |

| **Efecto Colateral**                                                                                                                                                                                                                                                                            |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Algunos usuarios pueden tener preocupaciones legítimas sobre la seguridad de sus datos y pueden ser reacios a proporcionar su información personal en línea. Esto puede conducir a una menor confianza en la farmacia en línea y a una menor participación de los usuarios o tasas de registro. |

<br>
<br>

####

| Código | Nombre             | Fecha           | Grado | Necesidad |
| ------ | ------------------ | --------------- | ----- | --------- |
| REQ002 | Carrito de compras | Sin especificar | ALTO  |           |

| **Descripción** |                                                                                                                                                                                                                                                                                           |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 | El sistema deberá de permitir al usuario la búsqueda de productos, deben poder seleccionar la cantidad de productos que desea, ver la descripción del producto, precio y disponibilidad.                                                                                                  |
|                 |                                                                                                                                                                                                                                                                                           |
|                 | **REQ002.1-AGREGAR PRODUCTOS AL CARRITO:** El usuario debe poder agregar productos al carrito. El sistema deberá permitir la actualización de la cantidad de los productos.                                                                                                               |
|                 |                                                                                                                                                                                                                                                                                           |
|                 | **REQ002.2-DISPONIBILIDAD DEL PRODUCTO:** El sistema deberá verificar si el producto se encuentra disponible para la compra antes de ser agregado al carrito. Si el producto no se encuentra disponible, el sistema deberá informar al usuario.                                           |
|                 |                                                                                                                                                                                                                                                                                           |
|                 | **REQ002.3-GESTION DEL CARRITO:** El usuario podrá ver el contenido actual del carrito de compras. El sistema deberá mostrar la lista de los productos, la cantidad, el precio unitario más el subtotal. El usuario debe poder modificar la cantidad del producto o eliminar el producto. |

| **Entradas**       | **Fuente**                     | **Salida**                     | **Destino**              | **Restricciones**                                                                                               |
| ------------------ | ------------------------------ | ------------------------------ | ------------------------ | --------------------------------------------------------------------------------------------------------------- |
| El ID del producto | Base de datos de los productos | Resumen del carrito de compras | Base de datos de compras | El usuario debe haber iniciado sesión para poder agregar productos al carrito. Disponibilidad de los productos. |

| **Proceso**                          |
| ------------------------------------ |
| Navegación y selección de productos. |

| **Efecto Colateral**                                                                   |
| -------------------------------------------------------------------------------------- |
| El tiempo de carga del sitio web puede aumentar si hay muchos productos en el carrito. |

<br>
<br>

####

| Código | Nombre                | Fecha           | Grado | Necesidad |
| ------ | --------------------- | --------------- | ----- | --------- |
| REQ003 | Búsqueda de productos | Sin especificar | ALTO  |           |

| **Descripción** |                                                                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 | El sistema debe permitir a los usuarios la capacidad de buscar productos farmacéuticos ya sea por el nombre del producto o la categoría.                                                                   |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.1-BUSQUEDA POR NOMBRE DE PRODUCTO:** El usuario debe poder buscar el producto que desea ingresando el nombre del producto y el sistema debe poder devolver resultados relevantes.                 |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.2-BUSQUEDA POR CATEGORIAS:** El sistema le debe permitir al usuario buscar productos por categorías como: salud y medicamentos, cuidado y aseo personal, maquillaje, maternidad y bebes, ofertas. |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.3-VISTA PREVIA DE PRODUCTOS:** Los usuarios deben poder ver la vista previa de los productos en los resultados de búsqueda junto a la información, marca y precio del producto.                   |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.4-SUGERENCIA DE BÚSQUEDA:** El sistema debe mostrar sugerencias de búsqueda cuando el usuario escribe basándose en términos relacionados y popularidad.                                           |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.5-HISTORIAL DE BÚSQUEDA:** El usuario puede tener acceso al historial de búsqueda de los productos que anteriormente ha buscado.                                                                  |
|                 |                                                                                                                                                                                                            |
|                 | **REQ003.6-INTEGRACION DEL CARRITO DE COMPRAS:** Los usuarios deben poder agregar los productos directamente desde los resultados de la búsqueda al carrito de compras.                                    |

| **Entradas**                 | **Fuente**                 | **Salida**                                               | **Destino**   | **Restricciones**                                                                               |
| ---------------------------- | -------------------------- | -------------------------------------------------------- | ------------- | ----------------------------------------------------------------------------------------------- |
| Palabras claves o categorías | Base de datos de productos | Lista de resultados de búsqueda con productos relevantes | Usuario final | Capacidad del sistema para mostrar resultados de manera eficiente. Disponibilidad del producto. |

| **Proceso**                                                                                                                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| El usuario digita palabras claves o elige una categoría de productos, y el sistema le muestra resultados relevantes a su búsqueda, mostrando una vista previa de los productos que coinciden con su búsqueda. El usuario puede agregar el producto buscado a su carrito de compras. |

| **Efecto Colateral**                                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Puede haber sobrecarga del servidor en momentos de alta demanda y mostrar resultados irrelevantes o productos agotados si no se actualiza debidamente el inventario. |

<br>
<br>

####

| Código | Nombre             | Fecha     | Grado Necesidad |
| ------ | ------------------ | --------- | --------------- |
| REQ004 | Gestión de pedidos | Sin fecha | ALTO            |

| Descripción | El sistema debe permitir a los usuarios realizar pedidos de productos disponibles en el sitio web. Los usuarios deben poder agregar productos a su carrito de compras, ver un resumen de su pedido y realizar el pago. |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

| Entradas                                                                       | Fuente        | Salida                                        | Destino       | Restricciones                                                                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------ | ------------- | --------------------------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Información del producto seleccionado, dirección de envío, información de pago | Usuario final | Confirmación de pedido realizado exitosamente | Usuario final | El sistema debe permitir a los usuarios realizar cambios en su pedido antes de confirmar el pago, y solo se realizará el cobro después de que se haya confirmado el pago por completo. Además, el sistema debe asegurarse de que el inventario de productos sea suficiente para procesar los pedidos antes de permitir a los usuarios realizar el pago. |

| Proceso | El sistema debe procesar el pedido del usuario, verificar la disponibilidad del producto en el inventario, enviar una confirmación de pedido al usuario y actualizar el inventario de productos. |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |

| Efecto Colateral | Si el inventario de productos no es suficiente para procesar los pedidos, el sistema debe notificar al usuario que el producto está temporalmente agotado y proporcionar una estimación de la fecha de disponibilidad del producto. Además, si el pago no se realiza correctamente, el sistema debe notificar al usuario y proporcionar una explicación de por qué el pago no se pudo procesar. |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

<br>
<br>

####

| Código | Nombre             | Fecha           | Grado | Necesidad |
| ------ | ------------------ | --------------- | ----- | --------- |
| REQ005 | Sistema de entrega | Sin especificar | ALTO  |           |

| **Descripción** |                                                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
|                 | Este sistema debe facilitar el servicio de entrega del producto al usuario que lo compró.                                             |
|                 |                                                                                                                                       |
|                 | **REQ004.1-SERVICIO DE MENSAJERÍA:** El sistema debe integrarse con servicios de mensajería para facilitar la entrega de los pedidos. |
|                 |                                                                                                                                       |
|                 | **REQ004.2-CÁLCULO DE COSTOS DE ENVÍO:** El sistema debe calcular automáticamente los costos de envío para cada pedido.               |

| **Entradas**       | **Fuente**             | **Salida**              | **Destino**                   | **Restricciones**                                   |
| ------------------ | ---------------------- | ----------------------- | ----------------------------- | --------------------------------------------------- |
| Pedido del cliente | Servicio de mensajería | Confirmación de pedidos | Ubicación dada por el usuario | Regulaciones de envío. Disponibilidad de productos. |

| **Proceso**                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Al momento de ser entregado el producto al domiciliario, se debe verificar que el producto sea actualizado y marcado en la base de datos de la farmacia. |

| **Efecto Colateral**                                                      |
| ------------------------------------------------------------------------- |
| Puede haber retraso al momento de recibir muchos pedidos al mismo tiempo. |

<br>
<br>

####

| Código | Nombre                    | Fecha           | Grado | Necesidad |
| ------ | ------------------------- | --------------- | ----- | --------- |
| REQ006 | Consultas y asesoramiento | Sin especificar | ALTO  |           |

| **Descripción** |                                                                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 | Brindar a los usuarios la opción de realizar consultas o solicitar asesoramiento farmacéutico en línea a través de un sistema de chat en vivo o correo electrónico.                                        |
|                 |                                                                                                                                                                                                            |
|                 | **REQ005.1-CONSULTA EN LÍNEA:** El usuario podrá realizar consultas en línea sobre medicamentos, efectos secundarios, dosis recomendadas, productos, etc.                                                  |
|                 |                                                                                                                                                                                                            |
|                 | **REQ005.2-ASESORAMIENTO FARMACEUTICO:** El usuario recibirá asesoramiento personalizado por el farmacéutico autorizado. El asesoramiento se realizará por medio de un chat en línea o llamada telefónica. |

| **Entradas**         | **Fuente**                                         | **Salida**                 | **Destino**   | **Restricciones**                |
| -------------------- | -------------------------------------------------- | -------------------------- | ------------- | -------------------------------- |
| Consultas de usuario | Conocimiento y experiencia del equipo farmacéutico | Respuestas y asesoramiento | Usuario final | Limitaciones de responsabilidad. |

| **Proceso**                                                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| El usuario realiza la consulta por uno de los medios de asesoramiento disponibles. El farmacéutico autorizado realiza el análisis y evaluación de la consulta y envía la respuesta y asesoramiento al cliente. |

| **Efecto Colateral**                 |
| ------------------------------------ |
| Posibles retrasos en las respuestas. |

##### Especificación de Requerimientos

        3.2 Requerimientos No Funcionales

| Código  | Nombre                   | Fecha | Grado Necesidad |
| ------- | ------------------------ | ----- | --------------- |
| RNF-001 | Usabilidad del sitio web | -     | Alto            |

| Descripción                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------- |
| El sitio web debe ser fácil de usar y navegar para los usuarios, permitiendo realizar compras de manera rápida y sencilla. |

<br>
<br>

| Código  | Nombre                          | Fecha   | Grado Necesidad |
| ------- | ------------------------------- | ------- | --------------- |
| RNF-002 | Velocidad de carga de la página | [Fecha] | Alto            |

### Descripción

El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga.

<br>
<br>

| Código  | Nombre                                                                                                                                                                                                    | Fecha | Grado Necesidad |
| ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- | --------------- |
| RNF-003 | Seguridad de la información                                                                                                                                                                               |       | Alto            |
|         | **Descripción:**                                                                                                                                                                                          |       |                 |
|         | El sitio web debe garantizar la confidencialidad, integridad y disponibilidad de la información de los usuarios y de la propia empresa, protegiéndola de accesos no autorizados, robo o pérdida de datos. |       |                 |

<br>
<br>

# Especificación de Requerimientos.

##

        Requerimientos de interfaz de usuario

| Código  | Nombre                        | Fecha       | Grado Necesidad | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------- | ----------------------------- | ----------- | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RUI-001 | Diseño de la página de inicio | Sin definir | Alto            | Este requisito implica la creación de un diseño atractivo y llamativo para la página de inicio del sitio web, con una organización clara y fácil de navegar para los usuarios. Este diseño debe reflejar la marca y el propósito del sitio web. Se espera que el diseño tenga una apariencia profesional y coherente con la imagen de la marca. También debe ser fácil de usar y navegar, lo que puede implicar la implementación de funciones como menús de navegación, enlaces a páginas importantes y llamados a la acción para guiar a los usuarios hacia el contenido más relevante. |

<br>
<br>

| Código  | Nombre                                         | Fecha | Grado Necesidad |
| :-----: | :--------------------------------------------- | :---: | :-------------: |
| RUI-002 | Botones de navegación claros y fáciles de usar |   -   |      MEDIO      |

### Descripción

Este requisito implica la creación de botones de navegación claros y fáciles de usar, que permitan a los usuarios moverse por el sitio web de manera intuitiva. Los botones deben ser visibles y fácilmente identificables para el usuario.

<br>
<br>

| Código | Nombre                                 | Fecha | Grado Necesidad |
| ------ | -------------------------------------- | ----- | --------------- |
| RUI-03 | Funcionalidad de búsqueda en la página |       | Alto            |

**Descripción:**

Este requisito implica la incorporación de una función de búsqueda en el sitio web, que permita a los usuarios buscar contenido específico dentro del sitio. La función de búsqueda debe ser fácil de encontrar y utilizar, y debe proporcionar resultados precisos y relevantes.

<br>
<br>

# Especificación de Requerimientos.

###

      4.0  Determinación de las tecnologías de hardware, software y servicios requeridos

<br>
4.1 Software

    Lenguaje de programación: Java
    Base de datos: MySQL
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

4.4 Presupuesto

Al ser un proyecto educativo no se cuenta con un presupuesto. la institucion brinda los recursos necesarios para la realizacion del proyecto. (cualquier tecnologia o recurso direferente a la brindada por la institucion y que se quiera implementar al software sera presupuestada por el cliente).
