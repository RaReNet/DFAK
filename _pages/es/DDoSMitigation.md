---
layout: page
title: "Mitigación de ataques DDoS"
author: RaReNet
language: es
summary: "Una amenaza enfrentada por muchos periodistas independientes, sitios de noticias y blogueros es tener sus voces calladas debido a que su página web está caida o modificada. En muchos casos, esto puede ser un problema cándido y frustrante, pero en casiones, puede ser debido a un ataque de "denegación de servicio" o una toma de la página web. Esta sección del Digital Fist Aid Kit (Kit de Primeros Auxilios Digitales) te mostrará algunos pasos básicos para diagnosticar probelmas potenciales."
date: 2015-08
permalink: /es/DDoSMitigation/
parent: /es/
---

# Mitigación de ataques DDoS

Una amenaza enfrentada por muchos periodistas independientes, sitios de noticias y blogueros es tener sus voces calladas debido a que su página web está caida o modificada. En muchos casos, esto puede ser un problema cándido y frustrante, pero en casiones, puede ser debido a un ataque de "denegación de servicio" o una toma de la página web. Esta sección del Digital Fist Aid Kit (Kit de Primeros Auxilios Digitales) te mostrará algunos pasos básicos para diagnosticar probelmas potenciales. Si tu sitio web está bajo un ataque de denegación de servicio, sesugieren algunas acciones inmediatas para siguientes pasos.

