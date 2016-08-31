---
layout: page
title: "Construyendo Confianza"
author: RaReNet
language: es
summary: "Anteriormente, mencionamos algunas formas básicas de comenzar a establecer confianzae entre alguien que busca ayuda y aquel que pueda brindársela. Esta sección busca colocar una capa técnica de confianza por encima de lo ya comentado, así como entender las herramientas que te pueden ayudar a mantener una conversación segura sólo con la persona con la que piensas que estás conversando. Es importante notar que a pesar de que esta sección tiene un nivel técnico importante, te pedimos que hagas tu mayor esfuerzo - ¡Es mejor usar herramientas de cifrado que no usarlas!"
date: 2015-08
redirect_from: /es/EstablishingTrust/
permalink: /es/ConstruyendoConfianza/
parent: /es/
---

# Construyendo Confianza

Anteriormente, mencionamos algunas formas básicas de comenzar a establecer confianza entre alguien que busca ayuda y aquel que pueda brindársela. Esta sección busca colocar una capa técnica de confianza por encima de lo ya comentado, así como entender las herramientas que te pueden ayudar a mantener una conversación segura sólo con la persona con la que piensas que estás conversando. Es importante notar que a pesar de que esta sección tiene un nivel técnico importante, te pedimos que hagas tu mayor esfuerzo - ¡Es mejor usar herramientas de cifrado que no usarlas!

Herramientas de cifrado como OTR ("Off the Record") y PGP ("Pretty Good Privacy") poseen muchos beneficios. Los mensajes o archivos cifrados con OTR o PGP están protegidos de cualquier persona tomando o monitoreando las comunicaciones entre tu computadora y el destino final de tus mensajes. El problema sin embargo, es estar seguro de que el destino final de tus mensajes es el 'correcto'.

Para usar herramientas de cifrado como estas, debes saber la dirección exacta a la que le envías los mensajes cifrados - esta no se compone solo de un correo electrónco o un usuario de mensajería instantánea, sino que requiere información adicional - que incluye la 'llave' de cifrado que utiliza esa cuenta.  La mayor parte de este proceso es llevado a cabo por tu computadora, ¡Pero es importante que des la confirmación final! Teóricamente, si estás tratando de establecer una comunicación segura con alguien, un atacante pudiera sustituir la información de cifrado por una propia, y de esta forma poder leer todas tus comunicaciones. Para protegerte de esta práctica te damos un par de recomendaciones.

## Confianza en sitios web
Los sitios web seguros (aquellos que comienzan con HTTPS) funcionan mediante un sistema en donde los exploradores dependen en un número limitado de compañías de confianza. Esto hace la experiencia relatívamente sencilla para los usuarios, pero si alguna de estas compañías queda comprometida (¡Que ha pasado!) o están dispuestas a colaborar con algún gobierno que pueda representar una amenaza para ti, la cadena de confianza en tu totalidad se vuelve un problema (este modelo también se utiliza para un tipo específico de sistema de seguridad para correo electrónico llamado S/MIME).

