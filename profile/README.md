📊 Índice de Actividad Económica (IAE) – CIENFI

Este proyecto tiene como objetivo construir un indicador granular de actividad económica a nivel de barrio para las ciudades de Calí, Medellín y Bogotá, mediante el uso de modelos de aprendizaje profundo que integran múltiples fuentes de datos oficiales, satelitales y administrativas.

🚀 Objetivo del proyecto

Desarrollar un Índice de Actividad Económica (IAE) que permita monitorear, analizar y visualizar la dinámica económica desagregado por ciudad. Este índice busca convertirse en una herramienta de apoyo para la toma de decisiones en política pública, planificación urbana y evaluación territorial.

🧠 Metodología

El IAE se calcula a partir de un modelo de redes neuronales que identifica patrones complejos entre variables clave como:

	•	✨ Luminosidad nocturna satelital (VIIRS)
	•	🌫 Contaminación del aire
	•	🚇 Movilidad urbana (torniquetes de transporte público)
	•	👥 Densidad poblacional
	•	📦 Datos de actividad económica oficial (PIB trimestral)

Proceso general:

Fase 1 – Preparación y limpieza de bases de datos
Fase 2 – Calibración del modelo
Fase 3 – Visualización geoespacial
  
  Integración de los resultados en un diseminador cartográfico para exploración pública, acompañado de una guía técnica para su interpretación.

🗂 Estructura del repositorio principal
```
├── 01_night_lights/              # Procesamiento de imágenes VIIRS
├── 02_mgn_dane/                  # Geometrías y datos del Marco Geoestadístico Nacional
├── 03_gdp_colombia/              # PIB trimestral por localidad
├── 04_transporte/                # Datos de torniquetes del sistema de transporte
├── 05_nb_boundary/               # Fronteras y delimitaciones oficiales de barrios
├── 06_model/                     # Entrenamiento y calibración del modelo neuronal
├── 07_visualization/             # Visualización y despliegue del IAE
└── README.md                     # Este archivo
```

📦 Dependencias

	•	R ≥ 4.3.0
	•	Paquetes principales: tidyverse, sf, terra, keras, tensorflow, mapview, readxl, data.table, entre otros.
	•	Python (opcional): Para interoperabilidad con r-reticulate.

📍 Estado del proyecto

✅ Repositorios de datos funcionales
⚙️ Modelos en calibración
🗺 Visualizador en desarrollo

👥 Equipo

Este proyecto está siendo desarrollado por el Centro de Investigación en Economía y Finanzas.

📄 Licencia

Uso interno con fines de política pública. Se espera publicar los resultados bajo una licencia de uso abierto con atribución una vez finalizado el proyecto.

