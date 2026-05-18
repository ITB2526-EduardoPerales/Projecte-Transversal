# **Projecte Transversal**

* **Nombre del proyecto:** pro-asixc1c-g3  
* **Miembros del grupo:** Lucia Isabel Bartolomé, Eduardo Perales, Pol Guerrero, Aleshka Cisneros.  
* **Centro:** Institut Tecnològic de Barcelona (ITB)  
* **Curso:** 2025/2026

[🏗️ 1\. Infraestructura del Centro de Procesamiento de Datos (CPD)](#🏗️-1.-infraestructura-del-centro-de-procesamiento-de-datos-\(cpd\))

[1.1.](#1.1.-diseño-arquitectónico-y-ubicación-física)

[1.2.](#1.2.)

[1.3.](#1.3.)

[1.4.](#1.4.)

[Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS)](#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-\(aws\))

[2.1.](#2.1.)

[2.2.](#2.2.)

[2.3. Automatización, Accesos y Gestión de Configuración](#2.3.-automatización,-accesos-y-gestión-de-configuración)

[📻 3\. Implantación de Servicios Multimedia y Redes](#📻-3.-implantación-de-servicios-multimedia-y-redes)

[3.1.](#3.1.)

[3.2.](#3.2.)

[3.3.](#3.3.)

[🗄️ 4\. Diseño y Administración de la Base de Datos](#🗄️-4.-diseño-y-administración-de-la-base-de-datos)

[4.1.](#4.1.)

[4.2.](#4.2.)

[4.3.](#4.3.)

[4.4.](#4.4.)

[📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital](#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital)

[5.1.](#5.1.)

[5.2.](#5.2.)

[📹 6\. Entregables Multimedia e Incidencias](#📹-6.-entregables-multimedia-e-incidencias)

## 

## 

## **🏗️ 1\. Infraestructura del Centro de Procesamiento de Datos (CPD)** {#🏗️-1.-infraestructura-del-centro-de-procesamiento-de-datos-(cpd)}

*(Cubre el bloque de hardware Mòdul 0371 y sostenibilidad Mòdul 1665\)*

### **1.1.** Diseño Arquitectónico y Ubicación Física {#1.1.-diseño-arquitectónico-y-ubicación-física}

* 1.1.1. Ubicación de la Sala y Justificación  
* 1.1.2. Medidas de Ocultación de la Infraestructura  
* 1.1.3. Sistema de Climatización, Rangos Ambientales y Calidad del Aire  
* 1.1.4. Especificaciones del Suelo y Techo Técnico  
* 1.1.5. Planos de Planta y Distribución de la Sala

### **1.2.** {#1.2.}

Infraestructura IT y Distribución de Racks

* 1.2.1. Inventario de Hardware Físico (Servidores, Switches y Patch Panels)  
* 1.2.2. Distribución Espacial de los Racks (Estructuración)  
* 1.2.3. Gestión del Cableado Estructurado  
* 1.2.4. Diagramas de Alzado de los Racks

### **1.3.** {#1.3.}

Infraestructura Eléctrica y Continuidad de Negocio

* 1.3.1. Diseño de la Alimentación Redundante  
* 1.3.2. Memoria de Cálculo de la Carga en Vatios (W) y Voltiamperios (VA)  
* 1.3.3. Dimensionamiento del Sistema de Alimentación Ininterrumpida (SAI)  
* 1.3.4. Justificación del Tiempo de Autonomía de las Baterías

### **1.4.** {#1.4.}

Seguridad Física y Prevención de Riesgos Laborales (PRL)

* 1.4.1. Sistemas de Control de Accesos y Registro  
* 1.4.2. Circuito Cerrado de Televisión (CCTV) y Planos de Cobertura  
* 1.4.3. Sistemas de Detección y Extinción de Incendios mediante Gas Limpio  
* 1.4.4. Plan de Evacuación, Señalización y Medidas Generales de PRL

---

## **Nube☁️ 2\. Despliegue de la Infraestructura Lógica en el Núvol (AWS)** {#nube☁️-2.-despliegue-de-la-infraestructura-lógica-en-el-núvol-(aws)}

*(Cubre la implementación en la nube y automatización)*

### **2.1.** {#2.1.}

Arquitectura de Red Virtual (VPC) y Seguridad Lógica

* 2.1.1. Diseño de Subredes, Tablas de Enrutamiento e Internet Gateway  
* 2.1.2. Configuración de Firewalls Lógicos (Security Groups)

### **2.2.** {#2.2.}

Implementación de Servicios en Instancias EC2

* 2.2.1. Servidor Web y Servicio SFTP Seguro (Autenticación AD)  
* 2.2.2. Servidor de Directorio Activo (LDAP/AD)  
* 2.2.3. Servidor de Centralización de Logs del Sistema

### **2.3. Automatización, Accesos y Gestión de Configuración** {#2.3.-automatización,-accesos-y-gestión-de-configuración}

* 2.3.1. Configuración de la Gestión Mediante Ansible (Playbooks)  
* 2.3.2. Gestión de Usuarios de Administración y Políticas de Llave Pública/Privada

---

## **📻 3\. Implantación de Servicios Multimedia y Redes** {#📻-3.-implantación-de-servicios-multimedia-y-redes}

*(Cubre el bloque Mòdul 0375\)*

### **3.1.** {#3.1.}

Servicio de Distribución de Audio Streaming

* 3.1.1. Descripción de la Funcionalidad del Servicio de Audio  
* 3.1.2. Guía de Instalación y Configuración del Servidor de Audio  
* 3.1.3. Justificación del Uso de Formatos Digitales (MP3/AAC/OGG)  
* 3.1.4. Pruebas de Validación, Acceso Web y Multi-cliente (Evidencias)

### **3.2.** {#3.2.}

Servicio de Vídeo Streaming y Videoconferencia

* 3.2.1. Descripción de la Funcionalidad del Servicio de Vídeo  
* 3.2.2. Configuración del Servidor de Vídeo y Protocolos de Streaming (RTMP/HLS)  
* 3.2.3. Formatos y Códecs Utilizados (H.264 / MP4)  
* 3.2.4. Despliegue de la Plataforma de Videoconferencia (Jitsi Meet)  
* 3.2.5. Análisis del Protocolo WebRTC y Evidencias de Videollamada Real

### **3.3.** {#3.3.}

Pruebas Transversales de Rendimiento y Ancho de Banda

* 3.3.1. Metodología de las Proves y Métricas (Download, Upload, Latencia)  
* 3.3.2. Análisis Correlativo del Consumo Multimedia Simultáneo  
* 3.3.3. Dictamen de Clasificación del Sistema (Acceptable / No Acceptable)  
* 3.3.4. Propuestas Técnicas de Optimización

---

## **🗄️ 4\. Diseño y Administración de la Base de Datos** {#🗄️-4.-diseño-y-administración-de-la-base-de-datos}

*(Cubre el bloque Mòdul 0377\)*

### **4.1.** {#4.1.}

Diseño Conceptual, Lógico y Físico de la Base de Datos

* 4.1.1. Diagrama Entidad-Relación (E/R) Completo y Cardinalidades  
* 4.1.2. Transformación al Modelo Relacional (PK, FK y Restricciones)  
* 4.1.3. Justificación del SGBD Elegido e Implementación en EC2  
* 4.1.4. Evidencias de Creación de Tablas e Inserción de Datos de Prueba

### **4.2.** {#4.2.}

Seguridad, Roles y Scripting de Automatización

* 4.2.1. Código Fuente del Script de Creación Automatizada (Bash/Python)  
* 4.2.2. Lógica del Script: Generación de .sql, Gestión de Errores y GRANT FILE  
* 4.2.3. Implementación de la Matriz de Roles (admin, vendes, administracio, treballador)

### **4.3.** {#4.3.}

Programación del Motor: Triggers de Control y Auditoría

* 4.3.1. Triggers de Control de Cuotas Mensuales y Límites Diarios  
* 4.3.2. Infraestructura de Auditoría: Tabla de Avisos y Triggers de Acceso No Autorizado  
* 4.3.3. Trigger de Restricción Operativa por Bloqueo de Usuario

### **4.4.** {#4.4.}

Automatización de Copias de Seguridad (Eventos)

* 4.4.1. Configuración del Evento Periódico y Sentencia SELECT INTO OUTFILE  
* 4.4.2. Mecanismo de Control y Registro en la Tabla de Backups

---

## **📊 5\. Sostenibilidad, Gestión del Cambio y Transformación Digital** {#📊-5.-sostenibilidad,-gestión-del-cambio-y-transformación-digital}

*(Cubre las competencias específicas del Mòdul 1665\)*

### **5.1.** {#5.1.}

Evaluación del Impacto de Seguridad e Importancia de las Datos

* 5.1.1. Informe de Evaluación de Riesgos y Seguridad Física/Lógica  
* 5.1.2. Valor Estratégico de los Datos en la Economía Digital y Normativa Internacional

### **5.2.** {#5.2.}

Optimización Tecnológica y Transformación Digital

* 5.2.1. Medidas de Optimización de Recursos e Impacto Ambiental de la Infraestructura  
* 5.2.2. Análisis de Transformación Digital: Alineación con los Objetivos Corporativos de Innovate Tech

---

## **📹 6\. Entregables Multimedia e Incidencias** {#📹-6.-entregables-multimedia-e-incidencias}

* 6.1. Enlace al Vídeo Demostrativo Oficial (3 Minutos)  
* 6.2. Registro de Incidencias, Problemas Encontrados y Soluciones Aplicadas
