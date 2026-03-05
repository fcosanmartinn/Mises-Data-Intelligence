# 📊 Mises Data Intelligence

**Mises Data Intelligence** automatiza la extracción y limpieza de datos macroeconómicos desde Our World in Data. Filtra información para Hispanoamérica, estandariza variables técnicas y exporta en XLSX o CSV para blindar los números contra errores regionales de Excel. Una herramienta esencial para la investigación económica.

## ✨ Características Principales
* **Filtro Regional Automático:** Aísla la información exclusiva de los países hispanoamericanos.
* **Limpieza de Variables:** Transforma los códigos técnicos (slugs) en encabezados legibles.
* **Exportación en XLSX:** Archivo nativo de Excel que previene la corrupción de decimales por configuraciones regionales.
* **Exportación en CSV:** Texto plano optimizado para programadores, bases de datos y machine learning.

## 🚀 Cómo Descargar e Instalar

### 🪟 Para usuarios de Windows (Recomendado)
No necesitas instalar Python ni saber de código. Solo sigue estos pasos:
1. Ve a la sección de **Releases** (Lanzamientos) en la barra lateral derecha de esta página.
2. Descarga el archivo comprimido más reciente (ej. `Mises_Data_Intelligence_v1.0.zip`).
3. Extrae la carpeta en tu computadora (Clic derecho > Extraer todo).
4. Haz doble clic en el ejecutable `Mises Data Intelligence.exe`. La interfaz se abrirá automáticamente en tu navegador y estará lista para usar.

### 🍎 Para usuarios de macOS / Linux
Debido a las políticas de seguridad de Apple con aplicaciones no firmadas, la ejecución se realiza desde el código fuente:
1. Descarga el repositorio haciendo clic en el botón verde **Code > Download ZIP** en la parte superior.
2. Extrae la carpeta en tus Descargas.
3. Abre la **Terminal** y asegúrate de tener instalado Python 3.
4. Instala las librerías necesarias ejecutando este comando:
   ```bash
   pip3 install eel pandas openpyxl charset-normalizer


5. Ingresa a la carpeta de la aplicación (ajusta el nombre si es distinto):

```bash
cd Downloads/Mises_Data_App-main

```

6. Inicia el programa ejecutando:
```bash
python3 app.py

```
## 🛠️ Cómo usar la aplicación

1. Navega a cualquier gráfico de investigación en [Our World in Data](https://ourworldindata.org).
2. Haz clic en la pestaña **Download** ubicada debajo del gráfico.
3. Copia el identificador técnico (código) de la métrica que necesitas.
4. Pega ese código en la barra de búsqueda de **Mises Data Intelligence** y haz clic en Descargar.
5. Selecciona tu formato de exportación preferido (**XLSX** para reportes institucionales en Excel o **CSV** para importar en otros softwares).
6. ¡Listo! Tu archivo se guardará limpio, filtrado por Hispanoamérica y con los formatos numéricos perfectos.
