# INFORME DEL ANALISIS 

| Fecha | Version | Descripcion/cambios | Autor  |
|----|-----|-----|----|
| 11/07/2023 | 1.0 | primer documento | Dariana Ruiz, Luis Cortezano, Andrés Padilla,Nehemías Yepes, Samuel Buzón, Abel Martínez |


### **1.	Propósito**
El propósito es describir mediante diagramas el funcionamiento y requerimientos del software, también a identificar los actores que intervendrán en el software y las respectivas funciones que realizarán en el sistema.

### **2.	Alcance**
El sistema será un sitio ventas web accesible a través de internet. El cual brindara una interfaz de usuarios y productos para que los usuarios puedan interactuar.
 Este sistema aportara en: 

• Registro e inicio de sesión de usuarios

• Administración de los productos disponibles del inventario

• Generar factura electrónica 

• Selección de productos y compra de los mismos

### **3.	Definiciones, Acrónimos, y Abreviaturas**

Actor: entidad que guarda una relación con el sistema y que le demanda una funcionalidad.

PQR: peticiones, quejas y reclamos.

RF/ REQ: requerimientos funciónales

RFN /RNF: requerimientos no funcionales.

Caso de Uso: es una técnica para la captura de requisitos de un nuevo sistema.

### **4.	Personal**

| Nombre | Correo | Telefono |
|-----|----|-----|
|Dariana Ruiz | darianaruizmontes@gmail.com | 3024486683
| Luis Cortezano | luisdavidcortezano@gmail.com | 3246794400 |
| Andrés Padilla | Andrespadillat27@gmail.com | 3127268142 |
| Nehemías Yepes | nyeres02102006@gmail.com | 3160412212 | 
| Samuel Buzón | buzonsamuel18@gmail.com | 3003191165 |
| Abel Martínez | martinezmattosabeljesus@gmail.com | 3243316646 |

### **5.	Situación Actual**

La farmacia actualmente lleva desde la gestión del inventario hasta la atención al cliente y el seguimiento de ventas de manera manual. Esta falta de un sistema en línea genera dificultades para administrar sus operaciones y, como resultado, experimentar una disminución en la eficiencia y la eficacia. Además, enfrenta problemas para satisfacer las expectativas de los clientes que buscan comodidad y rapidez en el proceso de compra de medicamentos. La falta de un sistema en línea dificulta ofrecer servicios adicionales y adaptarse a las tendencias del mercado digital, lo que puede afectar su competitividad en comparación con otras farmacias en línea.

### **6.	Perspectiva del Producto**

Con este proyecto se espera una mejora en las ventas de la farmacia, dicho sistema brindara facilidad al usuario en la compra de productos y obtención de la información de estos, a tener un mayor alcance de clientes, ahorro de tiempo y comodidad al no tener que desplazarse a la farmacia física.

### **7.	Funciones del Producto**

•	Módulo de gestión de usuario.

•	Módulo de inicio de sesión.

•	Módulo de búsqueda de producto.

•	Módulo de Carrito de compras.

•	Módulo de pago para compras en línea.

•	Generar factura electrónica de las compras que se realicen.

•	Módulo de PQR.

•	Módulo de publicidad.

### **8.	Características de Usuario**

El sistema cuenta con tres tipos de usuario 

Empleado: se encargará de la administración del sistema.

Cliente: realizara compras y consultas.

Administrador: se asegura del correcto funcionamiento y gestión de la plataforma.

### **9.	Requerimientos Funcionales**

| Codigo | Nombre |
|---|--|
| RF-001	| Registro de usuario |
| RF-002 | Inicio de sesión |
| RF-003	| Búsqueda de productos |
|RF-004	| Carrito de compras |
|RF-005	| Pago de compra en línea |
|RF-006	| Factura electrónica |
| RF-007 | PQR |
| RF-008 | Publicidad |



