# INFORME DEL ANALISIS

| Fecha      | Version | Descripcion/cambios | Autor                                                                                    |
| ---------- | ------- | ------------------- | ---------------------------------------------------------------------------------------- |
| 11/07/2023 | 1.0     | primer documento    | Dariana Ruiz, Luis Cortezano, Andrés Padilla,Nehemías Yepes, Samuel Buzón, Abel Martínez |

### **1. Propósito**

El propósito es describir mediante diagramas el funcionamiento y requerimientos del software, también a identificar los actores que intervendrán en el software y las respectivas funciones que realizarán en el sistema.

### **2. Alcance**

El sistema será un sitio ventas web accesible a través de internet. El cual brindara una interfaz de usuarios y productos para que los usuarios puedan interactuar.
Este sistema aportara en:

• Registro e inicio de sesión de usuarios

• Administración de los productos disponibles del inventario

• Generar factura electrónica

• Selección de productos y compra de los mismos

### **3. Definiciones, Acrónimos, y Abreviaturas**

Actor: entidad que guarda una relación con el sistema y que le demanda una funcionalidad.

PQR: peticiones, quejas y reclamos.

RF/ REQ: requerimientos funciónales

RFN /RNF: requerimientos no funcionales.

Caso de Uso: es una técnica para la captura de requisitos de un nuevo sistema.

### **4. Personal**

| Nombre         | Correo                            | Telefono   |
| -------------- | --------------------------------- | ---------- |
| Dariana Ruiz   | darianaruizmontes@gmail.com       | 3024486683 |
| Luis Cortezano | luisdavidcortezano@gmail.com      | 3246794400 |
| Andrés Padilla | Andrespadillat27@gmail.com        | 3127268142 |
| Nehemías Yepes | nyeres02102006@gmail.com          | 3160412212 |
| Samuel Buzón   | buzonsamuel18@gmail.com           | 3003191165 |
| Abel Martínez  | martinezmattosabeljesus@gmail.com | 3243316646 |

### **5. Situación Actual**

La farmacia actualmente lleva desde la gestión del inventario hasta la atención al cliente y el seguimiento de ventas de manera manual. Esta falta de un sistema en línea genera dificultades para administrar sus operaciones y, como resultado, experimentar una disminución en la eficiencia y la eficacia. Además, enfrenta problemas para satisfacer las expectativas de los clientes que buscan comodidad y rapidez en el proceso de compra de medicamentos. La falta de un sistema en línea dificulta ofrecer servicios adicionales y adaptarse a las tendencias del mercado digital, lo que puede afectar su competitividad en comparación con otras farmacias en línea.

### **6. Perspectiva del Producto**

Con este proyecto se espera una mejora en las ventas de la farmacia, dicho sistema brindara facilidad al usuario en la compra de productos y obtención de la información de estos, a tener un mayor alcance de clientes, ahorro de tiempo y comodidad al no tener que desplazarse a la farmacia física.

### **7. Funciones del Producto**

• Módulo de gestión de usuario.

• Módulo de inicio de sesión.

• Módulo de búsqueda de producto.

• Módulo de Carrito de compras.

• Módulo de pago para compras en línea.

• Generar factura electrónica de las compras que se realicen.

• Módulo de PQR.

• Módulo de publicidad.

### **8. Características de Usuario**

El sistema cuenta con tres tipos de usuario

Empleado: se encargará de la administración del sistema.

Cliente: realizara compras y consultas.

Administrador: se asegura del correcto funcionamiento y gestión de la plataforma.

### **9. Requerimientos Funcionales**

| Codigo | Nombre                  |
| ------ | ----------------------- |
| RF-001 | Registro de usuario     |
| RF-002 | Inicio de sesión        |
| RF-003 | Búsqueda de productos   |
| RF-004 | Carrito de compras      |
| RF-005 | Pago de compra en línea |
| RF-006 | Factura electrónica     |
| RF-007 | PQR                     |
| RF-008 | Publicidad              |

