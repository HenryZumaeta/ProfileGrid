# 🛰️ Grillado de Perfil Longitudinal

Automatización completa para generar grillas adaptadas a perfiles topográficos longitudinales utilizando **Model Builder en ArcGIS Pro 3.0.2**, sin necesidad de scripting.

---

## 📌 Descripción

Esta herramienta permite generar de forma automatizada una **grilla rectangular** superpuesta a perfiles longitudinales obtenidos a partir de curvas de nivel. Incluye funciones de interpolación, cálculo automático de filas, columnas, origen de grilla, etiquetado dinámico con unidades, y aplicación de simbología predefinida.

Está pensada para agilizar flujos de trabajo en proyectos de:

- Ingeniería civil
- Hidráulica e hidrología
- Topografía y catastro
- Cartografía temática

---

## 🧰 Herramienta principal

### 🔧 [`Grillado de perfil longitudinal.atbx`](https://github.com/HenryZumaeta/ProfileGrid/blob/856b8cbd7240d210309dd5d264a0cfc313d6564b/Grillado%20de%20perfil%20longitudinal.atbx)

- Desarrollada 100% con **Model Builder**
- Compatible con **ArcGIS Pro 3.0.2**

---

## 📂 Estructura del repositorio

```
ProfileGrid/
│
├── Grillado de perfil longitudinal.atbx        # Herramienta Model Builder
├── Layers/                                     # Simbología en formato .lyrx
│   └── Grillado_Perfiles.lyrx
├── shp/                                        # Datos de prueba
│   ├── 14h-curvas.shp                          # Curvas de nivel (Carta Nacional 14h)
│   └── Alineamiento.shp                        # Alineamiento de ejemplo
```

---

## 🗺️ Datos de ejemplo

Para facilitar la replicación del modelo, se incluyen:

- Curvas de nivel de la **Carta Nacional del Perú – Hoja 14h**
- Alineamiento vectorial de referencia para interpolación
- Simbología de grilla prediseñada con etiquetas y formato cartográfico

---

## ⚙️ Parámetros de entrada

- **Curvas de nivel**: shapefile lineal con campo de elevación (`Z`)
- **Alineamiento**: línea eje del perfil
- **Distancia en X / Y**: define el espaciado de la grilla (por ejemplo, `100 Meters`)
- **Sistema de coordenadas**: recomendado proyectado (UTM)
- **Simbología del grillado**: capa `.lyrx` opcional

---

## 🧠 Funcionalidades destacadas

- Cálculo automático de:
  - Número de filas y columnas
  - Coordenada de origen
- Etiquetas inteligentes (`X_grid`, `Y_grid`) con unidades ajustadas
- Aplicación automática de simbología
- Limpieza de archivos temporales (`*_eliminar`)
- Sin intervención manual intermedia

---

## 💬 Créditos

Autor: **Henry Zumaeta**  
Especialista en Ingeniería Civil e Inteligencia Artificial  
Contacto: [LinkedIn](https://www.linkedin.com/in/henryzumaeta)

---

## 📃 Licencia

Este proyecto se distribuye bajo una licencia abierta. Puedes usarlo, adaptarlo y compartirlo citando la fuente.

---

¡Gracias por visitar este repositorio! Si esta herramienta te fue útil, considera dejar una estrella ⭐ o compartir con tu red de colegas SIG.

