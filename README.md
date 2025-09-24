# Descripción del Proyecto

El **Servicio de Salud Metropolitano** está desarrollando un sistema de apoyo basado en **inteligencia artificial** para optimizar el proceso de **derivación de víctimas de delitos** hacia los organismos y centros más adecuados, considerando variables como comuna de residencia, edad, sexo, situación migratoria y tipo de delito, entre otras.  

Actualmente, la derivación se realiza de forma manual por parte de funcionarios, quienes deben revisar extensas listas de centros, lo que genera un proceso lento y con alta carga administrativa. El nuevo sistema busca **automatizar esta decisión**, reduciendo tiempos de respuesta y asegurando mayor precisión en la elección del centro de apoyo.  

## Componentes de la solución tecnológica

- **Backend en FastAPI**  
  - Integra un **agente de IA de OpenAI** encargado de analizar los casos y recomendar el centro más pertinente.  
  - La **API** no solo entrega las sugerencias de la IA, sino que también **registra las derivaciones en la base de datos** y mantiene la trazabilidad de cada caso.  
  - Administra la interacción con la **base de datos PostgreSQL**, que contiene información estructurada sobre comunas, provincias, tipos de delitos, centros disponibles y sus características.  

- **Frontend en React**  
  - **Módulo de ingreso y registro de derivaciones**: los funcionarios ingresan los datos del caso, reciben la recomendación de la IA y confirman la derivación, que luego se almacena en la base de datos a través de la API.  
  - **Dashboard interactivo de indicadores (KPIs)**: permite visualizar en tiempo real métricas clave como tiempos de atención, distribución geográfica, tipos de delitos más frecuentes y capacidad de respuesta de los centros.  

## Impacto esperado

Con este proyecto, el Servicio busca:  
- **Mejorar la atención a víctimas**.  
- **Aumentar la eficiencia de los equipos**.  
- **Fortalecer la coordinación interinstitucional**.  
- Disponer de **información estratégica en tiempo real** para la gestión en salud y seguridad pública.  