|                                        | Código                                                                                                                                                                                                                                                                                         | Nombre                   | Fecha               | Grado Necesidad                                                                                              |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ------------------- | ------------------------------------------------------------------------------------------------------------ |
| REQ001                                 | gestión de usuario                                                                                                                                                                                                                                                                             | Sin especificar          | ALTO                |
| Descripcion:                           | El sistema debe permitir que los usuarios se registren en la plataforma proporcionando su información personal.                                                                                                                                                                                |
|                                        | REQ001. 1-CREACION DE CUENTA: el sistema debe permitir a los visitantes registrarse como usuarios de la farmacia online. El usuario debe digitar sus datos personales como: ID, nombre, apellido, correo electrónico, contraseña, dirección y número de contacto.                              |
|                                        | REQ001. 2-VEREFICACION DE CORREO ELECTRONICO: después de que el usuario a registrado sus datos personales el sistema debe enviar un correo de verificación para confirmar el correo electrónico dado por el usuario.                                                                           |
|                                        | REQ0001. 3-INICIO DE SESION: el sistema debe permitir a los usuarios registrados iniciar sesión en la plataforma utilizando su ID y contraseña.                                                                                                                                                |
|                                        | REQ001. 4-PERFIL DE USUARIO: los usuarios deben tener acceso a un perfil de usuario para que puedan editar su información personal como dirección, número de contacto u otros datos de información.                                                                                            |
| Entradas                               | Fuente                                                                                                                                                                                                                                                                                         | Salida                   | Destino             | Restricciones                                                                                                |
| Identificación, Contraseña del usuario | usuario                                                                                                                                                                                                                                                                                        | Confirmación de registro | Interfaz de usuario | Validación de correo (Si el usuario no confirma la verificación del correo electrónico no podrá registrarse) |
| Proceso                                | el usuario debe acceder a la página de registro de la plataforma, digitar sus datos personales proporcionar una contraseña, confirmar el correo de verificación. Los datos del usuario se almacenan en la base de datos de la farmacia y se confirma su registro                               |
| Efecto colateral                       | Algunos usuarios pueden tener preocupaciones legítimas sobre la seguridad de sus datos y pueden ser reacios a proporcionar su información personal en línea. Esto puede conducir a una menor confianza en la farmacia en línea y a una menor participación de los usuarios o tasas de registro |

| Código       | Nombre                                                                                                                                                                                                        | Fecha           | Grado Necesidad |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| REQ002       | Inicio de sesión.                                                                                                                                                                                             | Sin especificar | ALTO            |
| Descripcion: | REQ002.1- INICIO DE SESION: el sistema debe permitir a los usuarios registrados iniciar sesión en la plataforma utilizando su ID y contraseña.                                                                |
|              | REQ002.2- RETABLECIMIENTO DE CONTRASEÑA: El sistema debe permitir al usuario el restablecimiento de su contraseña en caso de olvidarla, mediante un link de restablecimiento enviado a su correo electrónico. |

|                              | Código                                                                                                                                                                                                        | Nombre                                                     | Fecha         | Grado Necesidad                                                                                    |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- | ------------- | -------------------------------------------------------------------------------------------------- |
| REQ003                       | Búsqueda de productos                                                                                                                                                                                         | Sin especificar                                            | ALTO          |
| Descripcion:                 | El sistema debe permitir a los usuarios la capacidad de buscar productos farmacéuticos ya sea por el nombre del producto o la categoría.                                                                      |
|                              | REQ003. 1-BUSQUEDA POR NOMBRE DE PRODUCTO: El usuario de poder buscar el producto que desea ingresando el nombre del producto y el sistema debe poder de volver resultados relevantes.                        |
|                              | REQ003. 2-BUSQUEDA POR CATEGORIAS: El sistema le debe permitir al usuario poder buscar productos por categorías como: salud y medicamentos, cuidado y aseo personal, maquillaje, maternidad y bebes, ofertas. |
|                              | REQ003. 3-VISTA PEREVIA DE PRIDUCTOS: los usuarios deben poder ver la vista previa de los productos en los resultados de búsqueda junto a la información, marca y precio del producto.                        |
|                              | REQ003. 4-SUGERENCIA DE BÚSQUEDA: El sistema debe mostrar sugerencias de búsqueda, cuando el usuario escribe basándose en términos relacionados y popularidad.                                                |
|                              | REQ003. 5-HISTORIAL DE BÚSQUEDA: El usuario puede tener acceso al historial de búsqueda de los productos que anteriormente ha buscado.                                                                        |
|                              | REQ003. 6-INTEGRACION DEL CARRITO DE COMPRAS: los usuarios deben poner agregar los productos directamente desde el resultado de la búsqueda al carrito de compras.                                            |
| Entradas                     | Fuente                                                                                                                                                                                                        | Salida                                                     | Destino       | Restricciones                                                                                      |
| Palabras claves o categorias | Base de datos de productos                                                                                                                                                                                    | La Lista de resultado de búsqueda con productos relevantes | usuario final | La Capacidad del sistema para mostrar resultados de manera eficiente. Disponibilidad del producto. |

