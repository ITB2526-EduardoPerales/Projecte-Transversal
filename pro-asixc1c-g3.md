# **Projecte Transversal**

* **Nombre del proyecto: pro-asixc1c-g3**  
* **Miembros del grupo: Lucia Isabel Bartolomé, Eduardo Perales, Pol Guerrero, Aleshka Cisneros.**  
* **Centro: Institut Tecnològic de Barcelona (ITB)**  
* **Curso: 2025/2026**

## 

## 

## 

## 

**[1.Infraestructura del Centro de Procesamiento de Datos (CPD)	4](#1.infraestructura-del-centro-de-procesamiento-de-datos-\(cpd\))**

[**1.1 Diseño Arquitectónico y Ubicación Física	4**](#1.1-diseño-arquitectónico-y-ubicación-física)

[1.1.1. Ubicación de la Sala y Justificación	4](#1.1.1.-ubicación-de-la-sala-y-justificación)

[1.1.2. Medidas de Ocultación de la Infraestructura	4](#1.1.2.-medidas-de-ocultación-de-la-infraestructura)

[1.1.3. Sistema de Climatización, Rangos Ambientales y Calidad del Aire	4](#1.1.3.-sistema-de-climatización,-rangos-ambientales-y-calidad-del-aire)

[1.1.4. Especificaciones del Suelo y Techo Técnico	4](#1.1.4.-especificaciones-del-suelo-y-techo-técnico)

[1.1.5. Planos de Planta y Distribución de la Sala	4](#1.1.5.-planos-de-planta-y-distribución-de-la-sala)

[**1.2 Infraestructura IT y Distribución de Racks	5**](#1.2-infraestructura-it-y-distribución-de-racks)

[1.2.1. Inventario de Hardware Físico (Servidores, Switches y Patch Panels)	5](#1.2.1.-inventario-de-hardware-físico-\(servidores,-switches-y-patch-panels\))

[1.2.2. Distribución Espacial de los Racks (Estructuración)	6](#1.2.2.-distribución-espacial-de-los-racks-\(estructuración\))

[1.2.3. Gestión del Cableado Estructurado	7](#1.2.3.-gestión-del-cableado-estructurado)

[1.2.4. Diagramas de Alzado de los Racks	7](#1.2.4.-diagramas-de-alzado-de-los-racks)

[**1.3 Infraestructura Eléctrica y Continuidad de Negocio	10**](#1.3-infraestructura-eléctrica-y-continuidad-de-negocio)

[1.3.1. Diseño de la Alimentación Redundante	10](#1.3.1.-diseño-de-la-alimentación-redundante)

[1.3.2. Memoria de Cálculo de la Carga en Vatios (W) y Voltiamperios (VA)	10](#1.3.2.-memoria-de-cálculo-de-la-carga-en-vatios-\(w\)-y-voltiamperios-\(va\))

[1.3.3. Dimensionamiento del Sistema de Alimentación Ininterrumpida (SAI)	11](#1.3.3.-dimensionamiento-del-sistema-de-alimentación-ininterrumpida-\(sai\))

[1.3.4. Justificación del Tiempo de Autonomía de las Baterías	11](#1.3.4.-justificación-del-tiempo-de-autonomía-de-las-baterías)

[**1.4 Seguridad y Prevención de Riesgos Laborales	12**](#1.4-seguridad-y-prevención-de-riesgos-laborales)

[1\. Seguridad Física	12](#1.-seguridad-física)

[Sistema de control de acceso	12](#sistema-de-control-de-acceso)

[Videovigilancia	12](#videovigilancia)

[Sistemas de prevención, detección y extinción de incendios.	13](#sistemas-de-prevención,-detección-y-extinción-de-incendios.)

[Vías de evacuación	15](#vías-de-evacuación)

[2\. Seguridad Lógica	16](#2.-seguridad-lógica)

[Restricción de acceso por autorización	16](#restricción-de-acceso-por-autorización)

[Firewall	16](#firewall)

[Monitorización	17](#monitorización)

[Copias de seguridad (Backups)	17](#copias-de-seguridad-\(backups\))

[RAID	17](#raid)

[3\. Medidas de prevención de riesgos laborales	18](#3.-medidas-de-prevención-de-riesgos-laborales)

[Seguridad elèctrica	18](#seguridad-elèctrica)

[Control ambiental y condiciones de trabajo	18](#control-ambiental-y-condiciones-de-trabajo)

[Sonido y protección auditiva	18](#sonido-y-protección-auditiva)

[Ergonomía	19](#ergonomía)

[**Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS)	20**](#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-\(aws\))

[**2.1 Arquitectura de Red Virtual (VPC) y Seguridad Lógica	20**](#2.1-arquitectura-de-red-virtual-\(vpc\)-y-seguridad-lógica)

[2.1.1. Diseño de Subredes, Tablas de Enrutamiento e Internet Gateway	20](#2.1.1.-diseño-de-subredes,-tablas-de-enrutamiento-e-internet-gateway)

[2.1.2. Configuración de Firewalls Lógicos (Security Groups)	20](#2.1.2.-configuración-de-firewalls-lógicos-\(security-groups\))

[**2.2 Implementación de Servicios en Instancias EC2	20**](#2.2-implementación-de-servicios-en-instancias-ec2)

[2.2.1. Servidor Web y Servicio SFTP Seguro (Autenticación AD)	20](#2.2.1.-servidor-web-y-servicio-sftp-seguro-\(autenticación-ad\))

[2.2.2. Servidor de Directorio Activo (LDAP/AD)	20](#2.2.2.-servidor-de-directorio-activo-\(ldap/ad\))

[2.2.3. Servidor de Centralización de Logs del Sistema	26](#2.2.3.-servidor-de-centralización-de-logs-del-sistema)

[**2.3 Automatización, Accesos y Gestión de Configuración	27**](#2.3-automatización,-accesos-y-gestión-de-configuración)

[2.3.1. Configuración de la Gestión Mediante Ansible (Playbooks)	27](#2.3.1.-configuración-de-la-gestión-mediante-ansible-\(playbooks\))

[2.3.2. Gestión de Usuarios de Administración y Políticas de Llave Pública/Privada	27](#2.3.2.-gestión-de-usuarios-de-administración-y-políticas-de-llave-pública/privada)

[**📻 3\. Implantación de Servicios Multimedia y Redes	28**](#📻-3.-implantación-de-servicios-multimedia-y-redes)

[3.1. Servicio de Distribución de Audio Streaming	28](#3.1.-servicio-de-distribución-de-audio-streaming)

[3.2. Servicio de Vídeo Streaming y Videoconferencia	28](#3.2.-servicio-de-vídeo-streaming-y-videoconferencia)

[3.3. Pruebas Transversales de Rendimiento y Ancho de Banda	28](#3.3.-pruebas-transversales-de-rendimiento-y-ancho-de-banda)

[**🗄️ 4\. Diseño y Administración de la Base de Datos	28**](#4.-diseño-y-administración-de-la-base-de-datos)

[4.1. Diseño Conceptual, Lógico y Físico de la Base de Datos	28](#4.1.-diseño-conceptual,-lógico-y-físico-de-la-base-de-datos)

[4.2. Seguridad, Roles y Scripting de Automatización	28](#4.2.-seguridad,-roles-y-scripting-de-automatización)

[4.3. Programación del Motor: Triggers de Control y Auditoría	29](#4.3.-programación-del-motor:-triggers-de-control-y-auditoría)

[4.4. Automatización de Copias de Seguridad (Eventos)	29](#4.4.-automatización-de-copias-de-seguridad)

[**📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital	29**](#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital)

[5.1. Evaluación del Impacto de Seguridad e Importancia de las Datos	29](#5.1.-evaluación-del-impacto-de-seguridad-e-importancia-de-las-datos)

[5.2. Optimización Tecnológica y Transformación Digital	29](#5.2.-optimización-tecnológica-y-transformación-digital)

[**📹 6\. Entregables Multimedia e Incidencias	29**](#📹-6.-entregables-multimedia-e-incidencias)

## 

# 1.Infraestructura del Centro de Procesamiento de Datos (CPD) {#1.infraestructura-del-centro-de-procesamiento-de-datos-(cpd)}

## 1.1 Diseño Arquitectónico y Ubicación Física {#1.1-diseño-arquitectónico-y-ubicación-física}

### **1.1.1.	Ubicación de la Sala y Justificación** {#1.1.1.-ubicación-de-la-sala-y-justificación}

El CPD para Innovate Tech se encontraría en una planta intermedia del edificio. Las plantas bajas son más susceptibles a inundaciones o acceso fácil de parte de terceros, y las plantas más altas tienen más riesgo de calor elevado y goteras.   
En vista de un edificio de ejemplo, la planta  ideal sería la que se encuentre a la mitad.

### 

### 

### 

### 

### 

### 

### 

### 

### 

### 

### **1.1.2.	Medidas de Ocultación de la Infraestructura** {#1.1.2.-medidas-de-ocultación-de-la-infraestructura}

### **1.1.3.	Sistema de Climatización, Rangos Ambientales y Calidad del Aire** {#1.1.3.-sistema-de-climatización,-rangos-ambientales-y-calidad-del-aire}

### **1.1.4.	Especificaciones del Suelo y Techo Técnico** {#1.1.4.-especificaciones-del-suelo-y-techo-técnico}

### **1.1.5.	Planos de Planta y Distribución de la Sala** {#1.1.5.-planos-de-planta-y-distribución-de-la-sala}

## 1.2 Infraestructura IT y Distribución de Racks {#1.2-infraestructura-it-y-distribución-de-racks}

### **1.2.1. Inventario de Hardware Físico (Servidores, Switches y Patch Panels)** {#1.2.1.-inventario-de-hardware-físico-(servidores,-switches-y-patch-panels)}

Para montar la infraestructura de Innovate Tech, la idea clave es no cometer el error típico de comprar un servidor físico para cada servicio. Eso sería carísimo, poco eficiente y tiraría por tierra la sostenibilidad del proyecto. En su lugar, vamos a usar virtualización, consolidamos todo en solo dos servidores físicos potentes y un almacenamiento centralizado para ahorrar energía y optimizar recursos.  
Este es el hardware real que vamos a meter en el CPD:

* 2x Servidores Host (Dell PowerEdge R760 \- 2U cada uno):   
  Son las dos máquinas principales donde irá el hipervisor para crear las máquinas virtuales. Llevan fuentes redundantes con certificación Titanium para no gastar luz de más (sostenibilidad) y tarjetas de red dobles a 10 Gbps para que no haya cuellos de botella.  
* 1x Cabina de Almacenamiento Centralizado (QNAP Enterprise ZFS NAS ES1642dc \- 3U):   
  Aquí es donde guardaremos todos los datos de la empresa de forma centralizada. Elegimos este modelo porque tiene doble controladora activa (si una placa madre se quema, la otra sigue funcionando sin cortes). Además, usa el sistema de archivos ZFS y un entorno RAID 6, lo que significa que aunque se rompan dos discos a la vez, no perdemos ni un solo vídeo, audio o dato de la base de datos.  
* 2x Switches de Red (Cisco Catalyst 9300 \- 1U cada uno):   
  Se encargan de conectar todo. Los configuramos en modo *Stack* (apilados físicamente). Así, la red los ve como un único switch gigante; si uno se apaga o falla, el otro absorbe todo el tráfico al instante para que la empresa no se quede colgada.  
* 2x Patch Panels Cat6A (24 puertos \- 1U cada uno):   
  Sirven para organizar el cableado que viene de fuera del rack antes de conectarlo a los switches Cisco, protegiendo los puertos de estos últimos contra el desgaste de conectar y desconectar. Soporta velocidades de hasta 10 Gbps, algo fundamental para que las pruebas de ancho de banda salgan perfectas.

### **1.2.2. Distribución Espacial de los Racks (Estructuración)** {#1.2.2.-distribución-espacial-de-los-racks-(estructuración)}

El CPD va a tener 2 armarios Rack de 42U de altura. Los separamos de esta forma para organizar bien los flujos de aire (pasillo frío/caliente) y evitar que si falla algo, caiga toda la infraestructura a la vez:  
Rack 1: Servicios de Producción e Infraestructura Base  
Este armario se enfoca en las herramientas de gestión interna de la empresa.

* Hardware: Aquí dentro va el Host 1 (Dell R760), un patch panel y el primer switch Cisco.  
* Parte Virtual: Dentro del Host 1 creamos tres Máquinas Virtuales (VMs) independientes:  
  * `VM-01 (Servidor Web + SFTP Seguro):` La web y la subida de archivos segura, que además se comunica con el directorio activo para los usuarios.  
  * `VM-02 (Directorio Activo / LDAP):` Donde guardamos las cuentas y permisos de todos los empleados.  
  * `VM-03 (Servidor de Logs Centralizado):` La máquina encargada de recoger los eventos y logs de seguridad de todo el CPD para tenerlo todo auditado.

Rack 2: Servicios Multimedia, Almacenamiento y Alta Disponibilidad  
Este armario se encarga de la parte pesada: streaming, videollamadas y la persistencia de datos.

* Hardware: Contiene el Host 2 (Dell R760), la cabina de almacenamiento QNAP NAS y el segundo switch Cisco.   
* Parte Virtual: El Host 2 moverá estas cuatro VMs dedicadas al entorno multimedia:  
  * VM-04 (Base de Datos Relacional): El motor de la base de datos con toda la información de empleados, llamadas y medidas de red.  
  * VM-05 (Streaming de Audio): El servidor para la distribución de los canales de audio (MP3/AAC/OGG).  
  * VM-06 (Streaming de Vídeo): El servidor (Nginx/Jellyfin) para transmitir los vídeos en formato MP4/H.264.  
  * VM-07 (Videoconferencia Jitsi Meet): La plataforma para las videollamadas internas en tiempo real con WebRTC.

Cómo funciona la Alta Disponibilidad (HA): Al tener el almacenamiento en la cabina QNAP compartida entre los dos servidores, si el Host 1 se rompe o se apaga por mantenimiento, el Host 2 se da cuenta al instante y arranca las VMs del compañero de forma automática. Así, Innovate Tech nunca se queda sin servicio.

### **1.2.3. Gestión del Cableado Estructurado** {#1.2.3.-gestión-del-cableado-estructurado}

Para que la red vaya bien y las pruebas de velocidad (download, upload y latencia) den el máximo rendimiento, los cables se organizan con una separación física total: 

1. Cables de Datos (Por el Techo): Todo el cableado estructurado Cat6A y la fibra óptica van por bandejas metálicas suspendidas en el falso techo (techo técnico). De ahí bajan por detrás de los racks directos a los Patch Panels.  
2. Cables de Corriente (Por el Suelo): Los cables de electricidad que alimentan las fuentes redundantes van por debajo de las baldosas, por el suelo técnico, directos a las regletas (PDUs).

¿Por qué hacemos esto? (Evitar la EMI)  
Los cables eléctricos normales generan campos magnéticos a su alrededor. Si juntas un cable de datos con uno de luz, esa electricidad mete "ruido" e interferencias electromagnéticas (EMI) en la red. Esto provoca que se pierdan paquetes, que internet vaya lento y que el streaming o las llamadas de Jitsi sufran cortes.    
Al tirar los datos por el techo y la luz por el suelo, eliminamos las interferencias al 100%, asegurando que la red sea ultra estable.

### **1.2.4. Diagramas de Alzado de los Racks** {#1.2.4.-diagramas-de-alzado-de-los-racks}

Este esquema muestra cómo colocamos físicamente los equipos de arriba a abajo dentro de las 42U del armario:

* Lo pesado va abajo (Seguridad y PRL): El NAS QNAP y los servidores Dell son los equipos que más pesan. Al ponerlos abajo del todo (U1 a U5), el centro de gravedad del armario se mantiene bajo. Así evitamos que el rack pueda volcarse si hay un golpe, cumpliendo las normas de Prevención de Riesgos Laborales. Además, reciben primero el aire frío que entra por el suelo técnico.  
* Las comunicaciones en medio: Los switches y patch panels van en las posiciones U20 y U21. Se colocan ahí por comodidad: quedan a la altura de los ojos, lo que facilita a los técnicos conectar y etiquetar cables sin tener que tirarse al suelo.   
* Esquema del Alzado de los Racks:  
<img width="465" height="671" alt="ifr drawio" src="https://github.com/user-attachments/assets/7455635c-a47e-4da1-93bb-037dd169c689" />

<img width="574" height="672" alt="Captura de pantalla de 2026-05-19 08-40-37" src="https://github.com/user-attachments/assets/0d3c19c0-733a-4e43-994a-e55c1b492ca5" />

## 1.3 Infraestructura Eléctrica y Continuidad de Negocio {#1.3-infraestructura-eléctrica-y-continuidad-de-negocio}

### **1.3.1. Diseño de la Alimentación Redundante** {#1.3.1.-diseño-de-la-alimentación-redundante}

<img width="655" height="625" alt="Captura de pantalla de 2026-05-19 08-16-44" src="https://github.com/user-attachments/assets/cea95d07-61f7-423b-96b7-9c3ee7e7fd8a"/>

Aqui se puede ver el esquema de la alimentacion de los racks

### **1.3.2. Memoria de Cálculo de la Carga en Vatios (W) y Voltiamperios (VA)** {#1.3.2.-memoria-de-cálculo-de-la-carga-en-vatios-(w)-y-voltiamperios-(va)}

| Dispositivo | Cantidad | Consumo unitario | Subtotal |
| ----- | ----- | ----- | ----- |
| Dell PowerEdge R760 (Rack 1\) | 1 | 750 W | 750 W |
| Dell PowerEdge R760 (Rack 2\) | 1 | 750 W | 750 W |
| Cisco Catalyst 9300(×2 racks) | 2 | 250 W | 500 W |
| TOTAL | xxxxxxxxx | xxxxxxxxxx | 2000 W |

### **1.3.3. Dimensionamiento del Sistema de Alimentación Ininterrumpida (SAI)** {#1.3.3.-dimensionamiento-del-sistema-de-alimentación-ininterrumpida-(sai)}

VA \= W / FP \= 2.000 W / 0,9 \= 2.222 VA  
Se seleccionan dos SAIs de 2.200 VA / 1.980 W en doble conversión online, uno por línea. Cada SAI puede sostener solo la carga completa, por lo que si uno falla, el otro absorbe todo sin problema.  
Modelo recomendado: APC Smart-UPS Online SRT 2200VA RM (SRT2200RMXLI) doble conversión, baterías hot-swap, gestión SNMP, banco de baterías 48 V DC.

### **1.3.4. Justificación del Tiempo de Autonomía de las Baterías** {#1.3.4.-justificación-del-tiempo-de-autonomía-de-las-baterías}

Tiempo objetivo: 30 minutos — suficiente para arranque del grupo electrógeno y graceful shutdown ordenado de bases de datos y servicios.  
Ah \= (W × t) / (V\_bat × η)  
   \= (2.000 × 0,5) / (48 × 0,95)  
   \= 1.000 / 45,6  
   ≈ 22 Ah por SAI  
El APC SRT2200RMXLI incluye de serie \~17 Ah a 48 V. Con el módulo externo APC SRT48RMBP se alcanzan 35 Ah, lo que cubre los 30 minutos con margen.

## 1.4 Seguridad y Prevención de Riesgos Laborales {#1.4-seguridad-y-prevención-de-riesgos-laborales}

### **1\. Seguridad Física** {#1.-seguridad-física}

La seguridad física del centro de datos tiene por objeto proteger los equipos, los datos y al personal frente al acceso no autorizado, los incidentes ambientales y las situaciones de emergencia. A continuación se detalla el diseño propuesto para cada sección.

#### ***Sistema de control de acceso*** 

Con el fin de restringir el acceso al centro de datos únicamente al personal autorizado y de mantener un registro trazable de todas las operaciones de acceso, se implantará un sistema de control de acceso MFA basado en la autenticación por capas.

1. **Contraseña** {#Contraseña}
   La primera capa de seguridad consistirá en una contraseña personal asociada a cada usuario. Esto permite iniciar el proceso de autenticación y desbloquea el acceso al sistema de validación física.  
   Las contraseñas deben cumplir con las políticas de seguridad:  
* Longitud mínima  
* Combinación de carácteres  
* No incluir información personal  
* Caducidad periódica

2. **Tarjeta RFID**  
   Tras validar la contraseña, el usuario debe utilizar una tarjeta RFID personal e intransferible. Esta tarjeta identifica al empleado en el sistema y registra automáticamente el acceso. 

3. **Lector biométrico de huella dactilar**  
   Por último, será necesaria la validación biométrica mediante huella dactilar. Este sistema confirma físicamente la identidad de la persona y evita el acceso fraudulento con tarjetas robadas o compartidas. 

#### ***Videovigilancia*** {#Videovigilancia}

Para complementar el control de acceso y proporcionar pruebas visuales en caso de incidentes, se propone la instalación de un sistema de videovigilancia con cámaras IP de alta definición, diseñado para garantizar una cobertura total de todas las zonas críticas, especialmente los pasillos de aire y las zonas de manipulación de racks. Se instalarán un mínimo de cuatro cámaras IP, conectadas a la red interna y a un grabador de vídeo en red (NVR).

<img width="398" height="665" alt="Plano de camaras" src="https://github.com/user-attachments/assets/ac7a6d62-20bd-45d6-9aef-b9322771faa8" />

**Cámara 1 \- Puerta:**   
Supervisa las entradas y salidas.  
Permite verificar visualmente quién accede a la zona.

**Cámaras 2 y 4 \- Pasillos calientes:**   
Supervisa el cableado, la PDU y la zona de conexiones.

**Cámara 3 \- Pasillo frío:**   
Supervisa todas las operaciones de mantenimiento, la manipulación de servidores y las intervenciones técnicas.

**Especificaciones técnicas recomendadas:** 

* Resolución mínima de 1080p  
* Visión nocturna por infrarrojos (IR)  
* Grabación continua 24/7 durante 30 días  
* Acceso remoto cifrado

#### ***Sistemas de prevención, detección y extinción de incendios.*** {#sistemas-de-prevención,-detección-y-extinción-de-incendios.}

Los centros de datos son espacios con una alta concentración de equipos electrónicos y un elevado consumo energético, lo que aumenta el riesgo de incendio. Por este motivo, la protección contra incendios debe diseñarse de tal forma que se minimice tanto el riesgo de que se produzca un incendio como los daños causados por su extinción.

**Prevención**   
**Revisión de las instalaciones y los equipos eléctricos**

* Inspección periódica de los cuadros eléctricos, los SAI (sistemas de alimentación ininterrumpida), las PDU y el cableado.  
* Comprobación de posibles sobrecargas, conexiones defectuosas o calentamiento anormal.

**Control de temperatura y humedad**  
Se mantendrán unas condiciones ambientales adecuadas para evitar la condensación, la generación de electricidad estática y el sobrecalentamiento de los equipos.

* Temperatura ideal: entre 18 y 27 °C  
* Humedad relativa: entre el 40 y el 60 %

**Limpieza y control del polvo**

* Limpieza periódica de suelos y superficies para reducir la acumulación de polvo.  
* Uso de alfombrillas y suelos antiestáticos para minimizar las descargas que podrían dañar los equipos.

**Formación del personal**

* Formación sobre la manipulación segura de equipos eléctricos.  
* Formación sobre protocolos de evacuación.  
* Instrucciones básicas sobre cómo actuar en caso de incendio.  
* Concienciación sobre la importancia de no bloquear las salidas ni las vías de evacuación.

**Detección**  
Para detectar incendios en fase inicial, se instala un sistema de sensores conectados a una central de alarma, que envía alertas al personal.

* Detectores ópticos de humo en el techo: detectan las partículas de humo en el aire generadas por una combustión lenta.  
* Sensores de temperatura: pueden detectar aumentos anormales de la temperatura en la estancia y activar alertas antes de que se produzca un incendio. 

**Extinción**  
Dado que se trata de una sala con una alta concentración de equipos electrónicos, no es adecuado utilizar agua ni polvo químico, ya que podrían causar daños irreversibles en los servidores y la infraestructura. Por lo tanto, se propone un sistema de extinción de incendios con el gas limpio Novec 1230\.

**Características:**

* Extingue el fuego por sofocación y absorción de calor.  
* No deja residuos y no daña los circuitos electrónicos.  
* Es seguro para las personas durante un periodo limitado de exposición.

El sistema se activa automáticamente cuando los sensores detectan condiciones de incendio, tras un breve periodo de tiempo para permitir la evacuación de la sala.   
El panel del sistema de alarma contra incendios se ubicará en la pared justo al lado de la puerta, desde donde se podrá comprobar el estado de los detectores, verificar las alertas y activar o silenciar las alarmas manualmente. 

**Plano de los sensores**  
<img width="898" height="562" alt="Plano de sensores" src="https://github.com/user-attachments/assets/33d438bd-2d1b-457c-9c94-efc0950c9b56" />

En el plano, el cuadrado naranja situado en el techo representa la salida de descarga del sistema de extinción de incendios por gas, que se instalaría fuera de la sala de servidores y se conectaría al sistema.   
Por otro lado,los símbolos rojos del techo corresponden a detectores ópticos de humo, y los elementos de las paredes identifican los sensores de temperatura encargados de detectar aumentos anormales de calor. 

#### ***Vías de evacuación*** {#vías-de-evacuación}

Aunque la sala del CPD es pequeña, es fundamental garantizar una evacuación rápida y segura en caso de emergencia. La evacuación es directa e inmediata hacia el exterior, y no se requieren vías alternativas ni puertas secundarias. 

La sala de servidores tiene una única puerta de salida, la cual está equipada con una barra antipánico, lo que permite abrirla inmediatamente desde el interior.

<img width="400" height="639" alt="Plano de evacuación" src="https://github.com/user-attachments/assets/3a9ca6f1-e06c-43af-bd62-c34f392cea5b" />


**Señalización fotoluminiscente**  
En el suelo hay flechas fotoluminiscentes que indican la dirección hacia la puerta.

**Iluminación de emergencia**  
En el pasillo hay instaladas dos luces de emergencia autónomas que se activan automáticamente en caso de corte de suministro eléctrico.

### **2\. Seguridad Lógica** {#2.-seguridad-lógica}

#### ***Restricción de acceso por autorización*** {#restricción-de-acceso-por-autorización}

Para garantizar la seguridad de los sistemas y de la información del CPD, se implantará un sistema de control de acceso de autenticación multifactorial (MFA), que consiste en verificar la identidad del usuario mediante múltiples factores de seguridad, los cuales se especifican en el apartado de seguridad física.

**Registro y monitorización de los accesos**  
Todos los accesos se registrarán automáticamente en una base de datos centralizada con la siguiente información:

| ID del empleado | Fecha y hora de entrada | Tiempo dentro del CPD |
| :---- | :---- | :---- |
| Nombre y apellido | Fecha y hora de salida | Intento de acceso denegado |

Esta información puede utilizarse para realizar auditorías de seguridad, ya que facilita comprobar si los accesos corresponden con las tareas programadas y garantiza el cumplimiento de las políticas internas. También resulta útil en la investigación de incidentes, ya que permite identificar quién se encontraba en la sala de servidores en un momento determinado o si se han producido intentos de acceso no autorizados.

**Política de acceso**

* **Personal autorizado:** únicamente técnicos de sistemas, responsables de TI y personal de mantenimiento debidamente acreditados.  
* **Acceso restringido las 24 horas del día, los 7 días de la semana:** se puede acceder a la sala de servidores en cualquier momento, pero el acceso debe registrarse siempre en el sistema de control de accesos.  
* **Personal externo:** cualquier proveedor externo o visitante debe ir siempre acompañado de personal interno autorizado, y su acceso también debe registrarse.

#### ***Firewall*** {#firewall}

Los firewall son elementos fundamentales para proteger la infraestructura de red del centro de datos frente al malware o los intentos de intrusión. Por este motivo, se implementarán los siguientes niveles:

* **Firewall perimetral:** controla todas las conexiones entrantes y salientes de la red, bloqueando los intentos de acceso externo no autorizados y aplicando políticas de seguridad predefinidas.  
* **Firewall interno por segmentación:** permite separar los servicios y evita que un incidente de seguridad en un sistema se propague fácilmente al resto de la infraestructura.  
* **Listas de control de acceso (ACL):** permiten controlar qué tráfico se permite dentro de la red. 

#### ***Monitorización*** {#monitorización}

La supervisión del centro de datos permite un control constante de los servidores, la red y los sistemas de seguridad para detectar cualquier incidente de forma inmediata, antes de que afecte al funcionamiento de la infraestructura. 

* **Sistema SIEM y registros centralizados:** el CPD contará con un sistema SIEM (Security Information and Event Management) encargado de recopilar y analizar los registros generados, que se enviarán a un servidor de registros centralizado, lo que permitirá conservar un historial completo de las acciones y los eventos que se producen dentro de la infraestructura.   
* **Alertas en tiempo real:** cuando se detecte un incidente o una actividad sospechosa, se generarán alertas automáticas en tiempo real que se enviarán a los administradores del centro de datos. 

#### ***Copias de seguridad (Backups)*** {#copias-de-seguridad-(backups)}

**Estrategia 3-2-1**  
La infraestructura seguirá la estrategia 3-2-1 para reducir el riesgo de pérdida de datos. Esta política consiste en mantener tres copias de la información, utilizando dos soportes de almacenamiento diferentes y conservando una copia fuera de las instalaciones. 

**Copias de seguridad**  
Para garantizar la recuperación de la información en caso de cualquier incidente, el centro de datos realizará copias de seguridad periódicamente:

* **Diarias (incrementales):** solo se guardan los archivos modificados desde la última copia de seguridad, lo que reduce el espacio necesario y el tiempo requerido para completar el proceso.   
* **Semanal (completa):** se generará una copia completa de todos los servidores y servicios principales para proporcionar un punto de restauración completo en caso de que sea necesario recuperar el sistema entero.   
* **Mensual (fuera de las instalaciones):** se guardará una copia fuera del centro de datos, ya sea en otro CPD o en la nube. 

#### ***RAID*** {#raid}

Se utilizarán sistemas RAID en los servidores del centro de datos para aumentar la disponibilidad de los datos y reducir el riesgo de interrupción del servicio en caso de fallo de un disco duro.   
**RAID 5:** distribuirá los datos y la información de paridad entre varias unidades.  
**RAID 10:** replica los datos en diferentes discos y distribuye la carga de trabajo.  
Esta configuración permite que los servicios permanezcan activos incluso en caso de fallos en los discos y al mismo tiempo que garantiza un acceso a los datos a alta velocidad.

### **3\. Medidas de prevención de riesgos laborales**  {#3.-medidas-de-prevención-de-riesgos-laborales}

#### ***Seguridad elèctrica*** {#seguridad-elèctrica}

Una de las principales fuentes de riesgo dentro del centro de datos es la infraestructura eléctrica. Los servidores, los SAI, las PDU y los sistemas de alimentación funcionan a altas tensiones y están en funcionamiento continuo, lo que puede suponer riesgos de electrocución o sobrecalentamiento si no se manejan correctamente.

Para reducir estos riesgos, cualquier trabajo en equipos eléctricos debe ser realizado únicamente por personal autorizado y formado. Además, antes de manipular determinados componentes, el equipo debe desconectarse de forma segura siempre que sea posible.

**El personal técnico debe utilizar:**

* Guantes dieléctricos.  
* Herramientas aisladas.  
* Calzado de seguridad con suela aislante.

#### ***Control ambiental y condiciones de trabajo*** {#control-ambiental-y-condiciones-de-trabajo}

Los centros de datos generan grandes cantidades de calor debido al funcionamiento constante de los servidores y los equipos de red. Por este motivo, la sala estará equipada con sistemas de climatización que mantendrán unas condiciones ambientales estables para proteger los equipos y garantizar unas condiciones de trabajo adecuadas para el personal.

La temperatura y la humedad se mantendrán dentro de los niveles recomendados para evitar el estrés térmico, la condensación o la acumulación de electricidad estática. Además, las instalaciones se limpiarán periódicamente para evitar la acumulación de polvo, ya que esto puede afectar tanto a los equipos electrónicos como a la calidad del aire dentro de la sala.

#### ***Sonido y protección auditiva*** {#sonido-y-protección-auditiva}

Los sistemas de ventilación y refrigeración, así como los propios servidores, generan un nivel constante de ruido que puede resultar molesto o perjudicial en caso de exposición prolongada.

Para reducir la exposición, se recomienda limitar el tiempo que se pasa dentro del centro de datos y utilizar protección auditiva al realizar tareas prolongadas. 

#### ***Ergonomía*** {#ergonomía}

La distribución del CPD se diseñará de manera que los técnicos puedan trabajar de forma segura y cómoda. Los pasillos entre los racks serán lo suficientemente amplios como para facilitar el desplazamiento y las tareas de mantenimiento. Además, se recomienda el uso de carritos y herramientas de apoyo para mover servidores o componentes pesados, con el fin de prevenir lesiones musculoesqueléticas. 

**También se controlarán otros aspectos como:**

* La iluminación adecuada en la sala.  
* La organización del cableado en los racks para evitar cables sueltos en el suelo.  
* La señalización de las zonas peligrosas.

---

## Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS) {#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-(aws)}

### **2.1 Arquitectura de Red Virtual (VPC) y Seguridad Lógica** {#2.1-arquitectura-de-red-virtual-(vpc)-y-seguridad-lógica}

Antes de empezar con esto hemos hecho una imagen con respecto a nuestra distribución y cómo están conectados los servicios.  

<img width="1408" height="768" alt="Gemini_Generated_Image_s9d804s9d804s9d8" src="https://github.com/user-attachments/assets/876b1dfe-a120-4acc-8139-2f195a9b2646" />

#### ***2.1.1. Diseño de Subredes, Tablas de Enrutamiento e Internet Gateway*** {#2.1.1.-diseño-de-subredes,-tablas-de-enrutamiento-e-internet-gateway}

#### ***2.1.2. Configuración de Firewalls Lógicos (Security Groups)*** {#2.1.2.-configuración-de-firewalls-lógicos-(security-groups)}

### **2.2 Implementación de Servicios en Instancias EC2** {#2.2-implementación-de-servicios-en-instancias-ec2}

#### ***2.2.1. Servidor Web y Servicio SFTP Seguro (Autenticación AD)*** {#2.2.1.-servidor-web-y-servicio-sftp-seguro-(autenticación-ad)}

#### ***2.2.2. Servidor de Directorio Activo (LDAP/AD)*** {#2.2.2.-servidor-de-directorio-activo-(ldap/ad)}

Instalamos el paquete de ldap desde la terminal de una máquina linux  
<img width="594" height="54" alt="Captura de pantalla de 2026-05-19 10-16-03" src="https://github.com/user-attachments/assets/767dbb14-16c3-4a03-b1b2-ba3fdea274cf" />

Configuración del servicio de ldap  
<img width="737" height="378" alt="Captura de pantalla de 2026-05-19 10-25-46" src="https://github.com/user-attachments/assets/fb0c1295-dea1-4efe-963e-9ceb7714f826" />
<img width="737" height="378" alt="Captura de pantalla de 2026-05-19 10-27-17" src="https://github.com/user-attachments/assets/00a617e1-6956-4f89-9cda-2e7e8981f40e" />


Especificamos el nombre de dominio.  
<img width="737" height="378" alt="Captura de pantalla de 2026-05-19 10-26-33" src="https://github.com/user-attachments/assets/bc8c313d-6759-45cc-9fdd-e41ccefe07c7" />

Ponemos la contraseña de administrador de LDAP  
<img width="737" height="378" alt="Captura de pantalla de 2026-05-19 10-27-17" src="https://github.com/user-attachments/assets/758f590d-8062-4397-8bde-798c6bea29fe" />

Mensaje conforme la configuración ha sido correcta.
<img width="737" height="148" alt="Captura de pantalla de 2026-05-19 10-27-57" src="https://github.com/user-attachments/assets/832cd1dc-bdad-400a-b682-45456aa54608" />


Para organizar a los empleados y los grupos creamos un archivo .ldif

<img width="737" height="198" alt="Captura de pantalla de 2026-05-19 10-42-37" src="https://github.com/user-attachments/assets/f7bcbdb9-081d-4998-ac34-5c5da9b5d0c0" />


Ahora cargamos el archivo en la base de datos de LDAP y como se puede ver se ha añadido todo correctamente.

<img width="726" height="147" alt="Captura de pantalla de 2026-05-20 08-15-30" src="https://github.com/user-attachments/assets/5f1cf23b-b16a-4342-aa02-9ec2b8a3715a" />


Creamos el archivo usuarios.ldif para a posteriori poder crear los usuarios.

<img width="430" height="40" alt="Captura de pantalla de 2026-05-20 08-26-03" src="https://github.com/user-attachments/assets/748929d5-138f-4e77-8d7c-cc170d547960" />


Creación del usuario Eduardo

<img width="465" height="351" alt="Captura de pantalla de 2026-05-20 08-27-42" src="https://github.com/user-attachments/assets/90e3fa11-30e5-4277-b50e-623963e7b61e" />


Creación del usuario Pol  

<img width="443" height="278" alt="Captura de pantalla de 2026-05-20 08-29-44" src="https://github.com/user-attachments/assets/95ae1e9d-62bd-48e4-a344-c42b8f09d95e" />


Creación del usuario Lucia  

<img width="451" height="278" alt="Captura de pantalla de 2026-05-20 08-33-21" src="https://github.com/user-attachments/assets/c4c152af-fb03-4b6a-a765-ca1959e74f87" />


Creación del usuario Aleshka  

<img width="479" height="278" alt="Captura de pantalla de 2026-05-20 08-34-03" src="https://github.com/user-attachments/assets/09103ee9-a8a9-4a4a-8872-6beeaee17305" />


Añadimos los usuarios al directorio.

<img width="712" height="219" alt="Captura de pantalla de 2026-05-20 08-37-00" src="https://github.com/user-attachments/assets/c0fe2490-e566-4d4d-99b8-6815ef9c90d4" />


Asignamos contraseñas para cada uno de los usuarios en este caso @ITB2026 para todos para que cuando avancemos en el proyecto no haya confusiones o problemas.

<img width="712" height="241" alt="Captura de pantalla de 2026-05-20 08-39-33" src="https://github.com/user-attachments/assets/0e53ab2d-0c4b-47a4-ac2c-ee116cf3455c" />


Creamos el playbook de ansible:  

<img width="712" height="497" alt="Captura de pantalla de 2026-05-20 08-46-18" src="https://github.com/user-attachments/assets/dd04dc77-01d4-4b79-81b4-f81b596f9fe4" />



Ejecutamos el playbook y como se puede ver todo ha funcionado correctamente.

<img width="917" height="725" alt="Captura de pantalla de 2026-05-20 09-02-06" src="https://github.com/user-attachments/assets/208c3611-c24a-4ad6-bc48-41dac5c16cb6" />


#### ***2.2.3. Servidor de Centralización de Logs del Sistema*** {#2.2.3.-servidor-de-centralización-de-logs-del-sistema}

Desplegamos una máquina virtual VM-03 en AWS que nos servirá para centrar los logs, esta máquina tendrá como hardware virtual lo siguiente.  
**AMI** → Ubuntu server 24.04 LTS ya que es la más estable, tiene larga duración de soporte y su compatibilidad.  
**Tipo de instancia** → t3.medium, escogemos este ya que para nuestro proyecto necesitamos algo que nos vaya bien para los 7 servicios sin saturarse.  
**Grupo de seguridad** → Por el momento escogemos el grupo de seguridad por defecto pero más adelante tenemos que cambiarlo para asegurar que los servidores se comuniquen y garantizar su correcto funcionamiento.  
**Almacenamiento** → Para nuestro entorno reducido escogemos 30 GB  
![][image27]

### **2.3 Automatización, Accesos y Gestión de Configuración** {#2.3-automatización,-accesos-y-gestión-de-configuración}

#### ***2.3.1. Configuración de la Gestión Mediante Ansible (Playbooks)*** {#2.3.1.-configuración-de-la-gestión-mediante-ansible-(playbooks)}

#### ***2.3.2. Gestión de Usuarios de Administración y Políticas de Llave Pública/Privada*** {#2.3.2.-gestión-de-usuarios-de-administración-y-políticas-de-llave-pública/privada}

---

## **📻 3\. Implantación de Servicios Multimedia y Redes** {#📻-3.-implantación-de-servicios-multimedia-y-redes}

### **3.1. Servicio de Distribución de Audio Streaming** {#3.1.-servicio-de-distribución-de-audio-streaming}

**3.1.1. Descripción de la Funcionalidad del Servicio de Audio**  
**3.1.2. Guía de Instalación y Configuración del Servidor de Audio**  
**3.1.3. Justificación del Uso de Formatos Digitales (MP3/AAC/OGG)**  
**3.1.4. Pruebas de Validación, Acceso Web y Multi-cliente (Evidencias)**

### **3.2. Servicio de Vídeo Streaming y Videoconferencia** {#3.2.-servicio-de-vídeo-streaming-y-videoconferencia}

**3.2.1. Descripción de la Funcionalidad del Servicio de Vídeo**  
**3.2.2. Configuración del Servidor de Vídeo y Protocolos de Streaming (RTMP/HLS)**  
**3.2.3. Formatos y Códecs Utilizados (H.264 / MP4)**  
**3.2.4. Despliegue de la Plataforma de Videoconferencia (Jitsi Meet)**  
**3.2.5. Análisis del Protocolo WebRTC y Evidencias de Videollamada Real**

### **3.3. Pruebas Transversales de Rendimiento y Ancho de Banda** {#3.3.-pruebas-transversales-de-rendimiento-y-ancho-de-banda}

**3.3.1. Metodología de las Proves y Métricas (Download, Upload, Latencia)**  
**3.3.2. Análisis Correlativo del Consumo Multimedia Simultáneo**  
**3.3.3. Dictamen de Clasificación del Sistema (Acceptable / Not Acceptable)**  
**3.3.4. Propuestas Técnicas de Optimización**

---

# 4\. Diseño y Administración de la Base de Datos {#4.-diseño-y-administración-de-la-base-de-datos}

## 4.1. Diseño Conceptual, Lógico y Físico de la Base de Datos {#4.1.-diseño-conceptual,-lógico-y-físico-de-la-base-de-datos}

**4.1.1. Diagrama Entidad-Relación (E/R) Completo y Cardinalidades**  
**4.1.2. Transformación al Modelo Relacional (PK, FK y Restricciones)**  
**4.1.3. Justificación del SGBD Elegido e Implementación en EC2**  
**4.1.4. Evidencias de Creación de Tablas e Inserción de Datos de Prueba**

## 4.2. Seguridad, Roles y Scripting de Automatización {#4.2.-seguridad,-roles-y-scripting-de-automatización}

**4.2.1. Código Fuente del Script de Creación Automatizada (Bash/Python)**  
**4.2.2. Lógica del Script: Generación de .sql, Gestión de Errores y GRANT FILE**  
**4.2.3. Implementación de la Matriz de Roles (admin, vendes, administració, treballador)**

## 4.3. Programación del Motor: Triggers de Control y Auditoría {#4.3.-programación-del-motor:-triggers-de-control-y-auditoría}

**4.3.1. Triggers de Control de Cuotas Mensuales y Límites Diarios**  
**4.3.2. Infraestructura de Auditoría: Tabla de Avisos y Triggers de Acceso No Autorizado**  
**4.3.3. Trigger de Restricción Operativa por Bloqueo de Usuario**

## 4.4. Automatización de Copias de Seguridad  {#4.4.-automatización-de-copias-de-seguridad}

**4.4.1. Configuración del Evento Periódico y Sentencia SELECT INTO OUTFILE**  
**4.4.2. Mecanismo de Control y Registro en la Tabla de Backups**

---

## **📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital** {#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital}

*(Cubre las competencias específicas del Mòdul 1665\)*

### **5.1. Evaluación del Impacto de Seguridad e Importancia de las Datos** {#5.1.-evaluación-del-impacto-de-seguridad-e-importancia-de-las-datos}

**5.1.1. Informe de Evaluación de Riesgos y Seguridad Física/Lógica**  
**5.1.2. Valor Estratégico de los Datos en la Economía Digital y Normativa Internacional**

### **5.2. Optimización Tecnológica y Transformación Digital** {#5.2.-optimización-tecnológica-y-transformación-digital}

**5.2.1. Medidas de Optimización de Recursos e Impacto Ambiental de la Infraestructura**  
**5.2.2. Análisis de Transformación Digital: Alineación con los Objetivos Corporativos de Innovate Tech**  
---

## **📹 6\. Entregables Multimedia e Incidencias** {#📹-6.-entregables-multimedia-e-incidencias}

**6.1. Enlace al Vídeo Demostrativo Oficial (3 Minutos)**  
**6.2. Registro de Incidencias, Problemas Encontrados y Soluciones Aplicadas**  
