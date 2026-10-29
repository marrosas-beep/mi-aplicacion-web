# 🧘 PausaActiva · Fisioterapia & Ergonomía Laboral

> Aplicación web clínica, interactiva y de respuesta ultrarrápida para la prevención de **Trastornos Musculoesqueléticos (TME)** (cervicalgia, lumbalgia y sobrecarga postural) en estudiantes y profesionales que pasan más de 6 horas al día sentados frente a una pantalla.

[![GitHub license](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![GitHub Pages Ready](https://img.shields.io/badge/GitHub%20Pages-Ready-success.svg)](https://marrosas-beep.github.io/mi-aplicacion-web/)
[![Design System](https://img.shields.io/badge/Design%20System-Clinical%20Ergonomic%20Pause-00664b.svg)](DESIGN.md)

---

## 📌 1. El Problema y El Usuario

### El Problema
Las personas que estudian o trabajan sentadas más de 6 a 9 horas diarias frente a un monitor sufren de sobrecarga postural estática. Las pausas activas convencionales suelen fracasar porque las rutinas en video o papel son excesivamente largas, complejas de memorizar o carecen de dosificación clínica adecuada, provocando fatiga y dolor crónico en cuello y columna.

### El Usuario Objetivo
**Camilo**, 22 años, estudiante universitario de Fisioterapia y trabajador a tiempo parcial en computadora. Pasa entre 7 y 9 horas diarias sentado y experimenta rigidez continua al final de la jornada. Necesita una guía rápida, científicamente dosificada y segura que pueda realizar sin abandonar su puesto de trabajo.

---

## 🚀 2. Las 4 Funciones Implementadas

| # | Función del PRD | Implementación Técnica en la App |
|---|-----------------|-----------------------------------|
| **1** | **Filtrar por Zona Anatómica** | 4 botones de selección rápida: **Rutina Completa**, **Cuello / Cervical**, **Hombros / Brazos** y **Espalda / Lumbar**. Actualización instantánea del diagnóstico fisiopatológico, músculos diana y lista de ejercicios sin recargar la página. |
| **2** | **Tarjeta con Criterio Fisioterapéutico** | Ficha clínica completa con título, músculos objetivo, técnica paso a paso numerada y caja destacada de **"Recomendación Fisioterapéutica y Seguridad Biomecánica"** para prevenir sobreesfuerzos o parestesias. |
| **3** | **Temporizador Dinámico de 30s** | Cuenta regresiva exacta de 30 segundos con anillo SVG circular animado, cifras tabulares y botones táctiles ergonómicos: **Iniciar / Pausar**, **Siguiente**, **Anterior** y **Reiniciar**. Atajos de teclado (Espacio, Flechas). |
| **4** | **Notificaciones y Progreso** | Alerta visual (anillo ámbar los últimos 3s + destello verde al finalizar), alerta auditiva nativa con **Web Audio API** (campana armónica relajante D5-A5 sin archivos pesados) y barra de avance de la rutina (*"Ejercicio 2 de 4"*). |

---

## 🔬 3. Fundamento Biomecánico: ¿Por qué 30 segundos?

La duración de **30 segundos** por ejercicio no es arbitraria:
- Durante los primeros **6 a 10 segundos** de estiramiento estático, los husos neuromusculares disparan el reflejo miotático (contracción refleja defensiva).
- Entre los **15 y 20 segundos**, el **Órgano Tendinoso de Golgi (OTG)** activa el *reflejo de inhibición autógena*.
- A los **30 segundos**, el tejido muscular y las fascias se relajan y elongan de forma segura sin microdesgarros.

---

## 🎨 4. Sistema de Diseño (Design System)

Basado en la especificación [DESIGN.md](DESIGN.md):
- **Paleta Cromática Terapéutica:**
  - Primario Salvia / Esmeralda (`#00664b` y `#2a7f62`): Confianza clínica y confirmación de progreso.
  - Secundario Azul Sereno (`#386286`): Estabilidad articular y descanso cognitivo.
  - Ámbar Biomecánico (`#ac5d00` y `#ffdcc3`): Señalizador de precaución física y límites de rango articular.
  - Superficie Menta Ultraligera (`#edfdf4`): Elimina el deslumbramiento ocular de monitores convencionales.
- **Tipografía:** *Plus Jakarta Sans* (humanista, accesible y con cifras numéricas tabulares para el temporizador).
- **Iconografía:** *Material Symbols Outlined* de Google.

---

## 📁 5. Estructura del Proyecto

```text
├── index.html       # Aplicación Single Page (HTML5, Tailwind CSS, JS modular y Web Audio)
├── DESIGN.md        # Tokens de diseño, sistema de espaciado, elevaciones y paleta
├── screen.png       # Captura de referencia del prototipo ergonómico
├── README.md        # Documentación técnica y clínica
└── .gitignore       # Exclusiones estándar de desarrollo
```

---

## 💻 6. Cómo Ejecutar en Local

Puedes probar la aplicación de dos formas muy sencillas:

### Opción A (Sin dependencias, doble clic directo):
1. Abre tu explorador de archivos en la carpeta del proyecto.
2. Haz doble clic en [`index.html`](index.html). Se abrirá de inmediato en tu navegador habitual (Chrome, Edge, Firefox, Safari).

### Opción B (Servidor local ligero):
Si tienes Python o Node instalado:
```bash
# Con Python
python -m http.server 8080

# Luego ingresa en tu navegador a:
# http://localhost:8080
```

---

## 🌐 7. Despliegue en GitHub Pages

Para publicar tu aplicación web y tener un enlace público gratuito accesible desde cualquier computadora o celular:

1. Ve a tu repositorio en GitHub: **[github.com/marrosas-beep/mi-aplicacion-web](https://github.com/marrosas-beep/mi-aplicacion-web)**.
2. Haz clic en la pestaña **Settings** (Configuración).
3. En el menú lateral izquierdo, haz clic en **Pages**.
4. En **Build and deployment > Source**, selecciona: **Deploy from a branch**.
5. En **Branch**, selecciona `main` y la carpeta `/(root)`.
6. Haz clic en **Save**.
7. En 1-2 minutos, tu aplicación estará disponible públicamente en:
   👉 **`https://marrosas-beep.github.io/mi-aplicacion-web/`**

---

## 🗄️ 8. Módulo Firebase Firestore (Listo para Conectar)

La aplicación ya cuenta con un conector interactivo para Firebase Firestore:
- En la cabecera verás el botón **"Firestore Listo"**.
- Al hacer clic, se abre una ventana donde puedes ingresar las credenciales de tu proyecto de Firebase (`apiKey`, `projectId`, etc.).
- Permite registrar el historial de pausas activas completadas, métricas ergonómicas y preguntas/feedback del usuario cuando desees activarlo.

---

## 📄 Licencia y Créditos
Desarrollado para la electiva de salud, ergonomía y desarrollo web.
Repositorio oficial: [marrosas-beep/mi-aplicacion-web](https://github.com/marrosas-beep/mi-aplicacion-web).