| Código       | Nombre                                                                                                                                                                                                                                                                             | Fecha           | Grado Necesidad |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| REQ004       | Carrito de compras                                                                                                                                                                                                                                                                 | Sin especificar | ALTO            |
| Descripcion: | El sistema deberá de permitir al usuario la búsqueda de productos, deben poder seleccionar la cantidad de productos que desea, ver la descripción del producto, precio y disponibilidad                                                                                            |
|              | REQ004.1-AGREGAR PRODUCTOS AL CARRITO: el usuario debe poder agregar productos al carrito.El sistema deberá permitir la actualización de la cantidad de los productos.                                                                                                             |
|              | REQ004.2-DISPONIBILIDAD DEL PRODUCTO: el sistema deberá verificar si el producto se encuentra disponible para la compra antes de ser agregado al carrito. Si el producto no se encuentra disponible el sistema deberá informar al usuario.                                         |
|              | REQ004.3-GETION DEL CARRITO: el usuario podrá ver el contenido actual de carrito de compras.El sistema deberá mostrar la lista de los productos, la cantidad, el precio unitario más el subtotal, El usuario debe poder modificar la cantidad del producto o eliminar el producto. |

| Código       | Nombre                                                                                                                                                                     | Fecha           | Grado Necesidad |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| REQ005       | pago de compras en línea.                                                                                                                                                  | Sin especificar | ALTO            |
| Descripcion: | REQ005.1-PROCESIMIENTO DE SEGURO DE PAGO: el sistema debe garantizar que la información del usuario se maneje de forma segura y que se cumplan los estándares de seguridad |
|              | REQ005.2- INTEGRANCION DE METODOS DE PAGO: debe permitir la integración de varios métodos de pago                                                                          |
|              | REQ005.3-REEMBOLSO: debe permitir que los usuarios realicen reembolsos para las compras devueltas o canceladas.                                                            |

| Código       | Nombre                                                                                                                                                                                                                                   | Fecha           | Grado Necesidad |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| REQ006       | Factura electronica                                                                                                                                                                                                                      | Sin especificar | ALTO            |
| Descripcion: | REQ006.1-GENERACION AUTOMÁTICA DE FACTURA: el sistema de generar automáticamente facturas electrónicas al momento que la compra se haya realizado exitosamente                                                                           |
|              | REQ006.2-DETALLES DE COMPRA: la factura de electrónica deber contener detalles específicos de la compra, como el nombre del producto, precio unitario, descuentos aplicados, impuestos, descripción de la compra y el total de la compra |
|              | REQ006.3-ENVIO AUTOMATICO DE LA FACTURA: El sistema debe enviar automáticamente la factura al correo del usuario                                                                                                                         |
|              | REQ006.4-HISTORIAL DE FACURACION: el sistema debe permitir que tanto el usuario como el empleado pueda acceder en cualquier momento al historial completo de las facturas generadas                                                      |

