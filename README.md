# 🛰️ SkyTrack: Radar Aéreo Local Personalizable

**SkyTrack** es una aplicación web ligera (Client-Side) diseñada para el seguimiento de aeronaves en tiempo real sobre puntos geográficos específicos. Utilizando la red de datos abierta de **OpenSky Network**, la aplicación calcula distancias, trayectorias y tiempos estimados de llegada (ETA) para monitorizar el tráfico aéreo que cruza la vertical de un observador.

---

## 📋 Resumen de Finalidad
La aplicación nace de la necesidad de saber con precisión **cuándo pasará un avión** por un punto concreto (como tu casa o zona de observación). Está optimizada para ser visualizada en pantallas de alta resolución (Smart TV), monitores de control o dispositivos móviles, simulando un radar profesional con estética "Dark Mode".

---

## 🛠️ Informe de Trazabilidad de Requisitos (ITR) Acumulativo

| ID | Requisito | Descripción | Versión | Estado |
| :--- | :--- | :--- | :--- | :--- |
| **RQ-01** | **Fuente de Datos** | Conexión con API gratuita OpenSky Network. | v1.0 | ✅ |
| **RQ-02** | **Interfaz Visual** | Mapa interactivo basado en Leaflet.js con estilo radar. | v1.0 | ✅ |
| **RQ-03** | **Filtrado Geo** | Captura de tráficos en un radio de ~50km del punto de estudio. | v1.0 | ✅ |
| **RQ-04** | **Input Dinámico** | Formulario para cambiar Latitud y Longitud en tiempo real. | v2.0 | ✅ |
| **RQ-05** | **Cálculo Proximidad** | Implementación de fórmula de Haversine para distancia real (km). | v2.0 | ✅ |
| **RQ-06** | **Predicción ETA** | Estimación de tiempo de llegada basada en velocidad (m/s a km/h). | v2.0 | ✅ |
| **RQ-07** | **Persistencia** | Guardado de coordenadas preferidas mediante `localStorage`. | v2.0 | ✅ |
| **RQ-08** | **Diseño CSD** | Optimización para smartphones (Mobile First) y modo WebApp. | v2.1 | ✅ |
| **RQ-09** | **Resaltado** | Identificación visual automática del avión más inminente (color amarillo). | v2.1 | ✅ |

---

## 🚀 Historial de Versiones (Changelog)

### v2.1 (Client-Side Deployment & Mobile)
* **Ajuste Responsivo:** Interfaz adaptada para smartphones con controles táctiles optimizados en la parte inferior.
* **Modo App:** Añadidas meta-etiquetas para ejecución a pantalla completa en iOS y Android (Add to Home Screen).
* **UI/UX:** El avión con menor distancia se resalta dinámicamente en la lista y en el mapa.
* **Optimización:** Refresco de datos cada 10 segundos para balancear precisión y límites de API.

### v2.0 (Interactive & Predictive)
* **Interactividad:** Inclusión de panel de configuración para cambiar coordenadas sin tocar el código.
* **Matemáticas de Vuelo:** Añadida lógica para calcular la distancia euclidiana sobre la esfera terrestre.
* **Estimación de Tiempo:** Cálculo de ETA basado en la velocidad reportada por el transpondedor.
* **Persistencia:** La aplicación recuerda tu última ubicación configurada al recargar la página.

### v1.0 (MVP - Minimum Viable Product)
* **Visual Base:** Mapa en modo oscuro (CartoDB Dark Matter).
* **Iconografía:** Representación de aviones con rotación real según su rumbo (heading).
* **Geofencing:** Delimitación de área de estudio fija en Málaga (Alhaurín de la Torre).

---

## ⚙️ Instalación y Uso
1. Copia el código del archivo `index.html`.
2. Guárdalo localmente o súbelo a un hosting estático (GitHub Pages, Netlify).
3. Abre la URL en tu navegador.
4. **En TV:** Pulsa F11 para modo pantalla completa.
5. **En Móvil:** Selecciona "Añadir a pantalla de inicio" para usar como aplicación nativa.

---
**Desarrollado con fines educativos y de observación civil.**
