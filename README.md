# 🧮 SmartDifferentialCalc

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Flask](https://img.shields.io/badge/flask-2.0+-lightgrey.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

# SmartDifferentialCalc

**Calculadora avanzada para el análisis y resolución de Ecuaciones Diferenciales Ordinarias (EDO).**

SmartDifferentialCalc es una herramienta moderna diseñada para interpretar, procesar y resolver EDO de forma clara, estructurada y precisa. Su enfoque está orientado a facilitar el trabajo académico y técnico, permitiendo analizar soluciones, verificar resultados y explorar distintos métodos de resolución dentro de un entorno unificado.


[Demo](#-demo) • [Instalación](#-instalación-rápida) • [Uso](#-cómo-usarlo) • [Contribuir](#-contribuciones)

</div>

---

## 📖 ¿Qué es esto?

**SmartDifferentialCalc** es una aplicación web que resuelve ecuaciones diferenciales ordinarias (EDO) y, lo más importante, **te explica cómo lo hizo**, paso a paso, en español claro y sencillo.

A diferencia de otras calculadoras que te dan solo un resultado frío y sin contexto, SmartDifferentialCalc usa **inteligencia artificial** (DeepSeek) para generar explicaciones pedagógicas que realmente te ayudan a **entender** el proceso.

### 🎯 ¿Por qué existe este proyecto?

Este proyecto nació en 2025 como iniciativa académica dentro de la **asignatura de Ecuaciones Diferenciales** del programa de **Ingeniería de Software – FESC (Fundación de Estudios Superiores Comfanorte)**, en Cúcuta, Colombia.

La idea surgió de una necesidad muy puntual: presentar un proyecto que no fuera *“otro programa más en Python con Tkinter y gráficas básicas”*. Queríamos algo distinto, más actualizado, visualmente atractivo y alineado con el boom tecnológico del momento.

Al explorar calculadoras en línea, encontramos un problema común:

> *Mostraban únicamente la respuesta final o procedimientos tan técnicos que necesitabas otra calculadora para entenderlos.*

A partir de eso establecimos los objetivos:

- ✅ Resolver EDO de distintos tipos  
- ✅ Mostrar pasos claros y entendibles, como lo explicaría un buen profesor  
- ✅ Ser completamente gratuito y en español  
- ✅ Ofrecer una interfaz moderna, limpia y cómoda de usar  
- ✅ Basarse en tecnologías actuales mediante una API capaz de analizar, clasificar y procesar ecuaciones
  
Y así nació **SmartDifferentialCalc** 🚀 que en esencia, SmartDifferentialCalc está para convertir las EDO en algo más comprensible, usable y cercano a los estudiantes que realmente necesitan entenderlas.

---
## 📚 Documentación adicional

Si deseas consultar el documento completo donde se detalla el contexto, la investigación académica, la justificación, el planteamiento del problema, los objetivos, el propósito y el alcance del proyecto, puedes acceder aquí:

🔗 **Documento completo en Google Drive:**  
https://docs.google.com/document/d/11Y8t4TAVEoJalshx7t86nw62IlrW79wJ7IQaEVtRl0w/edit?tab=t.0

En este archivo encontrarás toda la fundamentación teórica y descriptiva del prototipo, incluyendo el resumen, la introducción, los objetivos, el marco conceptual y la explicación extendida del desarrollo técnico.

---

## ✨ Características principales

| Característica | Descripción |
|----------------|-------------|
| 🤖 **IA Integrada** | Usa DeepSeek para generar explicaciones detalladas en lenguaje natural |
| 📝 **Paso a paso** | No solo te da la respuesta, te enseña cómo llegar a ella |
| 🎨 **Interfaz intuitiva** | Teclado matemático virtual + campo de texto para ecuaciones |
| 🔒 **Seguro** | Tu API key nunca se expone al navegador, Flask actúa como proxy |
| 🇪🇸 **100% en español** | Toda la interfaz y explicaciones en tu idioma |
| ⚡ **Rápido** | Resultados en segundos, sin complicaciones |
| 📚 **Educativo** | Diseñado para estudiantes, profesores e ingenieros |

---

## 🎬 Demo

### Ejemplo de uso:

**Entrada:**
```
dy/dx = 2x
```

**Salida (resumen):**
```
📋 ECUACIÓN DIFERENCIAL ORDINARIA
dy/dx = 2x

🔍 ANÁLISIS:
- Tipo: Ecuación diferencial de primer orden
- Variables: y (dependiente), x (independiente)
- Método recomendado: Separación de variables

📐 SOLUCIÓN PASO A PASO:

Paso 1: Separar variables
dy = 2x dx

Paso 2: Integrar ambos lados
∫dy = ∫2x dx
y = x² + C

✅ SOLUCIÓN GENERAL:
y = x² + C (donde C es una constante de integración)
```

*(Este es un ejemplo simplificado. La IA genera explicaciones mucho más detalladas)*

---

## 🚀 Instalación rápida

### Requisitos previos

- Python 3.8 o superior
- Una cuenta en [DeepSeek](https://platform.deepseek.com/) (para obtener tu API key)
- Git instalado en tu sistema

### Paso 1: Clonar el repositorio

```bash
git clone https://github.com/Erickpe8/SmartDifferentialCalc.git
cd SmartDifferentialCalc
```

### Paso 2: Crear entorno virtual

**En Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**En Linux/Mac:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### Paso 3: Instalar dependencias

```bash
pip install -r requirements.txt
```

### Paso 4: Configurar variables de entorno

Crea un archivo `.env` en la raíz del proyecto con el siguiente contenido:

```env
DEEPSEEK_API_KEY=tu_clave_api_aqui
DEEPSEEK_API_URL=https://api.deepseek.com/v1/chat/completions
```

> **💡 Tip:** Para obtener tu API key, regístrate en [DeepSeek Platform](https://platform.deepseek.com/) y genera una nueva clave en tu dashboard.

### Paso 5: ¡Ejecutar!

```bash
python app.py
```

Abre tu navegador y ve a: **http://localhost:5000**

¡Listo! 🎉

---

## 🎮 Cómo usarlo

### Opción 1: Escribir directamente

1. Escribe tu ecuación en el campo de texto (ejemplo: `dy/dx + y = e^x`)
2. Haz clic en **"Calcular ecuación"**
3. Espera unos segundos mientras la IA trabaja
4. ¡Mira la solución detallada!

### Opción 2: Usar el teclado virtual

La interfaz incluye un teclado matemático con:
- **Funciones:** sin(, cos(, tan(, log(, exp(, sqrt(
- **Derivadas:** d/dx(, d/dy(
- **Variables:** x, y, t
- **Operadores:** +, -, *, /, ^
- **Constantes:** e, π
- **Números:** 0-9, punto decimal

Solo haz clic en los botones para construir tu ecuación y luego presiona **"Calcular ecuación"**.

### Ejemplos de ecuaciones que puedes resolver:

| Tipo | Ejemplo |
|------|---------|
| **Primer orden separable** | `dy/dx = 2x` |
| **Primer orden lineal** | `dy/dx + y = e^x` |
| **Homogénea** | `dy/dx = (x + y) / x` |
| **Bernoulli** | `dy/dx + y = y^2 * x` |

> **⚠️ Nota:** Actualmente el sistema está optimizado para EDO de primer orden. Las derivadas de orden superior (d²y/dx²) están en desarrollo.

---

## 🏗️ Arquitectura del proyecto

```
SmartDifferentialCalc/
│
├── app.py                    # Backend Flask (núcleo del sistema)
├── requirements.txt          # Dependencias Python
├── .env                      # Variables de entorno (NO subir a Git)
├── .gitignore               
│
├── templates/
│   └── index.html           # Interfaz principal
│
├── static/
│   ├── css/
│   │   └── style.css        # Estilos de la interfaz
│   └── js/
│       └── main.js          # Lógica del cliente
│
└── README.md                # Este archivo
```

### 🔄 Flujo de trabajo

```
[Usuario escribe ecuación]
         ↓
[JavaScript valida entrada]
         ↓
[Envía POST a /solve_ode]
         ↓
[Flask recibe y valida]
         ↓
[Flask construye prompt educativo]
         ↓
[Envía a DeepSeek API]
         ↓
[DeepSeek procesa y explica]
         ↓
[Flask recibe respuesta]
         ↓
[JavaScript muestra resultado]
```

---

## 🛠️ Tecnologías utilizadas

### Backend
- **Flask** - Framework web minimalista de Python
- **python-dotenv** - Manejo seguro de variables de entorno
- **requests** - Cliente HTTP para conectar con DeepSeek

### Frontend
- **HTML5** - Estructura semántica
- **CSS3** - Diseño responsivo y moderno
- **JavaScript (Vanilla)** - Sin frameworks innecesarios, puro y ligero

### IA
- **DeepSeek API** - Motor de procesamiento simbólico y explicaciones

### Extras
- **SymPy** (opcional) - Validación simbólica adicional

---

## 🧠 Decisiones de diseño

### ¿Por qué Flask y no Django/FastAPI?

Flask es perfecto para este proyecto porque:
- ✅ Solo tenemos una ruta principal (`/solve_ode`)
- ✅ No necesitamos ORM, base de datos ni autenticación compleja
- ✅ Es fácil de entender para estudiantes
- ✅ Se ejecuta en segundos

### ¿Por qué DeepSeek y no otro modelo?

- **Costo-beneficio:** DeepSeek es más económico que GPT-4
- **Matemáticas:** Tiene buen desempeño en razonamiento matemático
- **Español:** Genera explicaciones coherentes en nuestro idioma
- **Velocidad:** Respuestas rápidas sin sacrificar calidad

### ¿Por qué no usar solo SymPy?

**SymPy resuelve, pero no explica.**

Si solo quisiéramos la respuesta, SymPy bastaría. Pero nuestro objetivo es **educativo**: queremos que entiendas el proceso. La IA genera explicaciones naturales, paso a paso, como lo haría un tutor humano.

---

## 🔐 Seguridad

Este proyecto toma en serio la seguridad:

| Riesgo | Mitigación |
|--------|-----------|
| **Exposición de API key** | Clave almacenada en `.env`, nunca en el código |
| **Inputs maliciosos** | Validación en cliente (JS) y servidor (Flask) |
| **Man-in-the-middle** | DeepSeek usa HTTPS/TLS |
| **Errores informativos** | Mensajes genéricos al usuario, logs detallados en servidor |

> **🔒 Importante:** Nunca subas tu archivo `.env` a Git. Ya está en `.gitignore` por defecto.

---

## 📝 Componentes del sistema

### Jerarquía DOM

```
container-app
 ├── app-calculator
 │    ├── calculator-container-input-user
 │    │     ├── equationInput (textarea)
 │    │     ├── calculatorButtons (36 botones)
 │    │     ├── solveButton
 │    │     ├── loading
 │    │     └── error
 │    └── solution-calculator-container-output
 │          └── solutionOutput (pre)
```

### Componentes principales

| Componente | Archivo | Responsabilidades |
|-----------|---------|------------------|
| Backend Flask | `app.py` | Routing, validación, proxy API |
| Interfaz web | `index.html` | Estructura UI |
| Lógica cliente | `main.js` | Eventos, fetch API |
| Estilos | `style.css` | Layout, cuadrícula, responsividad |
| Entorno | `.env` | Claves seguras |

---

## ⚠️ Limitaciones conocidas

Como es un **prototipo educativo**, actualmente:

- ❌ Solo resuelve una ecuación a la vez
- ❌ No grafica las soluciones
- ❌ No soporta derivadas de segundo orden (d²y/dx²) todavía
- ❌ No guarda historial de ecuaciones resueltas
- ❌ Dependencia total de la API de DeepSeek (si cae, caemos)
- ❌ Sin streaming (la respuesta se bloquea hasta completarse)

---

## 🐛 Problemas comunes (Troubleshooting)

### "ModuleNotFoundError: No module named 'flask'"

**Solución:** Asegúrate de haber activado el entorno virtual e instalado las dependencias:
```bash
pip install -r requirements.txt
```

### "Error: API key inválida"

**Solución:** Verifica que tu `.env` tenga la clave correcta:
```env
DEEPSEEK_API_KEY=sk-xxxxxxxxxxxxxxxx
```

### "La aplicación no carga en localhost:5000"

**Posibles causas:**
1. El puerto 5000 está ocupado → Cambia el puerto en `app.py`:
   ```python
   app.run(debug=True, port=8080)
   ```
2. Firewall bloqueando → Agrega excepción para Python

### "La IA tarda mucho en responder"

**Causas normales:**
- Ecuaciones complejas requieren más procesamiento
- Latencia de red con DeepSeek API
- Uso intensivo de la API (límites de rate)

**Solución:** Paciencia 😊 o considera usar un plan de pago en DeepSeek.

---

## 🤝 Contribuciones

¡Nos encantaría tu ayuda! Este es un proyecto de código abierto y **todas las contribuciones son bienvenidas**.

### Cómo contribuir:

1. **Fork** este repositorio
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`)
3. Haz tus cambios y **commitea** (`git commit -m 'Agrega nueva funcionalidad'`)
4. **Push** a tu rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un **Pull Request**

### Áreas donde necesitamos ayuda:

- 🎨 Mejorar el diseño UI/UX
- 🐍 Optimizar el código Python
- 📊 Agregar graficación de soluciones
- 🧪 Escribir tests unitarios
- 📝 Mejorar la documentación
- 🌍 Agregar soporte para más idiomas

---

## 👥 Equipo

Este proyecto fue desarrollado con ❤️ por estudiantes de **Ingeniería de Software** en FESC, Cúcuta:

| Nombre | GitHub | Rol |
|--------|--------|-----|
| **Daniel Alejandro Arevalo Güecha** | [@Akarviii](https://github.com/Akarviii) | Backend & API Integration |
| **Erick Sebastián Pérez Carvajal** | [@Erickpe8](https://github.com/Erickpe8) | Frontend & Testing |
| **Wilson Elías Carreño Morantes** | - | Documentation & Research |
| **Cristian Andrés Dávila Sánchez** | - | Documentation & Research |

---

## 📄 Licencia

Este proyecto está bajo la licencia **MIT** - consulta el archivo [LICENSE](LICENSE) para más detalles.

En resumen: puedes usar, modificar y distribuir este código libremente, incluso para proyectos comerciales, siempre que incluyas la licencia original.

---

## 🙏 Agradecimientos


Este proyecto fue posible gracias al trabajo conjunto del equipo conformado por **Daniel Alejandro Arevalo Güecha**, **Erick Sebastián Pérez Carvajal**, **Wilson Elías Carreño Morantes** y **Cristian Andrés Dávila Sánchez**, quienes aportaron en áreas como backend, integración de API, frontend, testing, documentación y análisis.

Asimismo, extendemos un agradecimiento especial al docente **M.C.s. Giovanny Barbosa Casanova**, quien impartió la asignatura de Ecuaciones Diferenciales y brindó la guía necesaria para orientar el desarrollo de esta calculadora.


---

## ❓ Dudas y contacto

Si estás interesado en conocer más a fondo este proyecto, entender su funcionamiento, revisar el proceso de instalación o simplemente resolver alguna duda, puedes contactarme sin problema. Mis redes sociales están disponibles en mi perfil de GitHub, o si prefieres, puedes escribirme directamente al correo:

📧 **ericksperezc@gmail.com**

También puedes encontrarme en:

- 🎥 **YouTube:** https://www.youtube.com/@ErickPerez_8  
- 📸 **Instagram:** https://www.instagram.com/erickperez_8/

Además, el repositorio cuenta con espacios habilitados para soporte y participación de la comunidad:

## 📞 Contacto y soporte del proyecto

- 🐛 **Reportar errores (Issues):**  
  https://github.com/Erickpe8/SmartDifferentialCalc/issues

- 💬 **Discusiones y dudas generales:**  
  https://github.com/Erickpe8/SmartDifferentialCalc/discussions

Cualquier consulta enviada por estos medios será remitida al equipo desarrollador para dar respuesta de la manera más oportuna.

¡Gracias por llegar hasta aquí e interesarte en SmartDifferentialCalc! 💻✨

---

## ⭐ ¿Te gustó el proyecto?

Si este proyecto te sirvió, considera:
- ⭐ Darle una estrella en GitHub
- 🍴 Hacer un fork y contribuir
- 📢 Compartirlo con tus compañeros

---

<div align="center">

**Hecho con 🧠 y ☕ en Cúcuta, Colombia**

*"Democratizando el aprendizaje de ecuaciones diferenciales, una explicación a la vez"*

[⬆ Volver arriba](#-smartdifferentialcalc)

</div>