|                       | Código                                                                                                                                                                                                           | Nombre                     | Fecha   | Grado Necesidad                 |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- | ------- | ------------------------------- |
| REQ007                | PQR                                                                                                                                                                                                              | Sin especificar            | ALTO    |
| Descripcion:          | Brindar a los usuarios la opción de realizar consultas o solicitar asesoramiento farmacéutico en línea a través de un sistema de chat en vivo o correo electrónico.                                              |
|                       | REQ007.1-CONSULTA EN LÍNEA: el usuario podrá realizar consultas en línea sobre medicamentos, efectos segundarios, dosis recomendadas, productos, etc.                                                            |
|                       | REQ007.2-ASESORAMIENTO FARMACEUTICO: el usuario recibirá asesoramiento personalizado por el farmacéutico autorizado, el asesoramiento se realizará por medio de un chat en línea o llamada telefónica.           |
| Entradas              | Fuente                                                                                                                                                                                                           | Salida                     | Destino | Restricciones                   |
| Consultas de usuarios | Conocimiento y experiencia del equipo farmaceutico                                                                                                                                                               | Respuestas y asesoramiento | usuario | Limitaciones de responsabilidad |
| Proceso               | El usuario realiza la consulta por uno de los medios de asesoramiento disponibles, el farmacéutico autorizado realizara el análisis y evaluación de la consulta e envira la respuesta y asesoramiento al cliente |
| Efecto colateral      | Posibles retrasos en las respuestas                                                                                                                                                                              |

| Código       | Nombre                                                                                                                                                                                  | Fecha           | Grado Necesidad |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| REQ008       | Publicidad                                                                                                                                                                              | Sin especificar | ALTO            |
| Descripcion: | REQ008.1- ANUNCIOS DESTACADOS: Permitir a los proveedores o marcas asociadas a la farmacia destacar ciertos productos o promociones mediante anuncios patrocinados.                     |
|              | REQ008.2-OFERTAS Y PROMOCIONES: Mostrar anuncios y notificaciones de ofertas y promociones especiales para atraer a los clientes y aumentar las ventas.                                 |
|              | REQ008.3-INTEGRACIÓN CON REDES SOCIALES: Permitir que los clientes compartan o interactúen con anuncios en las redes sociales para aumentar la viralidad y el alcance de la publicidad. |

### **10. Requerimientos No Funcionales**

| Código       | Nombre                                                                                                                         | Fecha           | Grado Necesidad |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------- | --------------- |
| RFN-001      | Usabilidad del sitio web                                                                                                       | Sin especificar | ALTO            |
| Descripcion: | El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga. |

| Código       | Nombre                                                                                                                         | Fecha           | Grado Necesidad |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------- | --------------- |
| RFN-002      | Velocidad de carga de la página                                                                                                | Sin especificar | ALTO            |
| Descripcion: | El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga. |

| Código       | Nombre                                                                                                                                                                                                    | Fecha           | Grado Necesidad |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| RFN-003      | Seguridad de la información                                                                                                                                                                               | Sin especificar | ALTO            |
| Descripcion: | El sitio web debe garantizar la confidencialidad, integridad y disponibilidad de la información de los usuarios y de la propia empresa, protegiéndola de accesos no autorizados, robo o pérdida de datos. |

| Código       | Nombre                                                                                                                 | Fecha           | Grado Necesidad |
| ------------ | ---------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| RFN-004      | Disponibilidad                                                                                                         | Sin especificar | ALTO            |
| Descripcion: | El sistema debe estar disponible para el usuario en todo momento, minimizando el tiempo de inactividad no planificado. |

| Código       | Nombre                                                                                                               | Fecha           | Grado Necesidad |
| ------------ | -------------------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| RFN-005      | Privacidad y protección de datos                                                                                     | Sin especificar | ALTO            |
| Descripcion: | establecerse políticas claras de privacidad y protección de datos para proteger la información personal del usuario. |

| Código       | Nombre                                                                                                     | Fecha           | Grado Necesidad |
| ------------ | ---------------------------------------------------------------------------------------------------------- | --------------- | --------------- |
| RNF-006      | mantenibilidad                                                                                             | Sin especificar | ALTO            |
| Descripcion: | El sistema debe ser fácil de mantener y actualizar para agregar nuevas funcionalidades o corregir errores. |

