# Auditoria de Gobernanza y Privacidad: Dataset SABER 11 (2020-2)

**Curso:** Gestion y Gobernanza de Datos
**Profesor:** Santiago Jimenez Londono
**Integrantes:** Agustin Figueroa Sierra, Samuel Aristizabal Alzate

## Descripcion del Proyecto

Este repositorio contiene el trabajo final del curso de Gestion y Gobernanza de Datos. El objetivo principal es auditar un dataset publico real (Saber 11, periodo 2020-2 del ICFES) asumiendo el rol de un area de gobierno de datos. 

La auditoria se enfoca en evaluar la calidad de los datos, identificar informacion personal sensible (PII), medir los riesgos de re-identificacion mediante k-anonymity, y proponer un plan de remediacion basado en los marcos de referencia DAMA-DMBOK2.

## Contenido del Repositorio

* **cuaderno.ipynb:** Cuaderno de Jupyter (o Google Colab) que ejecuta de manera secuencial la auditoria tecnica. Incluye el perfilado de datos, deteccion automatica de PII, analisis de k-anonymity y aplicacion del plan de remediacion.
* **Informe_Final_Gobernanza.pdf:** Version PDF del informe ejecutivo. Detalla el resumen de hallazgos, el mapeo de capacidades de DAMA, resultados de calidad y privacidad, y recomendaciones tecnicas.
* **images/:** Directorio que almacena las visualizaciones estadisticas generadas por el cuaderno de auditoria.

*Nota: El dataset original (`Saber_11_2020-2_20260512.csv`) no se incluye directamente en el control de versiones debido a restricciones de tamano, pero puede ser descargado desde el portal datos.gov.co.*

## Instrucciones de Ejecucion Local

Para reproducir los analisis ejecutados en el cuaderno de Jupyter:

1. Clonar el repositorio.
2. Descargar el dataset original desde el portal oficial y colocar el archivo `.csv` en la raiz del proyecto.
3. Crear un entorno virtual (recomendado) e instalar las dependencias:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
4. Ejecutar el cuaderno de forma secuencial:
   ```bash
   jupyter notebook cuaderno.ipynb
   ```
