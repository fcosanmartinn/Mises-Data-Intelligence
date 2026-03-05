# 📊 Mises Data Intelligence

## Descripción del Proyecto
*Mises Data Intelligence* es una aplicación de escritorio diseñada para optimizar la extracción, limpieza y formateo de bases de datos macroeconómicas y sociales provenientes de *Our World in Data (OWID)*. 

### El Problema
Descargar bases de datos globales para la investigación económica suele implicar horas de trabajo manual y repetitivo. Los analistas se enfrentan a tres grandes obstáculos:
1. *Ruido Global:* Tener que aislar manualmente los datos de interés entre cientos de países y regiones agregadas.
2. *Jerga Técnica:* Trabajar con identificadores de base de datos (slugs) en lugar de nombres de variables legibles.
3. *Corrupción de Formatos Regionales:* El problema más crítico al cruzar información entre plataformas. Al descargar datos crudos con formato estadounidense (puntos decimales), Excel en Hispanoamérica suele malinterpretar estos valores como separadores de miles, destruyendo la integridad matemática de toda la base de datos (por ejemplo, leyendo un 1.73% como un 173%).

### La Solución
Esta herramienta automatiza y blinda todo el proceso. Con solo ingresar el identificador de un gráfico de OWID, la aplicación se conecta a la base de datos cruda y ejecuta un procesamiento inteligente:
* *Filtra automáticamente* la información, aislando exclusivamente a los países de Hispanoamérica.
* *Limpia los metadatos*, transformando los códigos técnicos en encabezados claros y estandarizados.
* *Exporta la data blindada* ofreciendo dos vías: un archivo *XLSX (Excel)* nativo que garantiza un formato numérico perfecto a prueba de configuraciones regionales, y un archivo *CSV* estructurado, ideal para inyectar en modelos de Python, R o SQL.

En resumen, Mises Data Intelligence transforma un proceso de extracción y limpieza que tomaría horas en una tarea de un solo clic, garantizando datos 100% íntegros y listos para la toma de decisiones.

## 🚀 Cómo Descargar e Instalar

### 🪟 Para usuarios de Windows (Recomendado)
No necesitas instalar Python ni saber de código. Solo sigue estos pasos:
1. Ve a la sección de **Releases** (Lanzamientos) en la barra lateral derecha de esta página en GitHub.
2. Descarga el archivo comprimido más reciente (ej. `Mises_Data_Intelligence_v1.0.zip`).
3. Extrae la carpeta en tu computadora (Clic derecho > Extraer todo).
4. Haz doble clic en el ejecutable `Mises Data Intelligence.exe`. La interfaz se abrirá automáticamente en tu navegador y estará lista para usar.

### 🍎 Para usuarios de macOS / Linux
Debido a las políticas de seguridad de Apple con aplicaciones nuevas, la forma más rápida y segura de usar la herramienta es ejecutándola directamente desde el código fuente:
1. Descarga el repositorio haciendo clic en el botón verde **Code > Download ZIP** en la parte superior de esta página.
2. Extrae la carpeta, preferiblemente en tus Descargas.
3. Abre la **Terminal** y asegúrate de tener instalado Python 3.
4. Instala las librerías necesarias ejecutando este comando:
   ```bash
   pip3 install eel pandas openpyxl charset-normalizer
