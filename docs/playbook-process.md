# Metodología de Respuesta: Phishing Playbook v1.0

[cite_start]Este documento detalla el cumplimiento del protocolo institucional para la resolución del incidente A-2703, basado en el Manual de Estrategias de Phishing de la organización[cite: 11, 12].

## 1. Propósito
[cite_start]El objetivo de este proceso es proporcionar una respuesta oportuna y adecuada a un incidente de phishing por parte de un analista de SOC de nivel uno[cite: 23].

## 2. Flujo de Trabajo Aplicado

### Paso 1: Recepción de la Alerta
* [cite_start]Se detectó y accedió al ticket de alerta **A-2703** indicando un posible intento de descarga de malware[cite: 1, 27].

### Paso 2: Evaluación de la Alerta
[cite_start]Se analizaron los siguientes elementos del ticket para determinar la legitimidad de la amenaza[cite: 28, 29]:
* [cite_start]**Severidad:** Clasificada como **Media**, lo que indica que puede requerir escalación[cite: 1, 33].
* [cite_start]**Detalles del Remitente:** Se identificó la dirección externa `76tguyhh6tgftrt7tg.su` y la IP `114.114.114.114`[cite: 5, 38, 39].
* [cite_start]**Detalles del Receptor:** El objetivo fue el departamento de Recursos Humanos (`hr@inergy.com`)[cite: 7, 35].
* [cite_start]**Cuerpo del Mensaje:** Se detectaron errores gramaticales y una solicitud inusual de uso de contraseña para abrir un currículum[cite: 8, 9, 41].

### Paso 3.0: Identificación de Enlaces o Archivos Adjuntos
* [cite_start]Se confirmó que el correo electrónico contenía un archivo adjunto llamado `bfsvc.exe`[cite: 10, 46].
* [cite_start]Siguiendo el protocolo, se procedió al análisis del archivo sin abrirlo en un entorno no aislado[cite: 43, 47].

### Paso 3.1: Determinación de Malicia
* [cite_start]Se verificó la reputación del archivo utilizando su valor hash: `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`[cite: 4, 51].
* [cite_start]El hash fue confirmado como **malicioso** mediante herramientas de inteligencia de amenazas[cite: 51].

### Paso 3.2: Actualización y Escalación
* [cite_start]Al confirmar que el archivo es malicioso, se procedió a la escalación del incidente[cite: 54].
* [cite_start]El estado del ticket se actualizó a **Escalado**[cite: 55].
* [cite_start]Se notificó a un analista de SOC de nivel dos para continuar con la contención[cite: 55].

---

## 3. Diagrama de Decisiones
El análisis se basó en el siguiente diagrama de flujo lógico:

1. [cite_start]**¿Contiene archivos adjuntos?** SÍ -> [Proceder a Paso 3.1][cite: 62].
2. [cite_start]**¿Es malicioso el archivo?** SÍ -> [Proceder a Paso 3.2: Escalar][cite: 62].
