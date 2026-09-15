# Alcance Futuro del Sistema 

## Visión General
Aunque la versión actual del Catálogo de Recursos Académicos se centra en la organización, almacenamiento estructurado y control de versiones, una versión futura evolucionará hacia un entorno de trabajo dinámico. El objetivo a largo plazo es transformar el repositorio en una plataforma automatizada que asista activamente en la experimentación, validación de código y gestión de flujos de trabajo de ingeniería.

## Funcionalidades Propuestas

1. **Generación Automática de Análisis Exploratorio (EDA):**
   Implementar un script de monitoreo que detecte automáticamente cuando se agreguen nuevos archivos CSV o SQL a la carpeta `data/`. Al detectarlos, el sistema ejecutará un pipeline que genere un reporte estadístico preliminar y visualizaciones básicas (usando librerías gráficas), guardando un cuaderno de resumen en la carpeta `notebooks/`.

2. **Módulo de Seguimiento de Experimentos Predictivos:**
   Integrar un sistema de registro ligero en los `notebooks/` y `src/` para capturar automáticamente las métricas de rendimiento y los hiperparámetros cada vez que se entrene un modelo de Machine Learning. Esto permitirá llevar un historial estructurado para comparar qué iteraciones de algoritmos y configuraciones ofrecen mejores predicciones a lo largo del tiempo.

3. **Pipeline de Validación de Código y Hardware (CI/CD Local):**
   Incorporar flujos de trabajo automatizados que verifiquen la integridad del código al hacer commits. Esto incluiría pruebas de sintaxis para scripts de Python, validación de consultas SQL complejas (como operaciones de agrupación o uniones múltiples), y un compilador de prueba para código de microcontroladores y circuitos (C/C++) almacenado en el repositorio.

4. **Generador Automatizado de Desglose de Proyectos:**
   Desarrollar una herramienta que lea etiquetas o metadatos específicos dentro de los apuntes de la carpeta `docs/` y genere automáticamente representaciones visuales del progreso del proyecto, como una Estructura de Desglose del Trabajo (EDT). Esto alinearía la gestión de los recursos académicos con metodologías y estándares profesionales de dirección de proyectos.