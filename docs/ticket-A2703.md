# Detalle del Ticket de Alerta: A-2703

| Atributo | Detalle |
| :--- | :--- |
| **ID del Ticket** | [cite_start]A-2703 [cite: 1] |
| **Alerta** | [cite_start]SERVER-MAIL Phishing attempt possible download of malware [cite: 1] |
| **Severidad** | [cite_start]Media [cite: 1] |
| **Estado** | [cite_start]**Escalado** [cite: 55] |

## 1. Análisis del Mensaje de Correo
- [cite_start]**Remitente:** Def Communications `<76tguyhh6tgftrt7tg.su>` (IP: 114.114.114.114)[cite: 5].
- [cite_start]**Destinatario:** `<hr@inergy.com>` (IP: 176.157.125.93)[cite: 7].
- [cite_start]**Asunto:** Re: Infrastructure Egnieer role[cite: 7].
- [cite_start]**Contenido:** El remitente solicita una posición de ingeniero y adjunta un supuesto currículum[cite: 8].

## 2. Evidencia Técnica (IoCs)
- [cite_start]**Archivo Adjunto:** `bfsvc.exe`[cite: 10].
- [cite_start]**Hash SHA256:** `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`[cite: 4].
- [cite_start]**Comprobación:** El hash ha sido verificado como malicioso mediante herramientas de inteligencia[cite: 51].
- [cite_start]**Observación:** El archivo está protegido por la contraseña `paradise10789` para intentar evadir el análisis automático de los gateways de correo[cite: 9].

## 3. Resolución y Comentarios
Se confirma que el correo es un intento de phishing legítimo. [cite_start]Debido a la presencia confirmada de malware ejecutable y la severidad del objetivo (RRHH), el ticket se escala siguiendo el paso 3.2 del manual de estrategias[cite: 53, 54].
