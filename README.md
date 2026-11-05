# 🧘 PausaActiva · Fisioterapia & Ergonomía Laboral

> Aplicación web clínica, interactiva y de respuesta ultrarrápida para la prevención de **Trastornos Musculoesqueléticos (TME)** (cervicalgia, lumbalgia, túnel carpiano y sobrecarga postural estática) en estudiantes y profesionales que pasan más de 6 horas al día sentados frente a una pantalla.

[![GitHub Pages Ready](https://img.shields.io/badge/GitHub%20Pages-Desplegado-dc2626.svg)](https://marrosas-beep.github.io/mi-aplicacion-web/)
[![Design System](https://img.shields.io/badge/Design%20System-Clinical%20Red%20Ergonomics-dc2626.svg)](DESIGN.md)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-101e19.svg)](LICENSE)
[![Audio](https://img.shields.io/badge/Web%20Audio-API%20Nativa%20D5--A5-dc2626.svg)](index.html)

---

## 📌 1. El Problema y El Perfil del Usuario

### El Problema Clínico
Hoy en día, las personas que trabajan o estudian sentadas más de 6 horas al día frente a una pantalla sufren de **Trastornos Musculoesqueléticos (TME)** como:
- **Cervicalgia y síndrome de cabeza adelantada:** Cada 2.5 cm de flexión anterior de cuello añade ~4.5 kg de carga a las vértebras C1-C7.
- **Lumbalgia postural por hiperpresión discal:** Estar sentado sin soporte dinámico incrementa la presión intradiscal en L4-L5 hasta en un 140% comparado con la bipedestación.
- **Síndrome del Túnel Carpiano y Tendinopatías:** Compresión del nervio mediano y sobrecarga en flexores/extensores por uso continuado de ratón y teclado.

La prevención suele fracasar porque los folletos o videos tradicionales son largos, pesados o carecen de **criterios biomecánicos y dosificación clínica**.

### El Usuario Objetivo
**Camilo**, 22 años, estudiante universitario de Fisioterapia y trabajador a tiempo parcial en computadora. Pasa entre 7 y 9 horas diarias sentado y experimenta rigidez continua al final de la jornada. Necesita una herramienta ágil, visual, científicamente segura y que pueda realizar en 2.5 a 3 minutos desde su puesto de trabajo.

---

## 🚀 2. Novedades y Funcionalidades Principales

### 🔴 1. Rediseño al Sistema Visual "Clinical Red"
Siguiendo las directrices ergonómicas, la interfaz ha evolucionado a una paleta **Rojo Clínico y Bio-alerta** (`#dc2626`, `#fee2e2`, `#991b1b`) sobre una superficie anti-reflejo suave (`#edfdf4`), reduciendo la fatiga ocular y destacando claramente las alertas de postura y seguridad.

### 🏃 2. Cinco Zonas Anatómicas con Ejercicios Guiados
1. **Rutina Completa:** Secuencia descompresiva integral cabeza a pies.
2. **Cuello / Cervical:** Flexión lateral asistida, retracción mentoniana (*chin tuck*) y rotación axial controlada.
3. **Hombros / Brazos:** Apertura pectoral contra síndrome cruzado, elevación/descarga escapular de Jacobson y abducción posterior.
4. **Muñecas / Manos (¡Nueva Zona!):** Elongación de flexores (túnel carpiano), estiramiento de extensores (codo de tenista/ratón), desviación ulnar asistida (tenosinovitis De Quervain) y bombeo miofascial en estrella.
5. **Espalda / Lumbar:** Báscula pélvica anteroposterior, torsión torácica en silla y extensión lumbar de pie (método McKenzie).

### 🎬 3. Ilustraciones SVG Animadas con CSS Keyframes
Cada uno de los 13 ejercicios incluye una **ilustración vectorial animada** integrada (`assets/*.svg`) con bucles fluidos (`@keyframes anim...`) para que el usuario aprenda la biomecánica correcta del movimiento **al instante sin necesidad de leer textos largos ni descargar videos pesados**.

### 📋 4. Dosificación Fisioterapéutica Explícita en Cada Tarjeta
Cada ejercicio detalla con rigor científico:
- **Series:** (ej. 2 a 3 series)
- **Repeticiones:** (ej. 1 sostenido de 30s o 10 ciclos de bombeo)
- **Tiempo Activo:** 30 segundos (activación del Órgano Tendinoso de Golgi)
- **Descanso Recomendado:** 10 a 15 segundos entre cambios articulares
- **Pauta de Respiración:** Ventilación diafragmática coordinada
- **Sensación Esperada:** Escala de tensión confortable (4/10) sin pellizcos
- **Técnica de Ejecución Paso a Paso:** 3 pasos numerados
- **Caja de Seguridad Biomecánica:** Pautas de precaución y detención inmediata ante parestesias.

### ⏱️ 5. Temporizador Circular Dinámico de 30 Segundos
- Anillo SVG interactivo con cuenta regresiva tabular.
- Código de colores: Transición a **ámbar** en los últimos 3 segundos y **destello rojo clínico** al finalizar.
- Botones ergonómicos de Iniciar/Pausar, Siguiente, Anterior y Reiniciar.
- Atajos de teclado: Barra espaciadora para Pausar/Reanudar, flechas derecha/izquierda para navegar.
- **Audio Clave Nativo:** Acorde armónico D5-A5 generado vía **Web Audio API** sin archivos de audio externos.

### 👁️ 6. Cronómetro Interactivo "Regla 20-20-20" (Descanso Ocular)
- **Indicación clínica:** Cada 20 minutos de pantalla, enfoca la mirada a 6 metros (20 pies) de distancia durante 20 segundos.
- **Cronómetro interactivo propio de 20s:** Botón de inicio, cuenta regresiva visual y señal sonora al culminar.

### 💧 7. Cronómetro y Guía de Hidratación de Discos Intervertebrales
- **Dosificación clínica:** 1 vaso (150 a 250 ml) por pausa activa. Ingesta total recomendada: **2.0 a 2.5 litros diarios** (30-35 ml/kg).
- **Advertencia de seguridad biomecánica:** Alerta explícita contra ingestas excesivas (>800 ml/hora) para prevenir sobrecarga renal e hiponatremia dilucional.
- **Cronómetro de 90 segundos:** Tiempo suficiente para ponerse de pie, caminar hacia el dispensador y reactivar la bomba muscular de los gemelos.

### 📝 8. Cuestionario Inicial Ergonómico y Calibración
- Modal inicial configurable: Nombre/Apodo, Rango de Edad, Horas frente a monitor, Nivel de Condición Física y Zona principal de molestia.
- Calibra automáticamente la rutina predeterminada y muestra un resumen en el encabezado.
- Almacenado de forma persistente y privada en `localStorage`.

### 🛡️ 9. Modal de Seguridad Clínica y Contraindicaciones
Aviso previo de criterios médicos con advertencia de consulta profesional ante:
- Parestesias (adormecimiento en manos o pies).
- Hernias discales agudas con dolor radicular lancinante.
- Inestabilidad cervical, mareos o antecedentes traumáticos recientes.

### 🔔 10. Recordatorio de Próxima Pausa e Historial con Escala EVA
- Temporizador en cuenta regresiva programable para la próxima pausa: **30, 45, 50 o 60 minutos**.
- Registro histórico de sesiones completadas en `localStorage` con fecha, minutos y evaluación de alivio en **Escala Visual Analógica (EVA 1-5)**.

### ☁️ 11. Conexión Coherente y Honesta a Firestore
- La cabecera muestra la realidad del sistema: **"Modo Local (Offline)"** de forma predeterminada.
- Al pulsar el botón, el usuario puede ingresar sus credenciales JSON de Firebase Firestore si desea sincronizar en la nube, cambiando dinámicamente a **"Firestore Conectado"** únicamente cuando los datos son válidos.

---

## 📁 3. Estructura de Archivos

```text
├── index.html            # SPA con toda la lógica clínica, UI responsiva y Web Audio API
├── DESIGN.md             # Sistema de tokens y colores Clinical Red
├── README.md             # Documentación exhaustiva técnica y biomecánica
├── assets/               # Ilustraciones vectoriales animadas con CSS Keyframes
│   ├── cervical-1.svg    # Flexión lateral de cuello
│   ├── cervical-2.svg    # Retracción mentoniana (chin tuck)
│   ├── cervical-3.svg    # Rotación axial cervical
│   ├── hombros-1.svg     # Apertura pectoral y retracción escapular
│   ├── hombros-2.svg     # Elevación y descarga de hombros (Jacobson)
│   ├── hombros-3.svg     # Abducción cruzada posterior de hombro
│   ├── manos-1.svg       # Flexores de muñeca (túnel carpiano)
│   ├── manos-2.svg       # Extensores de muñeca (codo de tenista)
│   ├── manos-3.svg       # Desviación ulnar (tenosinovitis De Quervain)
│   ├── manos-4.svg       # Bombeo miofascial y apertura en estrella
│   ├── espalda-1.svg     # Báscula pélvica anteroposterior
│   ├── espalda-2.svg     # Torsión torácica en silla ergonómica
│   └── espalda-3.svg     # Extensión lumbar de pie (McKenzie)
└── .gitignore            # Exclusiones de control de versiones
```

---

## 💻 4. Cómo Probar la Aplicación

### A. Uso Local Inmediato (Sin descargas ni instalación)
1. Abre la carpeta del proyecto en tu explorador de archivos de Windows.
2. Haz doble clic en el archivo [`index.html`](index.html).
3. Se abrirá al instante en tu navegador preferido (Chrome, Edge, Firefox, Brave).

### B. Servidor Local Ligero (Opcional)
Desde la terminal en esta carpeta:
```powershell
python -m http.server 8080
```
Y abre en tu navegador: `http://localhost:8080`

### C. Despliegue Público en GitHub Pages
La aplicación se encuentra desplegada y lista para acceso desde cualquier celular, tablet o computadora en:
👉 **[https://marrosas-beep.github.io/mi-aplicacion-web/](https://marrosas-beep.github.io/mi-aplicacion-web/)**

---

## 🏥 5. Fundamentos Fisiológicos: La Ciencia de la Pausa de 30s
- **0 a 8 segundos:** El huso neuromuscular reacciona por reflejo miotático para evitar el estiramiento.
- **12 a 20 segundos:** El **Órgano Tendinoso de Golgi (OTG)** detecta tensión sostenida e induce el reflejo de inhibición autógena.
- **20 a 30 segundos:** Se produce la elongación plástica del sarcomero y rehidratación de la matriz extracelular sin riesgo lesivo.

---

## 🗄️ 6. Guía Rápida: Cómo Conectar Firebase Firestore Paso a Paso

Si deseas que la app sincronice tus pausas activas en la nube (para que un docente, supervisor o fisioterapeuta las consulte en tiempo real):

1. **Crear proyecto gratuito en Firebase:**
   - Entra a [console.firebase.google.com](https://console.firebase.google.com/) con tu cuenta Google.
   - Haz clic en **"Crear un proyecto"** (o "Agregar proyecto"), asígnale un nombre (ej. `PausaActiva`) y finaliza el asistente.
2. **Crear la Base de Datos Cloud Firestore:**
   - En el menú lateral izquierdo, ve a **Compilación &gt; Firestore Database**.
   - Haz clic en **"Crear base de datos"**.
   - Selecciona **"Iniciar en modo de prueba"** (permite leer y escribir sin autenticación obligatoria) y pulsa Siguiente.
3. **Obtener las Credenciales:**
   - En el panel de Firebase, haz clic en el engranaje ⚙️ (arriba a la izquierda) &gt; **Configuración del proyecto**.
   - En la pestaña **General**, baja hasta **"Tus apps"** y haz clic en el ícono Web **`</>`**.
   - Asigna un apodo a la app y verás un bloque de código similar a este:
     ```javascript
     const firebaseConfig = {
       apiKey: "AIzaSy...",
       authDomain: "tu-proyecto.firebaseapp.com",
       projectId: "tu-proyecto",
       storageBucket: "tu-proyecto.appspot.com",
       messagingSenderId: "123456789",
       appId: "1:12345:web:abcdef"
     };
     ```
4. **Conectar en la Aplicación:**
   - En **PausaActiva**, pulsa el botón de la cabecera **"Modo Local (Offline)"**.
   - Pega ese bloque de código tal cual en el cuadro de texto.
   - Haz clic en **"Conectar Firestore"**.
   - Verás la confirmación inmediata y la cabecera pasará a **"Firestore Conectado"** (con luz verde). A partir de ese momento, cada pausa completada se guardará en tu base de datos en la colección `historial_pausas`.

---

## 📄 Créditos y Licencia
Desarrollado como proyecto clínico y ergonómico interactivo.  
Repositorio oficial: [marrosas-beep/mi-aplicacion-web](https://github.com/marrosas-beep/mi-aplicacion-web).  
Licencia MIT.