En general, es importante saber que pueden haber muchas razones por las cuales una página puede estar caida. Lo más común es que sea debido a errores de programación o problemas técnicos de la empresa que aloja el sitio web. A veces, otros factores como acciones legales tmbién pueden provocar que un servidor deshabilite un sitio. Encontrar el problema y las posibles soluciones puede ser complicado si no tienes experiencia en alojamiento web. Por lo tanto, siempre que sea posible el mejor primer paso es contactar a una persona de confianza que pueda ayudar con tu sitio web (tu webmaster, la persona que ayudó a configurar la página, personal interno si existe y la compañia que aloja el sitio web, o si ninguno de estos está disponible), [busca ayuda de una organización en la que confíes](SecureCommunication.md#seeking-and-providing-remote-help) )

Es una buena práctica **contactar a tu webmaster y a la empresa que aloja el sitio** ¡después de investigar lo que aparece a continuación!  El problema que enfrentas puede no estar reportado en su página de status, puede ser un problema temporal, o el proveedor puede no estar enterado todavía del problema. Una buena relación con tu proveedor de servicio llega muy lejos - se claro y educado y comparte los resultados de tu investigación usando estas preguntas para ayudarlos a rápidamente resolver el problema.

## Comienza respondiendo algunas preguntas simples:

### Información básica

- ¿Quién implementó el sitio web? ¿Está disponible para ayudar?
- ¿Quién es tu proveedor de alojamiento web? Esta es la compañía que provee el servidor en donde tu sitio web está funcionando. Si no sabes cuál proveedor es, puedes [usar una herramienta](http://www.whoishostingthis.com/) para encontrarlo.
- ¿Tienes un registro detallado de la cuenta de este proveedor de alojamiento web?
- ¿En dónde adquiriste el nombre de dominio? En algunos casos esta empresa es la misma que provee el alojamiento web, sin embargo esta puede ser otra compañía.
- ¿Tienes un registro detallado de la cuenta del proveedor de nombred de dominio? Si no, encontrarlo es el primer paso para recuperar tu sitio.
- ¿Quién mas sabe o puede tener acceso a la información de estas cuentas?

### Información de Diagnóstico

Pueden haber diferentes razones por las cuales tu sitio web está caído. Pueden ir desde la red hasta leyes, alojamiento, bloqueos, software, toma de página o problemas de rendimiento. La sección a continuación explica qué es cada una y cómo diagnosticar el problema que estás enfrentando.

- **¿Tu servidor web está funcionando pero tu página no está disponible?**
    1. Chequea [esta página](http://www.isup.me/)
        - ¿Tu página está al aire, pero no la puedes ver?
            - Este es un **problema de red**. Tu propia conexión a internet puede estar teniendo problemas o estra siendo bloqueado el acceso a tu página.
            - Esto también puede indicar que tu cuenta ha sido deshabilitada: **Are you seeing a message from your web hosting provider?**
                - Tu cuenta pudo haber sido deshabilitada por razones de pago, legales, de derechos de autor o alguna otra.
                - Esto es un **problema de políticas**. Primero, asegúrate de que tu información de facturación esté al día y que no hayan saldos pendientes en tu servicio de alojamiento y/o nombre de dominio. Si hay mensajes relacionados a problemas legales, [la referencia proporcionada](https://www.eff.org/issues/bloggers/legal/liability/IP) por la EFF -En Inglés-, aunque está basada en las leyes estadounidenses, es un buén lugar para aprender más.
        - **¿Tu página web no esta cargando en absoluto?** Tu compañia de hosting puede estar teniendo problemas, en ese caso estas en presencia de un **problema de alojamiento**.
            - ¿Puedes visitar el sitio web de la compañia de alojamiento web? Nota que esta *no* es la sección de administrador de tu propio sitio web, sino el de la compañía u organización que aloja tu página. Busca por un blog de 'status' (p.e. status.dreamhost.com): busca también en twitter.com para encontrar a otros usuarios discutiendo la posible falla del proveedor.
                - un búsqueda simple como '(nombre de la compañía) down' puede revelar si otros clientes están teniendo el mismo problema.
    2. **¿Puedes visitar otros sitios web con contenido similar al tuyo?**
        - Intenta visitar websites con contenidos similares a los tuyos o que cubran los mismos temas. También intenta acceder a tu sitio web usando [Tor](https://www.torproject.org/projects/gettor.html) (En Inglés) o [Psiphon](https://psiphon.ca/es/index.html). Si esto funciona, estás experimentando **problemas de bloqueo** - tu sitio web está disponible en otras partes del mundo, sin embargo está censurado en tu propio país.
    3. **¿Estás viendo mensajes de error?**
        - Esto puede ser un **problema de software**. Debes pensar en cualquier cambio reciente que tu o tu equipo hayan hecho en el sitio web y contactar al webmaster.
            - Una captura de pantalla, el link de la página qu está teniendo problemas con cualquier mensaje de error que veas ayudará al webmaster a entender qué pudo haber causado el problema.
            - También puedes buscar los mensajes de error en internet para ver si pueden ser arreglados con facilidad.
    4. **¿Estás viendo un sitio web diferente al tuyo? ¿Recibes alguna advertencia de tu explorador acerca de malware en tu propio sitio web?**
        - Esto puede ser debido a un **problema de modificación**. Echa un vistazo abajo para próximos pasos; necesitarás trabajar en conjunto con tu proveedor de alojamiento web y revisar la sección de Hackeo de Cuentas.
    5. **¿Tu página está cargando de forma intermitente o inusualmente lenta?**
        - Tu sitio web puede estar saturado por el número y velocidad de las solicitudes de páginas que está recibiendo - esto es un **problema de rendimiento**. Esto puede ser 'bueno' debido a que el sitio se ha vuelto más popular y simplemente necesita algunas mejoras para responder a más lectores.
            - chequea tu página de métricas para analizar los patrones de crecimiento.
            - Contacta a tu webmaster o proveedor de aloamiento por asistencia. Varias plataformas de bloging y manejadores de contenidos o CMS (Joomla, Wordpress y Drupal entre otros) tienen plugins para mejorar el cache local de las páginas web e integrar CDNs, los cuales pueden mejorar dramáticamente el rendimiento y la capacidad de adaptación. ALgunas de las soluciones a continuación también pueden ayudar con los problemas de rendimiento.

## Primeros pasos para mitifagar el problema:

### Cuando estás sufriendo un ataque de denegación de servicio

Si el diagnóstico mostrado arriba no ayuda o estás experimentando **problemas de rendimiento** severos, tu sitio web puede estar siendo víctima de un **ataque de denegación de servicio**, en donde un usuario malicioso (o usuarios), intentan ver el sitio repetidamente y rápidamente (usando herramientas automatizadas), y al hacerlo desplaza a los lectores reales. A veces es un solo 'atacante', lo cual generalmente no representa un gran problema - salvo que pagues por ancho de banda utilizado. El ataque más frecuente obervado es el ataque de denegación de servicio 'distribuido' (DDoS), en donde el atacante usa miles de equipos bajo su control para llevar a cabo el ataque contra un sitio web.

- Paso 1: Contacta a una persona de confianza que pueda ayudar con tu sitio web (tu webmaster, la persona que te ayudó a implemnetar el sitio, personal interno si existe y la compañía que aloja tu sitio web).
- Paso 2: En conjunto con la compañía en la que se adquirió el dominio (como EasyDNS, [Network Solutions](http://www.networksolutions.com/support/how-to-manage-advanced-dns-records/), [GoDaddy](http://support.godaddy.com/help/article/680/managing-dns-for-your-domain-names)) y cambia el parámetro 'Time to Live' o TTL a 1 hora. Esto puede ayudar a redirigir tu sitio web mucho más rápido una vez que está bajo atque (de forma predeterminada es 72 horas, o tres días). Esta configuración se encuentra generalmente en la sección de propiedades avanzadas del sominio, a veces como parte de SRV o Service records.
- Paso 3: Mueve tu sitio web a un servicio de mitigación de DDoS [full list](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services) (En Inglés). Para comenzar:
    - [Deflect.ca](https://deflect.ca/) (En Inglés)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/) (En Inglés)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo) (En Inglés)
- Paso 4: Tan pronto como hayas recuperado el control sobre el sitio web, revisa tus necesidades y decide entre un proveedor de alojamiento seguro o simplemente continuar el servicio de mitigación de DDoS.

### Cuando estás sufriendo de una modificación de página

- Paso 1: Verifica si se trata de una toma maliciosa del sitio web. Una práctica desafortunada pero a su vez legal consiste en comprar nombres de dominio vencidos recientemente para 'tomar' el tráfico que tenían para fines publicitarios. Es muy importante mantener al día los pagos de tus nombres de dominio.
- Paso 2: Si tu sitio ha sido modificado y/o tomado, primero recupera el control de tu cuenta de usuario del mismo y reestablece la clave, mira la sección de Hackeo de Cuentas para más información.
- Paso 3: Realiza una copia de seguridad del sitio modificado para poder usarla para investigación de la modificación.
- Paso 4: Deshabilita temporalmente tu sitio web - usa una página estática (landing page o parked page por ejemplo).
- Paso 5: Determina cómo fue atacado tu sitio. Tu proveedor de alojamiento web puede ayudar con esto. Los problemas más comunes están relacionados con partes viejas de tu sitio con código/herramientas actualmente en funcionamiento, sistemas de manejo de contenidos desactualizados y código propio con vulnerabilidades de seguridad.
- Paso 6: Reestablece tu sitio original desde una copia de seguridad. En el caso de que ni tu ni tu empresa de alojamiento web tengan copias de seguridad del sitio ¡tendrás que rehacer el sitio web desde cero! También nota que si las únicas copias de seguridad disponibles son las del proveedor de alojamiento web ¡el atacante pudo haber borrado estas copias de seguridad si tomó control de tu sitio!
- Paso 7: Mueve el sitio a un servicio de mitigación de ataques DDoS o a un servidor de alojamiento web seguro. Deflect.ca puede apoyarte protegiendo tu sitio de ataques informáticos. CloudFlare puede bloquear también algunos tipos de ataques habituales. Servidores de alojamiento web seguros como VirtualRoad/Qurium son muy buenos detectando y previniendo estos ataques.

## ¡No te detengas aquí! Siguientes pasos importantes:

**¡No esperes a ser atacado!** Todos los servicios listados anteriormente trabajaran rapidamente  para ayudarte a recuperar tu sitio durante o después de un ataque, sin embargo ¡puedes proteger tu sitio ahora, antes de que ocurra algún ataque! Esto puede reducirte costos al reducir el ancho de banda utilizado y manteniéndo el sitio activo durante un ataque. Una vez que has sido atacado, puede tomar hasta 3 dias para que el Internet te vuelva a 'encontrar' en tu nueva dirección protegida - por lo que en casi todos los casos **es mucho mejor estar preparado y comenzar ahora**.

1. **Los proveedores de alojamiento web seguro** necesitan que muevas completamente tu sitio web a sus servidores - porque estás cambiando de proveedor de alojamiento. Algunos de ellos pueden ayudarte durante este proceso. Los beneficios incluyen protección adicional para otros tipos de ataques además de la mitigación de DDoS; las desventajas pueden ser el costo (dependiendo de lo que estés pagando actualmente) y el control - tienes que poder confiar en tu proveedor, ya que este tendrá mucho control sobre tu sitio web.
    - Pros:
        - Provee un servicio que centraliza la mayoría, si no todas, las necesidades de tu sitio web
        - Provee servicios de protección contra ataques DDoS, hackeos y ataques de spam
        - Generalmente incluyen algunos servicios secundarios, consultoría e incluso defensa legal limitada en algunos casos
        - Generalmente tienen equipos grandes de soporte a disposición
    - Contras:
        - Debes alojar tu sitio web con estas empresas
        - Debes confiar en el servicio para que gestione tu sitio web y defienda tus derechos
        - Generalmente estos servicios son muy costosos (¡sin embargo no tienes que pagar por otros servicios de alojamiento / servicios DNS en absoluto!)

2. **Servicios de mitigación de ataques DDoS** funcionan permitiéndote mantener el sitio en donde sea que esté alojado, cambiando sólo la forma en la cual otros en internet lo encuentran y lo accesan - por lo general es mucho más sencillo de configurar Estos servicios tienen servidores alrededor del mundo, que esencialmente están en el medio del camino a tu sitio web y deciden absorber o rechazar el tráfico malicioso. Ellos 'reflejan' y sirven copias constantemente actualizadas de tu sitio. Estos servicios son sencillos de configurar y te dan control completo de tu sitio y configuración de alojamiento. Una particularidad con servicios en proxy es que en el caso de sitios web muy complejos se pueden experimentar problemas ocasionales con inicios de sesión de usuarios no administrativos y con código interactivo o de javascript. Por favor discute estos casos con tu webmaster y servicio de proxy para solucionar cualquier posible situación.
    - Pros:
        - Costo más bajo (generalmente con opciones gratuitas)
        - Rápido y fácil de configurar
        - No tienes que cambiar el servidor de alojamiento web
        - Puedes cambiar o cancelar el servicio en cualquier momento
    - Contras:
        - Existen menos opciones de soporte
        - Están enfocados principalmente en mitigar ataques DDoS - por lo que no necesariamente incluyen soluciones conra malware o spam.
        - El tráfico SSL (cifrado) será brevemente descifrado y vuelto a cifrar por el servidor proxy para mantener la comunicación entre el proxy y tu servidor de alojamiento.

3. Selecciona un proveedor específico - para cualquier servicio, debes sentirte cómodo con el proveedor. Esto está relacionado con la confianza, pero también con entender su modelo de negocios: ¿comprende un pago por servicio? Si hay una versión gratuita ¿Tiene menos soporte que una alternativa paga? ¿El proveedor está financiado por gobiernos? Lo mejor es cubrir tantos detalles como sean posibles para evitar sorpresas en el futuro.

### Para todos los servicios preguntate lo siguiente:

- ¿Cómo se estructura y sostiene la compañía u organización? ¿Qué tipo de rendiciones de cuengtas y reportes están obligados a hacer, si es el caso?
- Cnsidera en qué país o países tienen presencia legal y en cuáles ellos pudieran tener que responder ante solicitudes legales de las autoridades u otras medidas similares
- ¿Qué registros de actividad (logs) son creados y cuánto duran disponibles?
- ¿Hay restricciones sobre el tipo de contenido que el servicio va  alojar o pasar por proxy, en ese caso estas restricciones tendrían un impacto en tu sitio?
- ¿Hay restricciones sobre los países en donde el proveedor puede prestar servicio?
- ¿Aceptan una forma de pago que te resulte de utilidad? ¿Puedes costear el servicio?
- Comunicaciones seguras - deberías ser capaz de iniciar sesión de forma segura y comunicarte de forma privada con el proveedor del servicio.
- ¿Existe alguna opción de auntenticación en dos factores, para mejorar la seguridad del acceso administrativo? Esta y otras políticas de seguridad pueden reducir las amenazas de otros tipos de ataques contra tu sitio web.
- ¿De qué tipo de ayuda puedes tener sobre la marcha? ¿Existe un costo adicional para obtener soporte, y/o recibirás suficiente ayuda si usarás una versión gratuita?
- ¿Puedes 'probar' tu sitio web antes de moverlo a otro lugar a través de un sitio ntermedio (staging site)?

### Preguntas para servicios de alojamiento web seguros

- ¿Ofrecen soporte completo en mover el sitio web a sus servidores?
- ¿Los servicios ofrecidos son mejores a los que ya tienes, al menos para las herramientas y servicios que utilizas? Las cosas más importantes a chequear son:
    - Herramientas de Gestión como cPanel
    - Cuentas de correo electrónico (cuántas se pueden tener, cuotas, acceso mediante SMTP, IMAP)
    - Bases de datos (cuántas se pueden tener, tipos, acceso)
    - Acceso remoto mediante SFTP/SSH
    - Soporte para lenguajes de programación (PHP, Perl, Ruby, cgi-bin ...) o Sistemas de manejo de contenidos CMS (Drupal, Joomla, Wordpress…) que pueda usar tu sitio web

### Preguntas para servicios de mitigación de ataques DDoS:

- Si usas SSL (también conocido como HTTPS o tráfico web seguro), pregunta como lo gestionan el servicio de tu interés. En algunas configuraciones, puede ser más sencillo si compartes con ellos tu llave SSL privada. Si lo haces, necesitas tener un nivel muy alto de confianza en el proveedor que selecciones, ya que ellos pudieran 'hacerse pasar' por tu sitio web (de hecho, !es lo que les estarias pidiendo que hagan proporcionándote un proxy!)
- Pregunta cómo funcionarían los inicios de sesión para administradores y editores del sitio web, así como sus páginas particulares
- Habla acerca de cualquier sección interactiva de tu sitio web (usuarios que inician sesión, comentan, necesidades de administración/edición, páginas/código javascript/animaciones interactivos complejos) - cada proveedor de servicios proxy puede manejar estas secciones de formas diferentes: necesitarás probarlas tu mismo antes de cambiar definitivamente el sitio.

### Servicios de mitigación específicos
Algunos servicios están en una [lista con notas detalladas](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-service) (En Inglés). Es importante notar que esta no es una lista completa de servicios de este tipo. Sin embargo, estos servicios representan un buen punto de partida, debido a que han sido utilizados por otros miembros de las comunidades de medios independientes / Derechos Humanos / libertad de expresión. Para una cobertura inmediata, te presentamos dos opciones:

- Servicios de alojamiento web seguro:
    - [Qurium (formerly Virtual Road)](https://www.qurium.org/)
    - [The Positive Internet Company](http://www.positive-internet.com/services/vip-hosting)
    - [Greenhost](https://greenhost.net/)

- Servicios de mitigación de ataques DDoS:
    - [Deflect.ca](https://deflect.ca/)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo)

## Toma medidas de prevención adicionales contra atacantes

Incluso si nunca has sido víctima de un ataque de denegación de servicio, esta guía te ayudará a prepararte para uno, con suerte garantizando la disponibilidad del sitio en todo momento. Ve directamente a la sección [Responding to a Denial of Service Attack](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#responding-to-a-denial-of-service-attack) (En Inglés) para investigar soluciones habituales que pueden ser implementadas en el inmediato plazo, antes de ser atacado. En la sección de referencias útiles podrás encontrar guías para mantener tu sitio al aire.

- **Copias de seguridad**: Es bueno asegurase siempre de que tengas copias de seguridad disponibles (¡guardadas en un lugar diferente a donde está el sitio web!). Muchos proveedores de alojamiento web proveen esto compo parte de su servicio, sin embargo lo mejor es tener copias adicionales offline.
- **Mantente al día**: Si estás usando un Sistema de Manejo de Contenidos (CMS) como Wordpress o Drupal, chequea que el mismo está actualizado a su última versión, especialmente si han habido actualizaciones de seguridad. Si estás usando software particular, considera migra a un CMS que reciba actualizaciones frecuentes.
- **Monitoreo**: Existen algunos servicios que revisan constantemente tu sitio web y te avisan mediante un correo electrónico o mensaje de texto si no está disponible. [Este artículo](http://mashable.com/2010/04/09/free-uptime-monitoring/) (En Inglés) recopila algunos de los más populares. Toma en cuenta que el correo electrónico y/o número telefónico usado para habilitar este monitoreo estarán asociados al manejo de este sitio web.

## Investiga

Si eres víctima de un ataque de **Denegación de Servicio** o de **Modificación o Toma de Sitio**, resulta útil saber porqué fuiste atacado y porqué en este momento particular.

**Porqué fuiste atacado y porqué en este momento particular**: ¿Quién crees que puede estar interesado en hacerte un objetivo a ti o a tu organización? ¿HAs publicado algo controversial, puede el ataque estar relacionado al trabajo que haces o tu sitio web recibe mucho tráfico y tu nombre de dominio expiró? ¿Porqué ahora? Pudo un cambio reciente a tu sitio web haber provocado que tu o tu organización e volvieran un objetivo de ataques de DDoS o de Modificación/Toma? En la sección de referencias útiles. En la sección de referencias útiles hay links de guías que te pueden dar tips y trucos de cómo prevenir emergencias digitales y ser proactivo en tu seguridad digital.

## Helpful resources:

- [My Website is Down](https://github.com/OpenInternet/MyWebsiteIsDown) (En Inglés)
- [Cómo mantener su sitio activo](https://www.eff.org/es/keeping-your-site-alive)
- [Security in a Box](https://securityinabox.org/es/chapter_7_2)
- [Guía de modelos de amenazas, Vigilancia y Autodefensa](https://ssd.eff.org/risk/threats) (En Inglés)

