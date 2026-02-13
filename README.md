# 🗺️ Mapa Interactivo: Análisis de Internet en Colombia

Este proyecto es una herramienta de visualización geoespacial diseñada para analizar la cobertura y el tamaño de las empresas proveedoras de internet a nivel municipal en Colombia. Utiliza datos exportados desde QGIS y una capa de personalización avanzada mediante JavaScript y Python.

## 🚀 Características Principales

* **Filtros Dinámicos:** Permite filtrar municipios según el tamaño de la empresa líder (Gigante, Muy Grande, Grande, Mediana, Pequeña, Micro).
* **Conteo en Tiempo Real:** Un indicador muestra cuántos municipios cumplen con los criterios seleccionados actualmente.
* **Diseño Responsive:** Optimizado para su visualización en computadoras de escritorio y dispositivos móviles.
* **Panel Colapsable:** Interfaz limpia que permite ocultar los controles para priorizar la exploración del mapa.
* **Popups Enriquecidos:** Ventanas emergentes con información detallada, tablas de datos y diseño adaptativo.
* **Optimización de Capas:** Sistema "Anti-Fantasmas" que desactiva la interacción de elementos ocultos para una navegación fluida.

## 🛠️ Tecnologías Utilizadas

* **[Leaflet.js](https://leafletjs.com/):** Biblioteca principal para mapas interactivos.
* **QGIS:** Para el procesamiento de datos geoespaciales y exportación inicial.
* **Python:** Script automatizado para la limpieza de código e inyección de funcionalidades avanzadas.
* **HTML5/CSS3/JS:** Para la interfaz de usuario y la lógica de filtrado.
* **GitHub Pages:** Hosting del mapa en línea.

## ⚙️ Cómo Actualizar el Mapa

Si realizas cambios en QGIS y necesitas actualizar el sitio:

1.  Exporta tu proyecto desde QGIS usando el plugin `qgis2web` (formato Leaflet).
2.  Ejecuta el script de Python `mapa_colombia_pro.py` incluido en este repositorio.
3.  Selecciona el archivo `index.html` generado por QGIS.
4.  El script moverá automáticamente los archivos a la carpeta del repositorio y aplicará todas las mejoras (filtros, responsive, estilos).
5.  Realiza un `git push` a la rama `main`.

## 📂 Estructura del Repositorio

* `/data`: Contiene los archivos GeoJSON de los municipios.
* `/css`: Estilos originales de Leaflet y QGIS.
* `/js`: Lógica de renderizado y complementos.
* `index.html`: El archivo principal del mapa (procesado por el script).
* `mapa_colombia_pro.py`: Script de automatización y post-procesamiento.

![Vista previa del mapa](screenshot_1.png)


## 💻 Comandos de Git (Guía Rápida)

Si necesitas gestionar los archivos entre tu PC y GitHub, estos son los comandos esenciales:

### 1. Traer cambios desde GitHub al local (Descargar)
Si hiciste cambios directamente en la web de GitHub o alguien más subió archivos:
```bash
git pull origin main

Subir cambios del local a GitHub (Publicar)
Después de ejecutar el script de Python y verificar que todo está bien:

# Añadir todos los cambios al área de preparación
git add .

# Crear el paquete con un mensaje descriptivo
git commit -m "Mejora: Popups responsive y botón de filtros"

# Subir a la nube
git push origin main

3. Otros comandos útiles
git status: Ver qué archivos han cambiado.

git clone [URL]: Descargar el repositorio completo por primera vez.

---

### ¿Cómo actualizar tu local ahora mismo?

1.  Abre tu terminal o consola en la carpeta del proyecto.
2.  Escribe: `git pull origin main`.
3.  ¡Listo! Ya tienes en tu PC lo que subiste a GitHub.
---
Generado con ❤️ para el análisis de conectividad en Colombia.