| Código |	Nombre |	Fecha	| Grado Necesidad |
|---|----|----|----|
| REQ001	| gestión de usuario| Sin especificar| ALTO |
|---|---|
|  Descripcion:   | El sistema debe permitir que los usuarios se registren en la plataforma proporcionando su información personal. |
| REQ001. 1-CREACION DE CUENTA: el sistema debe permitir a los visitantes registrarse como usuarios de la farmacia online. El usuario debe digitar sus datos personales como: ID, nombre, apellido, correo electrónico, contraseña, dirección y número de contacto. |
| REQ001. 2-VEREFICACION DE CORREO ELECTRONICO: después de que el usuario a registrado sus datos personales el sistema debe enviar un correo de verificación para confirmar el correo electrónico dado por el usuario. |
| REQ0001. 3-INICIO DE SESION: el sistema debe permitir a los usuarios registrados iniciar sesión en la plataforma utilizando su ID y contraseña. |
| REQ001. 4-PERFIL DE USUARIO: los usuarios deben tener acceso a un perfil de usuario para que puedan editar su información personal como dirección, número de contacto u otros datos de información.|


| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| REQ002	| Inicio de sesión. | Sin especificar| ALTO |
|---|---|
| Descripcion: | REQ002.1- INICIO DE SESION: el sistema debe permitir a los usuarios registrados iniciar sesión en la plataforma utilizando su ID y contraseña.
| REQ002.2- RETABLECIMIENTO DE CONTRASEÑA:  El sistema debe permitir al usuario el restablecimiento de su contraseña en caso de olvidarla,  mediante un link de restablecimiento enviado a su correo electrónico. |

| Código |	Nombre |	Fecha	| Grado Necesidad |
|---|----|----|----|
| REQ003	| Búsqueda de productos  | Sin especificar| ALTO |
|---|---|
| Descripcion: |  El sistema debe permitir a los usuarios la capacidad de buscar productos farmacéuticos ya sea por el nombre del producto o la categoría.
| REQ003.1-BUSQUEDA POR NOMBRE DE PRODUCTO: El usuario de poder buscar el producto que desea ingresando el nombre del producto y el sistema debe poder de volver resultados relevantes.
| REQ003.2-BUSQUEDA POR CATEGORIAS: El sistema le debe permitir al usuario poder buscar productos por categorías como: salud y medicamentos, cuidado y aseo personal, maquillaje, maternidad y bebes, ofertas. |
| REQ003.3-VISTA PEREVIA DE PRIDUCTOS: los usuarios deben poder ver la vista previa de los productos en los resultados de búsqueda junto a la información, marca y precio del producto. |
|  REQ003.4-SUGERENCIA DE BÚSQUEDA: El sistema debe mostrar sugerencias de búsqueda, cuando el usuario escribe basándose en términos relacionados y popularidad. |
| REQ003.5-HISTORIAL DE BÚSQUEDA: El usuario puede tener acceso al historial de búsqueda de los productos que anteriormente ha buscado. |
| REQ003.6-INTEGRACION DEL CARRITO DE COMPRAS: los usuarios deben poner agregar los productos directamente desde el resultado de la búsqueda al carrito de compras. |


| Código |	Nombre |	Fecha	| Grado Necesidad |
|---|----|----|----|
| REQ004	| Carrito de compras | Sin especificar| ALTO |
|---|---|
| Descripcion: | El sistema deberá de permitir al usuario la búsqueda de productos, deben poder seleccionar la cantidad de productos que desea, ver la descripción del producto, precio y disponibilidad |
| REQ004.1-AGREGAR PRODUCTOS AL CARRITO: el usuario debe poder agregar productos al carrito.El sistema deberá permitir la actualización de la cantidad de los productos. |
| REQ004.2-DISPONIBILIDAD DEL PRODUCTO: el sistema deberá verificar si el producto se encuentra disponible para la compra antes de ser agregado al carrito. Si el producto no se encuentra disponible el sistema deberá informar al usuario.  
| REQ004.3-GETION DEL CARRITO: el usuario podrá ver el contenido actual de carrito de compras.El sistema deberá mostrar la lista de los productos, la cantidad, el precio unitario más el subtotal, El usuario debe poder modificar la cantidad del producto o eliminar el producto. |
 
