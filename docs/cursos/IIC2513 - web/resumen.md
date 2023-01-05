# Resumen

## HTTP

_Hypertext Transfer Protocol_. Sirve para la transferencia de información. Se desentiende de la capa de transporte, confia en el TCP y deja que las redes hagan lo suyo.
Es carente de estados, o sea no hay vinculo entre solicitudes y no se acuerda de uno (stateless). Tiene un header (información solicitud) una linea en blanco (espaciador) y un Body (informacion en si)

### TCP
_Tranmission Control Protocol_. Estandar para transmitir los datos, trabaja con las direcciones IP, definiendo como se envian los paquetes de información entre los computadores.

### IP
Especifica la dirección de un computador dentro de una red.

- IPv4: Son del formato XXX.XXX.XXX.XXX, donde XXX es un int que va desde 0 a 255, permitiendo crear un total de 4,294,967,296 (o 256 4 ) direcciones diferentes. Ejemplo: 172.16.254.1
- IPv6: Se escriben en formato hexadecimal, con la gracia que permite generar muchas más direcciones que IPv4.

IANA: Es la entidad que supervisa la asignación global de direcciones IP. (Organiza y entrega rangos)

### DNS
Servidores que guardan nombres de páginas, de forma tal que cuando uno desea conectarse a una, escribe su nombre en lugar de la dirección IP.

### Request

Tiene la siguiente sintaxis:
- Métodos
	- Head: Obtener la cabecera de lo que se envia como respuesta a un GET
	- POST: Envia datos
	- GET: Obtiene datos
	- PATCH: Actualiza un dato
	- DELETE: Borra un recurso
	- PUT: Almacena datos