### **Modelo Entidad Relación**

![Diagrama MER](diagramas\MER.jpg)

### **Diagramas de casos de uso**

![Casos de Uso](diagramas\CduFamaciaOnline.jpg)
![Caso de uso Gestion de usuario](diagramas\CduGestUsuario.jpg)
![Caso de uso Inicio de sesion](diagramas\CduIniSesion.jpg)
![Caso de uso Gestion de productos](diagramas\CduGestProducto.jpg)
![Caso de uso Gestion carro de compras](diagramas\CduGestCarroComp.jpg)
![Caso de uso Gestion de inventario](diagramas\CduGestInventario.jpg)
![Caso de usoPQR](diagramas\CduPQR.jpg)
![Caso de uso gestion de proveedores](diagramas\CduGestProveedr.jpg)

|                | CASO DE USO                                                                                                                                                       | GESTION DE USUARIO |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ |
| Descripcion    | Este es el sistema dedicado únicamente para el inicio de sesión del cliente, mostrando ese detalle, los pasos que se necesitan para un correcto inicio de sesión. |
| Precondicion   | El cliente debe estar regristrado en la base de datos antes de iniciar sesión.                                                                                    |
| Secuencion     | PASO                                                                                                                                                              | Acción             |
| ---            | 1. El cliente ingresa el nombre y contraseña                                                                                                                      |
| ---            | 2. El sistema valida los datos.                                                                                                                                   |
| ---            | 3. Si los datos son incorrectos el sistema le da otra oportunidad al cliente para volver a escribir los datos.                                                    |
| ---            | 4. Una vez validado los datos el cliente ingresa a la pagina web.                                                                                                 |
| Post condición | Luego de iniciar sesión el cliente tiene acceso a los productos farmaceuticos de la pagina web.                                                                   |
| Excepciones    | PASO                                                                                                                                                              | Acción             |
| ---            | 1. Si el cliente no esta registrado o el correo electrónico ya ha sido previamente registrado por otro cliente, no se puede iniciar sesión.                       |

|                | CASO DE USO                                                                                              | GESTION DE PRODUCTOS |
| -------------- | -------------------------------------------------------------------------------------------------------- | -------------------- |
| Descripcion    | De esta manera el sistema puede saber que productos esta seleccionando el usuario.                       |
| Precondicion   | El usuario busca productos.                                                                              |
| Secuencion     | PASO                                                                                                     | Acción               |
| ---            | 1. El usuario oprime el buscador.                                                                        |
| ---            | 2. Luego el usuario escribe el nombre del producto que desea buscar.                                     |
| ---            | 3. El sistema analiza el nombre del producto y lo encuentra.                                             |
| Post condición | Si el cliente escribio correctamente el nombre del producto el sistema lo habra encontrado exitosamente. |
| Excepciones    | PASO                                                                                                     | Acción               |
| ---            | 1. Si el cliente escribió incorrectamente el nombre del producto el sistema no lo encontrara.            |

|                | CASO DE USO                                                                                      | GESTION DE CARRITO |
| -------------- | ------------------------------------------------------------------------------------------------ | ------------------ |
| Descripcion    | De esta manera podremos identificar los productos que el cliente ha seleccionado.                |
| Precondicion   | Que el cliente allá seleccionado los productos previamente.                                      |
| Secuencion     | PASO                                                                                             | Acción             |
| ---            | 1. Luego de haber buscado los productos el cliente deberá seleccionar los productos.             |
| ---            | 2. El sistema identifica los productos y los ingresa al carrito                                  |
| Post condición | Si el cliente seleccionó los productos el sistema ya abra ingresado los productos en el carrito. |
| Excepciones    | PASO                                                                                             | Acción             |
| ---            | 1. Si el cliente no selecciona los productos el sistema no los ingresa al carrito.               |