| Código |	Nombre |	Fecha	| Grado Necesidad |
|---|----|----|----|
| REQ005	| pago de compras en línea.  | Sin especificar| ALTO |
|---|---|
| Descripcion: | REQ005.1-PROCESIMIENTO DE SEGURO DE PAGO: el sistema debe garantizar que la información del usuario se maneje de forma segura y que se cumplan los estándares de seguridad. |
| REQ005.2- INTEGRANCION DE METODOS DE PAGO: debe permitir la integración de varios métodos de pago |
| REQ005.3-REEMBOLSO:  debe permitir que los usuarios realicen reembolsos para las compras devueltas o canceladas. |


| Código |	Nombre |	Fecha	| Grado Necesidad |
|---|----|----|----|
| REQ006	| Factura electronica | Sin especificar| ALTO |
|---|---|
| Descripcion: | REQ006.1-GENERACION AUTOMÁTICA DE FACTURA: el sistema de generar automáticamente facturas electrónicas al momento que la compra se haya realizado exitosamente |
| REQ006.2-DETALLES DE COMPRA: la factura de electrónica deber contener detalles específicos de la compra, como el nombre del producto, precio unitario, descuentos aplicados, impuestos, descripción de la compra y el total de la compra |
| REQ006.3-ENVIO AUTOMATICO DE LA FACTURA: El sistema debe enviar automáticamente la factura al correo del usuario |
| REQ006.4-HISTORIAL DE FACURACION: el sistema debe permitir que tanto el usuario como el empleado pueda acceder en cualquier momento al historial completo de las facturas generadas |

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| REQ007	| PQR | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | Brindar a los usuarios la opción de realizar consultas o solicitar asesoramiento farmacéutico en línea a través de un sistema de chat en vivo o correo electrónico.
| |REQ007.1-CONSULTA EN LÍNEA: el usuario podrá realizar consultas en línea sobre medicamentos, efectos segundarios, dosis recomendadas, productos, etc.
| |REQ007.2-ASESORAMIENTO FARMACEUTICO: el usuario recibirá asesoramiento personalizado por el farmacéutico autorizado, el asesoramiento se realizará por medio de un chat en línea o llamada telefónica.

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| REQ008 | Publicidad  | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | REQ008.1- ANUNCIOS DESTACADOS: Permitir a los proveedores o marcas asociadas a la farmacia destacar ciertos productos o promociones mediante anuncios patrocinados.
| |REQ008.2-OFERTAS Y PROMOCIONES: Mostrar anuncios y notificaciones de ofertas y promociones especiales para atraer a los clientes y aumentar las ventas.
| |REQ008.3-INTEGRACIÓN CON REDES SOCIALES: Permitir que los clientes compartan o interactúen con anuncios en las redes sociales para aumentar la viralidad y el alcance de la publicidad.


### **10.	Requerimientos No Funcionales**

| Codigo | Nombre |
|----|---|
| RFN-001 | Usabilidad del sitio web |
|RFN-002 |	Velocidad de carga de la página |
|RFN-003 | Seguridad de la información |
| RFN-004 |	Disponibilidad
| RFN-005 | Privacidad y protección de datos|
|RFN-006 | Mantenibilidad |

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RFN-001	| Usabilidad del sitio web | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga.|

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RFN-002	| Velocidad de carga de la página | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | El sitio web debe cargar de manera rápida y eficiente para los usuarios, sin tiempos de espera prolongados o errores de carga.|

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RFN-003	| Seguridad de la información | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | El sitio web debe garantizar la confidencialidad, integridad y disponibilidad de la información de los usuarios y de la propia empresa, protegiéndola de accesos no autorizados, robo o pérdida de datos.|

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RFN-004	| Disponibilidad | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | El sistema debe estar disponible para el usuario en todo momento, minimizando el tiempo de inactividad no planificado.


| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RFN-005	| Privacidad y protección de datos  | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: |  establecerse políticas claras de privacidad y protección de datos para proteger la información personal del usuario.

| Código |	Nombre |	Fecha	| Grado Necesidad
|---|----|----|----|
| RNF-006	| mantenibilidad | Sin especificar| ALTO |

| |   |
|---|---|
| Descripcion: | El sistema debe ser fácil de mantener y actualizar para agregar nuevas funcionalidades o corregir errores.






