# ElevationsRegister

**Registrador experimental de inclinaciones longitudinales y laterales mediante los sensores de orientación de un teléfono móvil.**

ElevationsRegister es una herramienta web experimental desarrollada para registrar variaciones de inclinación durante recorridos, utilizando los sensores de orientación disponibles en dispositivos móviles.

El proyecto está pensado principalmente como una herramienta de exploración y levantamiento de datos para recorridos, permitiendo registrar información temporal, marcar eventos asociados a estaciones y posteriormente exportar los datos para su análisis y visualización.

> ⚠️ **Proyecto experimental:** los datos obtenidos mediante sensores de teléfonos móviles dependen del dispositivo, sistema operativo, calibración, condiciones de uso y calidad de los sensores. Los resultados no deben considerarse mediciones topográficas o ferroviarias de precisión.

---

## 📌 Características

- 📱 Registro mediante sensores de orientación del teléfono.
- 📐 Medición de inclinación longitudinal.
- ↔️ Medición de inclinación lateral.
- 🎯 Calibración del dispositivo antes de comenzar un levantamiento.
- ⏱️ Registro periódico mediante un intervalo configurable.
- 🚉 Marcado manual de eventos durante el recorrido.
- 🟡 Registro de eventos de **ARRIVAL** y **DEPARTURE**.
- 🏷️ Identificación opcional de estaciones.
- 📊 Contador de muestras registradas.
- ⏲️ Registro de tiempo transcurrido desde el inicio.
- 💾 Exportación de los datos a CSV.
- 🌐 Funcionamiento directamente desde el navegador.
- 📲 Compatible con el desarrollo como Progressive Web App (PWA).
- 🖥️ No requiere instalación de software especializado para realizar las pruebas.
- 🔓 Código abierto para experimentación y adaptación.

---

# 🎯 Objetivo

El objetivo de InclinationRegister es explorar la posibilidad de utilizar los sensores disponibles en teléfonos móviles como una herramienta de levantamiento preliminar para estudiar la inclinación de un recorrido.

El proyecto surge a partir de la necesidad de registrar cambios de orientación durante un desplazamiento, manteniendo asociados los datos de inclinación con una referencia temporal.

En el contexto ferroviario, esto permite posteriormente estudiar:

- cambios de pendiente;
- variaciones de inclinación;
- comportamiento del recorrido;
- diferencias entre distintos sectores;
- relación entre inclinación y ubicación temporal;
- identificación de zonas asociadas a estaciones;
- generación de perfiles longitudinales a partir de los datos registrados.

---

# 🧭 Principio de funcionamiento

El teléfono registra información de orientación utilizando los sensores disponibles en el dispositivo.

Durante la calibración se establece una referencia inicial:

```text
Orientación inicial
       ↓
   Calibración
       ↓
Referencia base
       ↓
Medición durante recorrido
       ↓
Diferencia respecto a la referencia
       ↓
Inclinación registrada
