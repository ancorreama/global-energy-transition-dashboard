# ¿Está el mundo reduciendo realmente su dependencia de los combustibles fósiles?

## Contexto

La transición energética se ha convertido en uno de los principales desafíos globales del siglo XXI. A medida que aumenta la demanda de electricidad y se intensifican los compromisos climáticos, surge una pregunta clave:

**¿Está el mundo reduciendo realmente su dependencia de los combustibles fósiles?**

Este proyecto analiza la evolución de la infraestructura energética mundial utilizando la *Global Power Plant Database* del World Resources Institute (WRI), que recopila información sobre miles de plantas de generación eléctrica en todo el mundo.

A partir de este dataset se exploran:

- La distribución geográfica de la infraestructura energética global
- La composición de la matriz energética por fuente de generación
- La evolución de la capacidad instalada a lo largo del tiempo
- El crecimiento de las energías renovables frente a los combustibles fósiles

El objetivo principal es evaluar si el crecimiento de las energías renovables está transformando de manera significativa la matriz energética global o si los combustibles fósiles continúan dominando la capacidad instalada.

---

## Dashboard interactivo

Puedes explorar el dashboard aquí:

👉 https://lookerstudio.google.com/reporting/f4a1ceea-c95c-4fbd-8564-4f958d331333/page/p_ojp39amd1d

---

## Fuente de datos

World Resources Institute (WRI)  
Global Power Plant Database  
https://datasets.wri.org/datasets/global-power-plant-database

---

## Herramientas utilizadas

- Google Sheets (limpieza y preparación de datos)
- Looker Studio (visualización y storytelling)
- GitHub Pages (presentación web)

---

## Documentación del modelado de datos

El proceso de preparación y modelado de datos se realizó en Python utilizando la base original **Global Power Plant Database** del World Resources Institute (WRI).

### Principales etapas del modelado

**1. Carga de datos**
Se importó el archivo original en formato CSV mediante la librería pandas.

**2. Limpieza de datos**
- Eliminación de registros duplicados.
- Remoción de valores nulos en variables clave.
- Filtrado de plantas con capacidad no válida.

**3. Transformación de variables**
Se generaron nuevas variables para facilitar el análisis:

- Clasificación de tipo de energía: Renovable / No renovable.
- Conversión de capacidad instalada de MW a GW.
- Cálculo de antigüedad de las plantas.
- Transformación de variables temporales a formato largo para análisis de tendencias.

**4. Selección final de columnas**
Se conservaron únicamente variables relevantes para optimizar el rendimiento del dashboard en Looker Studio.

**5. Exportación**
La base final fue exportada a CSV y cargada en Google Sheets para su conexión con Looker Studio.

---

📄 La documentación completa del proceso se encuentra disponible en este repositorio:

👉 [Documentación completa del modelado] [DocumentaciónModeladoDatos_ProyectoFinal_Grupo4.pdf](https://github.com/user-attachments/files/25890073/DocumentacionModeladoDatos_ProyectoFinal_Grupo4.pdf)

👉 Conuslta aquí el código https://colab.research.google.com/drive/1HgNM5fyoVaInyZKgPkH-Q68hpG5WQLP4?usp=sharing

---

## Equipo

**DataSquad**  
Proyecto académico de visualización de datos
