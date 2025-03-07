# Proyecto-Integrado-2

# Análisis de Comportamiento de Usuario para una Aplicación de Productos Alimenticios

## Descripción del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los usuarios y las usuarias en una empresa emergente que vende productos alimenticios. El enfoque principal será:
- Estudiar el embudo de ventas para entender cómo los usuarios llegan a la etapa de compra y dónde se detienen en el proceso.
- Evaluar los resultados de un experimento A/A/B para tomar decisiones informadas sobre posibles cambios de diseño en la aplicación.

## Objetivos del Análisis

1. **Embudo de Ventas**: Identificar las etapas críticas donde los usuarios se pierden y calcular las proporciones de avance entre etapas.
2. **Prueba A/A/B**: Comparar el desempeño de dos grupos de control y un grupo experimental para determinar el impacto del cambio de fuentes en los resultados.

## Descripción de los Datos

El dataset contiene registros de eventos generados por los usuarios. Cada entrada incluye:
- `EventName`: Nombre del evento.
- `DeviceIDHash`: Identificador único del usuario.
- `EventTimestamp`: Fecha y hora del evento.
- `ExpId`: Número de experimento (246 y 247 son los grupos de control, 248 es el grupo de prueba).

## Pasos del Análisis

### 1. Preparación de los Datos
- Renombrar las columnas para mayor comodidad.
- Revisar y limpiar datos ausentes o inconsistentes.
- Agregar columnas para fechas y horas separadas.

### 2. Exploración Inicial
- Contar el número total de eventos y usuarios únicos.
- Calcular el promedio de eventos por usuario.
- Determinar el rango de fechas y filtrar los datos incompletos.

### 3. Estudio del Embudo de Ventas
- Identificar y clasificar los eventos por frecuencia.
- Calcular la proporción de usuarios que realizan cada evento.
- Construir el embudo de eventos y analizar las transiciones entre etapas.

### 4. Análisis A/A/B
- Validar la similitud entre los grupos de control (246 y 247).
- Comparar el desempeño del grupo experimental (248) con los grupos de control, evento por evento.
- Evaluar la significancia estadística de las diferencias entre grupos.

### 5. Consideraciones Estadísticas
- Establecer un nivel de significancia adecuado (por ejemplo, 0.05) y ajustar en función del número de pruebas realizadas.
- Revisar conclusiones basadas en las pruebas estadísticas.

## Herramientas Usadas
- Python para el análisis de datos.
- Bibliotecas clave: Pandas, NumPy, Matplotlib, Seaborn y SciPy.
- Entorno: Jupyter Notebook o cualquier IDE de tu preferencia.



