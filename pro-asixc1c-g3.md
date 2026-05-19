## **PROJECTE 2  E-COMMERCE AMB TELEGRAM**

## 

## 

## 

##            

POL GUERRERO GONZÁLEZ  
DANIEL XAVIER PÉREZ CHULCA  
ORIOL PLAZAS LEÓN  
**CURS:** SMX2A  
**PROFESSORS:** Abel Susín, Lina Camprubí, Fernando Rivero, Joaquim Tarinas, Joaquim Sabrià

## 

# **Projecte Transversal**

* **Nombre del proyecto: pro-asixc1c-g3**  
* **Miembros del grupo: Lucia Isabel Bartolomé, Eduardo Perales, Pol Guerrero, Aleshka Cisneros.**  
* **Centro: Institut Tecnològic de Barcelona (ITB)**  
* **Curso: 2025/2026**

## 

**[🏗️ 1\. Infraestructura del Centro de Procesamiento de Datos (CPD)	3](#🏗️-1.-infraestructura-del-centro-de-procesamiento-de-datos-\(cpd\))**

[**1.1. Diseño Arquitectónico y Ubicación Física	3**](#1.1.-diseño-arquitectónico-y-ubicación-física)

[**1.2. Infraestructura IT y Distribución de Racks	3**](#1.2.-infraestructura-it-y-distribución-de-racks)

[**1.3. Infraestructura Eléctrica y Continuidad de Negocio	3**](#1.3.-infraestructura-eléctrica-y-continuidad-de-negocio)

[**1.4. Seguridad Física y Prevención de Riesgos Laborales (PRL)	3**](#1.4.-seguridad-física-y-prevención-de-riesgos-laborales-\(prl\))

[**Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS)	4**](#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-\(aws\))

[**2.1. Arquitectura de Red Virtual (VPC) y Seguridad Lógica	4**](#2.1.-arquitectura-de-red-virtual-\(vpc\)-y-seguridad-lógica)

[**2.2. Implementación de Servicios en Instancias EC2	4**](#2.2.-implementación-de-servicios-en-instancias-ec2)

[**2.3. Automatización, Accesos y Gestión de Configuración	4**](#2.3.-automatización,-accesos-y-gestión-de-configuración)

[**📻 3\. Implantación de Servicios Multimedia y Redes	4**](#📻-3.-implantación-de-servicios-multimedia-y-redes)

[**3.1. Servicio de Distribución de Audio Streaming	4**](#3.1.-servicio-de-distribución-de-audio-streaming)

[**3.2. Servicio de Vídeo Streaming y Videoconferencia	4**](#3.2.-servicio-de-vídeo-streaming-y-videoconferencia)

[**3.3. Pruebas Transversales de Rendimiento y Ancho de Banda	5**](#3.3.-pruebas-transversales-de-rendimiento-y-ancho-de-banda)

[**🗄️ 4\. Diseño y Administración de la Base de Datos	5**](#🗄️-4.-diseño-y-administración-de-la-base-de-datos)

[**4.1. Diseño Conceptual, Lógico y Físico de la Base de Datos	5**](#4.1.-diseño-conceptual,-lógico-y-físico-de-la-base-de-datos)

[**4.2. Seguridad, Roles y Scripting de Automatización	5**](#4.2.-seguridad,-roles-y-scripting-de-automatización)

[**4.3. Programación del Motor: Triggers de Control y Auditoría	5**](#4.3.-programación-del-motor:-triggers-de-control-y-auditoría)

[**4.4. Automatización de Copias de Seguridad (Eventos)	6**](#4.4.-automatización-de-copias-de-seguridad-\(eventos\))

[**📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital	6**](#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital)

[**5.1. Evaluación del Impacto de Seguridad e Importancia de las Datos	6**](#5.1.-evaluación-del-impacto-de-seguridad-e-importancia-de-las-datos)

[**5.2. Optimización Tecnológica y Transformación Digital	6**](#5.2.-optimización-tecnológica-y-transformación-digital)

[**📹 6\. Entregables Multimedia e Incidencias	6**](#📹-6.-entregables-multimedia-e-incidencias)

## 

## **🏗️ 1\. Infraestructura del Centro de Procesamiento de Datos (CPD)** {#🏗️-1.-infraestructura-del-centro-de-procesamiento-de-datos-(cpd)}

***(Cubre el bloque de hardware Mòdul 0371 y sostenibilidad Mòdul 1665\)***

### **1.1. Diseño Arquitectónico y Ubicación Física** {#1.1.-diseño-arquitectónico-y-ubicación-física}

* **1.1.1. Ubicación de la Sala y Justificación**  
* **1.1.2. Medidas de Ocultación de la Infraestructura**  
* **1.1.3. Sistema de Climatización, Rangos Ambientales y Calidad del Aire**  
* **1.1.4. Especificaciones del Suelo y Techo Técnico**  
* **1.1.5. Planos de Planta y Distribución de la Sala**

### **1.2. Infraestructura IT y Distribución de Racks** {#1.2.-infraestructura-it-y-distribución-de-racks}

**1.2.1. Inventario de Hardware Físico (Servidores, Switches y Patch Panels)**

Para montar la infraestructura de Innovate Tech, la idea clave es no cometer el error típico de comprar un servidor físico para cada servicio. Eso sería carísimo, poco eficiente y tiraría por tierra la sostenibilidad del proyecto. En su lugar, vamos a usar virtualización : consolidamos todo en solo dos servidores físicos potentes y un almacenamiento centralizado para ahorrar energía y optimizar recursos.

Este es el hardware real que vamos a meter en el CPD:

* **2x Servidores Host (Dell PowerEdge R760 \- 2U cada uno):**   
  Son las dos máquinas principales donde irá el hipervisor para crear las máquinas virtuales. Llevan fuentes redundantes con certificación Titanium para no gastar luz de más (sostenibilidad) y tarjetas de red dobles a 10 Gbps para que no haya cuellos de botella.  
* **1x Cabina de Almacenamiento Centralizado (QNAP Enterprise ZFS NAS ES1642dc \- 3U):**   
  Aquí es donde guardaremos todos los datos de la empresa de forma centralizada. Elegimos este modelo porque tiene doble controladora activa (si una placa madre se quema, la otra sigue funcionando sin cortes). Además, usa el sistema de archivos ZFS y un entorno **RAID 6**, lo que significa que aunque se rompan dos discos a la vez, no perdemos ni un solo vídeo, audio o dato de la base de datos.  
* **2x Switches de Red (Cisco Catalyst 9300 \- 1U cada uno):**   
  Se encargan de conectar todo. Los configuramos en modo *Stack* (apilados físicamente). Así, la red los ve como un único switch gigante; si uno se apaga o falla, el otro absorbe todo el tráfico al instante para que la empresa no se quede colgada.  
* **2x Patch Panels Cat6A (24 puertos \- 1U cada uno):**   
  Sirven para organizar el cableado que viene de fuera del rack antes de conectarlo a los switches Cisco, protegiendo los puertos de estos últimos contra el desgaste de conectar y desconectar. Soporta velocidades de hasta 10 Gbps, algo fundamental para que las pruebas de ancho de banda salgan perfectas.  
    
  **1.2.2. Distribución Espacial de los Racks (Estructuración)**

El CPD va a tener 2 armarios Rack de 42U de altura. Los separamos de esta forma para organizar bien los flujos de aire (pasillo frío/caliente) y evitar que si falla algo, caiga toda la infraestructura a la vez:

**Rack 1: Servicios de Producción e Infraestructura Base**

Este armario se enfoca en las herramientas de gestión interna de la empresa.

* **Hardware:** Aquí dentro va el **Host 1 (Dell R760)**, un patch panel y el primer switch Cisco.  
* **Parte Virtual:** Dentro del Host 1 creamos tres **Máquinas Virtuales (VMs)** independientes:  
  * **`VM-01 (Servidor Web + SFTP Seguro):`** La web y la subida de archivos segura, que además se comunica con el directorio activo para los usuarios.  
  * **`VM-02 (Directorio Activo / LDAP):`** Donde guardamos las cuentas y permisos de todos los empleados.  
  * **`VM-03 (Servidor de Logs Centralizado):`** La máquina encargada de recoger los eventos y logs de seguridad de todo el CPD para tenerlo todo auditado.

Este armario se encarga de la parte pesada: streaming, videollamadas y la persistencia de datos.

* **Hardware:** Contiene el **Host 2 (Dell R760)**, la cabina de almacenamiento **QNAP NAS** y el segundo switch Cisco.   
* **Parte Virtual:** El Host 2 moverá estas cuatro **VMs** dedicadas al entorno multimedia:  
  * **VM-04 (Base de Datos Relacional):** El motor de la base de datos con toda la información de empleados, llamadas y medidas de red.  
  * **VM-05 (Streaming de Audio):** El servidor para la distribución de los canales de audio (MP3/AAC/OGG).  
  * **VM-06 (Streaming de Vídeo):** El servidor (Nginx/Jellyfin) para transmitir los vídeos en formato MP4/H.264.  
  * **VM-07 (Videoconferencia Jitsi Meet):** La plataforma para las videollamadas internas en tiempo real con WebRTC.

**Cómo funciona la Alta Disponibilidad (HA):** Al tener el almacenamiento en la cabina QNAP compartida entre los dos servidores, si el Host 1 se rompe o se apaga por mantenimiento, el Host 2 se da cuenta al instante y arranca las VMs del compañero de forma automática. Así, Innovate Tech nunca se queda sin servicio.

* **1.2.3. Gestión del Cableado Estructurado**

* **1.2.4. Diagramas de Alzado de los Racks**

### **1.3. Infraestructura Eléctrica y Continuidad de Negocio** {#1.3.-infraestructura-eléctrica-y-continuidad-de-negocio}

* **1.3.1. Diseño de la Alimentación Redundante**  
* **1.3.2. Memoria de Cálculo de la Carga en Vatios (W) y Voltiamperios (VA)**  
* **1.3.3. Dimensionamiento del Sistema de Alimentación Ininterrumpida (SAI)**  
* **1.3.4. Justificación del Tiempo de Autonomía de las Baterías**

### **1.4. Seguridad Física y Prevención de Riesgos Laborales (PRL)** {#1.4.-seguridad-física-y-prevención-de-riesgos-laborales-(prl)}

* **1.4.1. Sistemas de Control de Accesos y Registro**  
* **1.4.2. Circuito Cerrado de Televisión (CCTV) y Planos de Cobertura**  
* **1.4.3. Sistemas de Detección y Extinción de Incendios mediante Gas Limpio**  
* **1.4.4. Plan de Evacuación, Señalización y Medidas Generales de PRL**

---

## **Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS)** {#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-(aws)}

***(Cubre la implementación en la nube y automatización)***

### **2.1. Arquitectura de Red Virtual (VPC) y Seguridad Lógica** {#2.1.-arquitectura-de-red-virtual-(vpc)-y-seguridad-lógica}

* **2.1.1. Diseño de Subredes, Tablas de Enrutamiento e Internet Gateway**  
* **2.1.2. Configuración de Firewalls Lógicos (Security Groups)**

### **2.2. Implementación de Servicios en Instancias EC2** {#2.2.-implementación-de-servicios-en-instancias-ec2}

* **2.2.1. Servidor Web y Servicio SFTP Seguro (Autenticación AD)**  
* **2.2.2. Servidor de Directorio Activo (LDAP/AD)**  
* **2.2.3. Servidor de Centralización de Logs del Sistema**

### **2.3. Automatización, Accesos y Gestión de Configuración** {#2.3.-automatización,-accesos-y-gestión-de-configuración}

* **2.3.1. Configuración de la Gestión Mediante Ansible (Playbooks)**  
* **2.3.2. Gestión de Usuarios de Administración y Políticas de Llave Pública/Privada**

---

## **📻 3\. Implantación de Servicios Multimedia y Redes** {#📻-3.-implantación-de-servicios-multimedia-y-redes}

***(Cubre el bloque Mòdul 0375\)***

### **3.1. Servicio de Distribución de Audio Streaming** {#3.1.-servicio-de-distribución-de-audio-streaming}

* **3.1.1. Descripción de la Funcionalidad del Servicio de Audio**  
* **3.1.2. Guía de Instalación y Configuración del Servidor de Audio**  
* **3.1.3. Justificación del Uso de Formatos Digitales (MP3/AAC/OGG)**  
* **3.1.4. Pruebas de Validación, Acceso Web y Multi-cliente (Evidencias)**

### **3.2. Servicio de Vídeo Streaming y Videoconferencia** {#3.2.-servicio-de-vídeo-streaming-y-videoconferencia}

* **3.2.1. Descripción de la Funcionalidad del Servicio de Vídeo**  
* **3.2.2. Configuración del Servidor de Vídeo y Protocolos de Streaming (RTMP/HLS)**  
* **3.2.3. Formatos y Códecs Utilizados (H.264 / MP4)**  
* **3.2.4. Despliegue de la Plataforma de Videoconferencia (Jitsi Meet)**  
* **3.2.5. Análisis del Protocolo WebRTC y Evidencias de Videollamada Real**

### **3.3. Pruebas Transversales de Rendimiento y Ancho de Banda** {#3.3.-pruebas-transversales-de-rendimiento-y-ancho-de-banda}

* **3.3.1. Metodología de las Proves y Métricas (Download, Upload, Latencia)**  
* **3.3.2. Análisis Correlativo del Consumo Multimedia Simultáneo**  
* **3.3.3. Dictamen de Clasificación del Sistema (Acceptable / Not Acceptable)**  
* **3.3.4. Propuestas Técnicas de Optimización**

---

## **🗄️ 4\. Diseño y Administración de la Base de Datos** {#🗄️-4.-diseño-y-administración-de-la-base-de-datos}

***(Cubre el bloque Mòdul 0377\)***

### **4.1. Diseño Conceptual, Lógico y Físico de la Base de Datos** {#4.1.-diseño-conceptual,-lógico-y-físico-de-la-base-de-datos}

* **4.1.1. Diagrama Entidad-Relación (E/R) Completo y Cardinalidades**  
* **4.1.2. Transformación al Modelo Relacional (PK, FK y Restricciones)**  
* **4.1.3. Justificación del SGBD Elegido e Implementación en EC2**  
* **4.1.4. Evidencias de Creación de Tablas e Inserción de Datos de Prueba**

### **4.2. Seguridad, Roles y Scripting de Automatización** {#4.2.-seguridad,-roles-y-scripting-de-automatización}

* **4.2.1. Código Fuente del Script de Creación Automatizada (Bash/Python)**  
* **4.2.2. Lógica del Script: Generación de .sql, Gestión de Errores y GRANT FILE**  
* **4.2.3. Implementación de la Matriz de Roles (admin, vendes, administració, treballador)**

### **4.3. Programación del Motor: Triggers de Control y Auditoría** {#4.3.-programación-del-motor:-triggers-de-control-y-auditoría}

* **4.3.1. Triggers de Control de Cuotas Mensuales y Límites Diarios**  
* **4.3.2. Infraestructura de Auditoría: Tabla de Avisos y Triggers de Acceso No Autorizado**  
* **4.3.3. Trigger de Restricción Operativa por Bloqueo de Usuario**

### **4.4. Automatización de Copias de Seguridad (Eventos)** {#4.4.-automatización-de-copias-de-seguridad-(eventos)}

* **4.4.1. Configuración del Evento Periódico y Sentencia SELECT INTO OUTFILE**  
* **4.4.2. Mecanismo de Control y Registro en la Tabla de Backups**

---

## **📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital** {#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital}

***(Cubre las competencias específicas del Mòdul 1665\)***

### **5.1. Evaluación del Impacto de Seguridad e Importancia de las Datos** {#5.1.-evaluación-del-impacto-de-seguridad-e-importancia-de-las-datos}

* **5.1.1. Informe de Evaluación de Riesgos y Seguridad Física/Lógica**  
* **5.1.2. Valor Estratégico de los Datos en la Economía Digital y Normativa Internacional**

### **5.2. Optimización Tecnológica y Transformación Digital** {#5.2.-optimización-tecnológica-y-transformación-digital}

* **5.2.1. Medidas de Optimización de Recursos e Impacto Ambiental de la Infraestructura**  
* **5.2.2. Análisis de Transformación Digital: Alineación con los Objetivos Corporativos de Innovate Tech**

---

## **📹 6\. Entregables Multimedia e Incidencias** {#📹-6.-entregables-multimedia-e-incidencias}

* **6.1. Enlace al Vídeo Demostrativo Oficial (3 Minutos)**  
* **6.2. Registro de Incidencias, Problemas Encontrados y Soluciones Aplicadas**