- URI: Especifica el recurso solicitado
    ![](https://i.imgur.com/gHNWd5Y.png)

- version http

### Response

- Codigos 1xx: Informacion recibida
- Codigos 2xx: Eecibido exitosamente
- Códigos 3xx: Redireccionamiento
- Códigos 4xx: Errores cliente
- Códigos 5xx: Errores servidor

## URL

(Uniform Resource Locator) Es una ubicación. Se usa para identificar la forma de un recurso en la web. Tiene:
- Protocolo: ftp/http
- Hostname: Nombre dado por el DNS. Ej: localhost
- Puerto: Nº con lugar fisico donde se escucha una pitición. Ej: 80=HTTP, 443=HTTPS
- Ruta: nombre del recurso solicitado. Ej: .../admin.html

## DOM

Modelo jerárquico que el navegador construye en base al HTML que está cargando. Incluye como nodo a todos los tags y la estructura según la jerarquía que les fue dado dentro de la página, donde la etiqueta madre contiene a todas las otras etiquetas.

## CSSOM

Mapa de objetos de css que organiza el arbol de propiedades

## Js

- Promesas: Encadenar las llamadas asíncronas (que caen en el event loop) y poder controlar el orden de ejecución. Tiene los estados de resolve, pending y reject
- Loop: Gestionar operaciones que sean blocking I/O

## Node.js

Es una plataforma OpenSource que permite la ejecucion de js fuera del navegador generando un runtime environment externo. Es single thread gracias a un patron de event loop. No es ni un lenguaje ni un framework ni un servidor.

### Libuv (velociraptor unicorn)

Biblioteca que maneja las colas, los sockets, el filesystem, signal handling, etc.
Otorgar un ambiente de contexto de ejecución a V8 fuera de un browser

## NPM

Hermano de node, es un gestor de paquetes.

## Middleware

Se encarga de recibir solicitudes del cliente y mandarlos al lugar adecuado del servidor.

### KOA
Framework para app web que implementa multiples middlewares especializados en labores atomicos

## Tipos de app

- SSG: (static Site Generator) más hacer que ver. En vez de generar según la demanda del usuario, genera anticipadamente las vistas. Ej: NextJS
- SSR: (Server-side Reading) Web focalizados en el contenido NO en la interacción. Es una técnica que deja el rendering del componente o página al lado del servidor liberando de esa tarea al cliente Por ejemplo para blogs
- SPA: la aplicación funciona como si fuera una sola página (single page), utiliza un sistema de routing en un único html.
- PWA: Es como una aplicación pero relacionada a una página web. Te deja el icono de aplicación, te deja descargar paginas de antemano para disponibilidad offline y creo que te da más permisos

_SPA son paginas web construidas para ser usadas en navegadores. Las PWA se construyen para ser usadas en dispositivos móviles._


## Roles
- Developers
- SEO, CM
- Oficial de ciberseguridad
- Q&A, Encargados de calidad de software
- Operaciones: Encargados de operar la plataforma, mantenerla activa,etc
- Administrador de sistemas
- Administrador de base de datos
- Jefe de proyectos/ Ing. de software: Para gestión y control de proyectos
- UX: Encargado de User Experience

## Callback
Es una funcion que es pasada como parámetro a otra función con la “esperanza” de que sea invocada en algun momento.

## JQuery
Biblioteca multiplataforma de js que simplifica la sintaxis para acceder a componentes y eventos del DOM

## APIs
Aísla implementación de la invocación. Es una interfaz que permite la interacción entre multiples actores de sofware

## JWT
Sirve para codificar y firmar, no encriptar. Vela por la integridad y autenticidad de la inf.
- Header: Contiene info acerca del algoritmo de encriptación
- Payload: Inf. A transferir en notacion json
- Signature:  Se forma con el encoded header, el encoded payload, un secreto y el algoritmo usado para hacer el encoding.

## CDN
Red de servidores distribuidos que se articulan para entregar contenido y transferirlo utilizando internet. Si un sitio ya descargo contenido una vez, no se vuelve a descargar

## Firewall
Monton de reglas de trafico de informacion

## DNS
Un sistema de nomenclatura jerárquica descentralizado para dispositivos
Permite identificar (descifrar) la IP que corresponde a un nombre de dominio.

## JOSE
Framework cuyo propósito es entregar un metodo que permita el intercambio seguro en transferencia de dos sistemas

## Proxy Inverso:
Enruta una dirección proveniente de una solicitud un cliente, identifica el servicio (domain más puerto) que puede atender la consulta del recurso y luego se encarga de enrutar la respuesta.

## ORM
Object-Relational-Mapping. Separa el lenguaje de programacion del concepto de trabajo con base de datos, encapsulando el codigo para trabajar con los datos y mapeando un registro o estructura de datos con objetos o clases.

## AJAX
_Asynchronous JavaScript and XML_. Es un conjunto de técnicas de desarrollo web que permiten que las aplicaciones web funcionen de forma asíncrona

## TLS

Protocolo de seguridad de internet.

## Diseño y QA

- Análisis estático de código: Se analiza el código escrito, sin ejecutarlo
- Análisis Dinámico: Ejecución y búsqueda de mal comportamiento, desempeño o seguridad.
- Code Review: Distintos pares revisan el código
- Testing: Diseño de pruebas automatizadas para someter a un software bajo diferentes casos de prueba
    - Testing unitario: Testear un componente de forma individual
    - Testing de integración: Testear varios componentes trabajando en conjunto

## Seguridad

- **Injection**: Envío de datos no fiables a un interprete como parte de un comando o consulta. Puede permitir al atacante acceder a datos sin la autorización apropiada.
- **Quiebre de autenticación**: Incorrecta implementación de gestión de sesiones y autenticación, que permite al atacante comprometer contraseñas, claves, tokens de inicio de sesión, etc.
- **Exposición de datos sensibles**: Protección inadecuada de datos sensibles.
- **Broken acces control**: Restricciones sobre que pueden hacer los usuarios autentificados.
- **Security missconfiguration**: Resultado de configuraciones por defecto, incompletas, abiertas, cabeceras de http con informacion sensible
- **Cross site scripting (XSS)**
Cuando la aplicación incluye datos no fiables en una nueva pagina web sin validación. Permite ejecutar scripts en el navegador de la víctima.
    - XSS Persistente: El ataque es almacenado en el servidor de destino
    - XSS reflective: Cuando la app recibe datos desde un request que incluye datos de una inyeccion no segura. EJ: https://OWO.com/status?msg=hora+mundo
    - XSS DOM: Orientado en el lado del cliente, para alterar el contenido visible.

    **Proteccion contra XSS**
    - Escaping: Asegurar que son seguros antes de renderizarlo
    - Validacion de entrada: Todo dato no fiable sera malicioso. Proceso de asegurar que esta presentando los datos correctos
    - Sanitización: Limpiar fragmentos HTML y documentos

- **Deserialización insegura**: Convierte estructuras complejas en un formato plano de bytes. Al deserializar, se produce una ejecución remota de código.
- **Componentes con vulnerabilidades conocidas**
- **Insuficiente monitoreo y/o logging**: Permite que los atacantes sigan atacando un sistema

### Cookies
- Man in the middle: Hay que usar la directiva Secure para setear una cookie
- Ataque CSRF: Se evita con cabecera en los request

## ""Mono canonico""

<figure markdown>
   ![img](https://i.imgur.com/aHqM9i5.jpg){ width="300" }
</figure>