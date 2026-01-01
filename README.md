# Investigación de Incidente de Phishing - Caso A-2703

## Descripción del Proyecto
Este repositorio documenta el análisis y la respuesta a un incidente de seguridad real simulado. El objetivo es demostrar la capacidad de identificar, investigar y escalar una amenaza de phishing siguiendo un protocolo de actuación (Playbook) profesional en un entorno de Centro de Operaciones de Seguridad (SOC).

## Escenario
Como Analista de SOC Nivel 1, recibí una alerta de severidad media sobre un posible intento de descarga de malware a través de un correo de phishing dirigido al departamento de Recursos Humanos.

## Herramientas y Metodología
- **Análisis de Hash:** Verificación de integridad y reputación mediante herramientas de inteligencia de amenazas (VirusTotal).
- **Playbook de Respuesta:** Seguimiento del flujo de trabajo institucional para la evaluación y escalación de incidentes.
- **Documentación:** Registro detallado en ticket de soporte y diario de gestión.

## Hallazgos Clave
- [cite_start]**IoC (Indicador de Compromiso):** Hash de archivo verificado como malicioso[cite: 4].
- [cite_start]**Táctica:** Ingeniería social mediante oferta de empleo con archivo ejecutable camuflado[cite: 8, 10].
- [cite_start]**Estado Final:** Escalado a Nivel 2 para contención avanzada[cite: 55].
