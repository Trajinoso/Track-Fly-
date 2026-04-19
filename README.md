# 🛰️ SkyTrack: Radar Aéreo Local (Security Edition)

**SkyTrack** es una aplicación web (Client-Side) para el seguimiento de aeronaves en tiempo real. Calcula distancias y tiempos de llegada (ETA) para monitorizar el tráfico aéreo sobre coordenadas personalizables.

## 📋 Resumen de Finalidad
Optimizado para Smart TV y dispositivos móviles. Permite vigilancia aérea con estética de radar profesional y protección de privacidad para el usuario.

---

## 🛠️ Informe de Trazabilidad de Requisitos (ITR) Acumulativo

| ID | Requisito | Versión | Estado |
| :--- | :--- | :--- | :--- |
| **RQ-01** | Fuente de Datos (API OpenSky) | v1.0 | ✅ |
| **RQ-02** | Mapa Interactivo (Leaflet Dark) | v1.0 | ✅ |
| **RQ-03** | Input de Coordenadas Dinámico | v2.0 | ✅ |
| **RQ-04** | Cálculo de Distancia (Haversine) | v2.0 | ✅ |
| **RQ-05** | Estimación de Tiempo de Llegada (ETA) | v2.0 | ✅ |
| **RQ-06** | Persistencia en LocalStorage | v2.0 | ✅ |
| **RQ-07** | Diseño Responsivo para Smartphones | v2.1 | ✅ |
| **RQ-08** | **Privacidad: Credenciales vía Prompt** | v2.3 | ✅ |
| **RQ-09** | **Seguridad: Ofuscación Base64 de cabeceras**| v2.3 | ✅ |
| **RQ-10** | **Prevención de Bloqueos (Rate Limit Info)** | v2.3 | ✅ |

---

## 🚀 Historial de Versiones (Changelog)

### v2.3 (Security & Privacy Update)
* **Protección de Datos:** Se elimina la necesidad de escribir contraseñas en el código fuente. El sistema solicita las credenciales al abrir la web y las guarda de forma local y cifrada en el navegador.
* **Cierre de Sesión:** Botón para borrar credenciales del dispositivo.
* **Depuración:** Mensajes en pantalla cuando la API de OpenSky está saturada (Error 429).
* **Frecuencia:** Ajuste de refresco a 15s para maximizar la duración del cupo de datos.

### v2.1 (Mobile Ready)
* Adaptación de paneles para pantallas táctiles verticales.
* Soporte para "Añadir a pantalla de inicio" como WebApp.

### v2.0 (Predictive)
* Introducción de cálculos matemáticos para distancia y tiempo estimado (ETA).
* Sistema de resaltado en amarillo para el tráfico más inminente.

### v1.0 (MVP)
* Estructura base de radar y conexión inicial.

---

## ⚙️ Despliegue Seguro
Este código es seguro para ser **Público** en GitHub porque no contiene tus claves.
1. Sube el código a GitHub.
2. Abre tu URL de GitHub Pages.
3. Introduce tu usuario/pass de OpenSky cuando se te solicite (se guardará solo en ese dispositivo).