## Confianza en heramientas de comunicación
Para correos electrónicos, chat y lamadas telefónicas seguras, esto es un poco más 'directo'. ¡El escenario ideal es encontrarse con alguien en persona para intercambiar informaciones de huellas electrónicas. En ee caso no hay riesgos de que alguien este 'interceptando' y cambiando la información! Obviamente esto no siempre es posible. Las distintas herramientas disponibles tienen diferentes formas de abordar este problema. [Security in a Box tiene un capítulo completo](https://securityinabox.org/es/chapter-7) dedicado a comunicaciones privadas.

### Chat: 'OTR'
En chats o mensajería instantánea, el estandar actual para establecer confianza es llamado OTR, o Off The Record (Fuera de Registro). Diferente a la funcionalidad 'off the record' en GChat (Hangouts) que simplemente no deja un registro permanente de la conversación en los servidores de Google. OTR provee las ventajas descritas anteriormente (seguridad de extremo a extremo y protección contra monitoreo), sin embargo, notablemente provee una capa adicional de seguridad - cada sesión de conversación es protegida de forma independiente. Esto significa que si alguien es capaz de guardar tus coversaciones y logra descrifrar el contenido de un chat seguirá sin poder ver el contenido de las demas conversaciones. Esto también da cierto grado de 'negabilidad' p.e. ya que tus conversaciones están protegidas y autenticadas, no hay forma de probar que alguno de esos mensajes provino de ti. OTR funciona en Adium, Jitsi y [Pidgin](https://securityinabox.org/es/pidgin_main).

Sin embargo, para beneficiarte de estas características, debes buscar una forma de 'autenticarte' con la persona con la que estas conversando. Solamente deberás hacer esto una vez por dispositivo y contacto seguro (y puedes usar aplicaciones como [KeySync](https://guardianproject.info/apps/keysync/) para facilitar el proceso). La clave para relacionar esta confianza digital con una persona que conoces es a través de un secreto conocido por ambos - puedes llamar a los otros y comparar directamente un código único de sus cuentas o usar una metodología de pregunta y respuesta cuando sabes que sólo esta persona específica conoce una respuesta particular que acordaron previamente.

Referencias:

• Authenticacion en OTR: [https://securityinabox.org/es/pidgin_securechat](https://securityinabox.org/es/pidgin_securechat)
• Detalles técnicos sobre OTR (En Inglés): [https://otr.cypherpunks.ca/](https://otr.cypherpunks.ca/)
• Email: PGP

## Confianza en el correo electrónico: PGP

PGP (o Pretty Good Privacy - Privacidad muy buena) y su equivalente de código abierto GPG te permiten cifrar correos electrónicos y archivos para ti mismo o para enviar a otros. Con complementos como [Enigmail para Thunderbird](https://securityinabox.org/es/thunderbird_main) o [GPGOL](http://www.gpg4win.org/) para Outlook, puedes usar PGP eficientemente para proteger el contenido de tus correos (aunque no el asunto, o a quién le estás escribiendo).

Para enviar un correo electrónico cifrado con PGP, no necesitas tus propias llaves PGP. Las llaves PGP vienen en pares, una pública y una privada. La llave pública es como la dirección de una casa que cualquiera puede saber pero solo alguien con la llave 'privada' puede acceder a la cuenta para recibir los mensajes enviados a esa dirección. Por la misma magia de PGP, solo la persona en esa dirección (con la llave privada) puede enviar mensajes desde esa dirección (mensajes que pueden ser verificados mediante la parte pública de la llave). Revisa las referencias listadas abajo para ver una discusión más detallada de cómo funciona PGP.

El problema con esto, por supuesto, es encontrar las llaves públicas o 'direcciones' - existen directorios digitales para llaves PGP en donde puedes buscar por direcciones de correo o nombres ([https://sks-keyservers.net/i/#extract](https://sks-keyservers.net/i/#extract) y [https://pgp.mit.edu/](https://pgp.mit.edu/) son dos muy populares) - sin embargo no existe una autoridad que garantice que esas llaves pertenecen a las personas correctas. Es completamente posible que alguien haya cargado su propia llave incluso con una dirección falsa de correo para hacerse pasar por alguien mas.

De nuevo, el truco está en verificar que la llave que estamos usando es la correcta utilizando otro método - muchas personas comparten en papel sus 'huellas' o 'fingerprints', o las publican en sus perfiles de twitter o sitios web. El problema con esto es que sólo funciona para una comunidad pequeña de amigos, no en una escala global en Internet.

Para personas que están relativamente seguras y pueden manejar publicamente su red de contactos, se pueden 'firmar' las llaves PGP de otras personas que ya has conocido y verificado. Esto ayuda con el problema de la confianza al crear una 'red de confianza' p.e. si has verificado la llave de alguien y confias en esa persona para verificar las llaves de otros, puedes confiar también en cualquier llave que ellos hayan firmado.

Generalmente esto no es un gran problema siempre que confíes razonablemente en que tienes la llave y la dirección de correo correcta de la persona con la que te quieres comunicar, así que considera cualquier cambio extraño en llaves y correos electrónicos como sospechoso.

Referencias:
• [https://pressfreedomfoundation.org/encryption-works#pgp](https://pressfreedomfoundation.org/encryption-works#pgp) (En Inglés)
• [https://www.cryptoparty.in/brief#crypto](https://www.cryptoparty.in/brief#crypto) (En Inglés)

## Confianza en voz cifrada: ZRTP

### Voz Cifrada: ZRTP

ZRTP es similar a OTR en muchos aspectos, cambia con cada conversación y protege el historial de las conversaciones. ZRTP es el estandar de cifrado integral de llamadas de voz (usado por [Jitsi](https://securityinabox.org/en/jitsi), [RedPhone](https://whispersystems.org/#privacy), o [Silent Circle](https://silentcircle.com/)). Es requerido que leas en voz alta una secuencia corta de caracteres a la persona con la que estás hablando para autenticar la llamada usando tu voz en combinación con estos caracteres únicos.

Referencias:
• [https://jitsi.org/Documentation/ZrtpFAQ#faqHow](https://jitsi.org/Documentation/ZrtpFAQ#faqHow) (En Inglés)
• [https://silentcircle.com/web/faq-zrtp/?#7](https://silentcircle.com/web/faq-zrtp/?#7) (En Inglés)