|                | CASO DE USO                                                                                                              | PQR    |
| -------------- | ------------------------------------------------------------------------------------------------------------------------ | ------ |
| Descripcion    | El cliente y administrador tienen una relación en el tema de consultar y asesorar.                                       |
| Precondicion   | El administrador debe de estar preparado para cualquier consulta que haga el cliente.                                    |
| Secuencion     | PASO                                                                                                                     | Acción |
| ---            | 1. El cliente hace una consulta.                                                                                         |
| ---            | 2. El administrador asesora.                                                                                             |
| Post condición | Si la información otorgada por el administrador hacia el cliente fue la indicada el cliente debería sentirse satisfecho. |
| Excepciones    | PASO                                                                                                                     | Acción |
| ---            | 1. Si la pregunta del cliente no es la adecuada el administrador no podrá responder.                                     |

|                | CASO DE USO                                                                                                                                                    | GESTION DE INVENTARIO |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| Descripcion    | El administrador proporciona suministros a la droguería lo cual indica un cambio en la base de datos lo cual es actualizado por el sistema.                    |
| Precondicion   | El administrador debe hacer un cambio en la droguería para que esto suceda.                                                                                    |
| Secuencion     | PASO                                                                                                                                                           | Acción                |
| ---            | 1. El administrador proporciona suministros a la droguería.                                                                                                    |
| ---            | 2. El administrador le da instrucciones al sistema para que este mismo actualice la base de datos del inventario.                                              |
| Post condición | El sistema ya habrá actualizado la base de datos del inventario una vez el administrador le allá otorgado las indicaciones.                                    |
| Excepciones    | PASO                                                                                                                                                           | Acción                |
| ---            | 1. Para que el sistema actualice la base de datos el administrador debe darle las instrucciones sobre qué productos específicamente proporcionó al inventario. |

|                | CASO DE USO                                                                                                                                    | GESTION DE PROVEEDORES |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
| Descripcion    | Asumir un servicio por parte del personal administrativo en el área de los suministros o mercancía de la droguería a manos de los proveedores. |
| Precondicion   | Que se allá levado un acuerdo con el proveedor antes de interactuar con la mercancía.                                                          |
| Secuencion     | PASO                                                                                                                                           | Acción                 |
| ---            | 1. Identificación de los bienes y servicios que se necesitan.                                                                                  |
| ---            | 2. Creación de la solicitud de compra                                                                                                          |
| ---            | 3. Revisión y aprobación de la solicitud de compra.                                                                                            |
| ---            | 4. Solicitud de propuesta a los proveedores.                                                                                                   |
| ---            | 5. Negociación del contrato y aprobación.                                                                                                      |
| ---            | 6. Envío y recibo del producto o servicio solicitado.                                                                                          |
| ---            | 7. Revisión y comparación con lo solicitado.                                                                                                   |
| ---            | 8. Aprobación y pago de facturas.                                                                                                              |
| ---            | 9. Actualización de registros contables.                                                                                                       |
| Post condición | Si el negocio con el proveedor resultó exitoso se le podrá hacer mas pedidos a largo plazo.                                                    |
| Excepciones    | PASO                                                                                                                                           | Acción                 |
| ---            | 1. Si no hay capital no se puede llevara cabo un trato con el proveedor.                                                                       |
| ---            | 2. Si ya hay mercancía o productos de algo especifico no es necesario llamar un proveedor para reponerlos.                                     |

### **Diagramas de actividades**

### **Gestión de usuario**

![Gestion de usuario](diagramas\GestUsuarios.jpg)

### **Inicio de sesión**

![Inicio de sesion](diagramas\InicdSesion.jpg)

### **Gestión de productos**

![Gestion de Productos](diagramas\GestProductos.jpg)

### **Gestión de pedidos**

![Gestion de pedidos](diagramas\GestPedidos.jpg)

### **PQR**

![PQR](diagramas\PQR.jpg)

### **Gestión de inventario**

![Gestion de inventario](diagramas\GestInventario.jpg)

### **Gestión de proveedores**

![Gestion de Proveedores](diagramas\GestProveedores.jpg)

### **Diagramas de clases (UML)**

![Diagrama de Clases ](diagramas\DigClases.jpg)
