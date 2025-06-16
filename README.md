# 🗺️ Geolocalización de Direcciones en Valledupar, Colombia

Este repositorio contiene una serie de herramientas en Python para geolocalizar direcciones comerciales en Valledupar (Cesar, Colombia), agruparlas por cercanía geográfica y visualizar los resultados sobre mapas interactivos.

---

## 📌 Objetivo

Facilitar el análisis espacial de direcciones comerciales mediante:

- Geolocalización automática usando la API de Google Maps.
- Agrupación de puntos mediante **clustering jerárquico** (Agglomerative Clustering).
- Visualización de resultados en mapas interactivos con **Folium**.
- Generación de archivos Excel por grupo para distribución operativa.

---

## ⚙️ Requisitos

- Python 3.8+
- Cuenta de Google con acceso a la API de Geocoding.
- Datos en formato `.csv` o `.xlsx` con columnas de direcciones.

---

## 📦 Librerías necesarias

```bash
pip install pandas scikit-learn numpy folium openpyxl requests
```

---

## 🧭 Estructura del Proyecto


| Archivo / Carpeta                   | Descripción                                                                          |
| ----------------------------------- | ------------------------------------------------------------------------------------ |
| `geolocalizacion_google_maps.ipynb` | Extrae coordenadas (latitud y longitud) de direcciones usando la API de Google Maps. |
| `clusterizacion_direcciones.ipynb`  | Agrupa las direcciones por proximidad usando clustering jerárquico y genera mapas.   |
| `dividir_por_pareja.py`             | Genera archivos Excel separados para cada grupo asignado.                            |
| `DIRECCIONES.csv`                   | Archivo de entrada con direcciones a geolocalizar (no incluido por privacidad).      |

---

## 🧪 Ejecución

1. Geolocalización:
Ejecuta geolocalizacion_google_maps.ipynb para obtener las coordenadas de tus direcciones.
2. Clustering:
Usa clusterizacion_direcciones.ipynb para agrupar direcciones por cercanía y visualizar los grupos en un mapa.
3. Exportación por grupo:
Ejecuta dividir_por_pareja.py para generar un archivo por cada grupo creado.

---

## 📍 Consideraciones
Las direcciones deben estar localizadas en Valledupar, Cesar, Colombia.

Se recomienda usar direcciones verificadas de bases como Cámara de Comercio.

La API de Google tiene límites gratuitos diarios. Se aplica una espera de 1 segundo entre llamadas para evitar bloqueos.

---

## 📊 Visualización
El script genera mapas interactivos en Jupyter Notebook, donde cada grupo se representa con un color distinto para facilitar la interpretación geográfica de los resultados.

---

## 💡 Uso Sugerido
Este proyecto puede ser utilizado para:

* Optimizar rutas de visitas o inspecciones.

* Organizar operativos de control territorial.

* Apoyar análisis de concentración de comercio o informalidad.

---

## 👩‍💻 Autor
Katheryn Sofía Oviedo Castañeda
Contadora Pública | MSc. en Analítica Aplicada | Apasionada por el análisis geoespacial y la automatización de procesos públicos

---

### 📄 Licencia
Uso interno o académico. No usar con fines comerciales sin autorización previa.

---
