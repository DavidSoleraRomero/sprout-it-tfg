# 🌱 Sprout It - TFG DAM

**Gestión gamificada de plantas** | *Proyecto fin de grado - CPIFP Alan Turing*

---

## 🎥 Video Checkpoint (5 minutos)  
🔗 [Ver en YouTube](https://youtu.be/2HuGz19Bpaw)  
Resumen del estado actual del proyecto con una demostración práctica. En el video se exponen los principales avances, funcionalidades implementadas y cómo se cumplen los requisitos de prácticamente todas las asignaturas del ciclo.

---

## 📚 Historial de cambios y bibliografía  
📁 [Acceder a Google Drive](https://docs.google.com/document/d/1duXJVxwfllh2DBYBOJwPx-ZhWH_NcNUKUzaMo3aMl0U/edit?usp=sharing)  
Contiene documentación histórica, bibliografía y enlaces complementarios.

---

## 📌 Descripción breve

Sprout It es una aplicación multiplataforma que convierte el seguimiento y cuidado de plantas en una experiencia intuitiva y motivadora. Integra:

- 📲 **Gestión botánica**: permite registrar plantas, especies, fechas de riego, fertilización, etc.
- 🎮 **Elementos gamificados**: las plantas suben de nivel con el cuidado del usuario.
- ☁️ **Sincronización en la nube**: disponible en versión móvil (Kotlin) y web (Ionic Angular) con datos unificados mediante Firebase y persistencia local con Room.
- 🧠 **Procesamiento externo**: generación de CSV desde la app y análisis con Power BI gracias a una API desarrollada en Python.
- 🧪 **Diseño iterativo**: prototipado inicial en Balsamiq y refinamiento visual y funcional en Figma.

> 🔍 **Toda la documentación técnica y justificación del proyecto está disponible en el [Anteproyecto completo](https://jolly-ferret-4f4.notion.site/Sprout-It-Anteproyecto-67480a4cb7ed4ed6b85b363386838851?pvs=4)**

---

## 🔗 **Enlaces del Proyecto**

### 🌍 **Aplicación Web**

- 🔗 **Aplicación desplegada en Netlify (redirige a HOME)**  
  [https://sprout-it.netlify.app](https://sprout-it.netlify.app/)

- 💻 **Repositorio (Ionic + Angular)**  
  [https://github.com/DavidSoleraRomero/sprout-it](https://github.com/DavidSoleraRomero/sprout-it)

---

### 📱 **Aplicación Móvil**

- 📱 **Repositorio (Kotlin)**  
  [https://github.com/DavidSoleraRomero/sprout-it-android](https://github.com/DavidSoleraRomero/sprout-it-android)

---

## 📝 **Instrucciones Generales**

Estas instrucciones aplican tanto a la **aplicación web** como a la **aplicación móvil**. En los videos a continuación se mencionan detalles específicos para cada plataforma:

### ✍️ **Registro de Usuario:**
- Regístrate y si eres un *sprouter privilegiado*, podrás **editar** y **eliminar** especies y fertilizantes.

### 🔑 **Iniciar Sesión:**
- Inicia sesión con la opción de **autologin**, para una experiencia continua sin necesidad de reingresar tus credenciales.

### 🌱 **Gestión de Plantas:**
- Puedes **regar**, **visualizar**, **editar** y **eliminar** las plantas en tu colección.

### 🌿 **Gestión de Especies:**
- Visualiza la ubicación de las especies y tienes la opción de **editar** o **eliminar** según sea necesario.

### 🌾 **Gestión de Fertilizantes:**
- Puedes **ver**, **editar** y **eliminar** los fertilizantes asignados a tus plantas.

### 👤 **Perfil de Usuario:**
- Modifica tu **foto de perfil**, **nombre**, **apellido**, **usuario** y consulta tu **correo electrónico**.

---

## 🔍 **Algunos Detalles Específicos**

### 🌍 **Aplicación Web (Ionic + Angular)**

#### 📧 **Envío de Correos**
- Se **envía un correo** de forma automática al usuario en tres situaciones:
  - **Registrarse**
  - **Iniciar sesión**
  - **Intento de inicio de sesión fallido**

#### 🤖 **IA Generativa**
- **IA generativa** aplicada a las colecciones de:
  - **Plantas**
  - **Especies**
  - **Fertilizantes**
  
  Esto permite ofrecer **descripciones personalizadas** e información relevante para cada colección.

#### 🌳 **Vista 3D de Plantas**
- **Vista 3D interactiva (ThreeJS)** de las plantas, para proporcionar una **experiencia visual y enriquecedora** al usuario.

---

### 📱 **Aplicación Móvil (Kotlin)**

#### 🔗 **Compartir Información**
- En la versión móvil, puedes **compartir información** de tus **plantas** y **especies** con otras aplicaciones, gracias a la integración de **Intents**.

#### 💾 **Almacenamiento Local**
- La aplicación **almacena los datos localmente** utilizando **Room**, lo que garantiza un **acceso rápido y eficiente**, mientras se sincronizan los datos con Firebase.

---

## 📹 **Manual Detallado**

Para más detalles, consulta el **manual completo** en los siguientes videos:

🎥 **Manual Detallado de la Aplicación Web (Ionic + Angular)**  
[Ver video](https://youtu.be/VcPFS6k2OSQ)

🎥 **Manual Detallado de la Aplicación Móvil (Kotlin)**  
[Ver video](https://youtu.be/GoUTTPHh7dQ)

---

### 🧠 Procesamiento de datos

- 🐍 **API en Python para generar CSV a partir de datos de Firebase**  
  [https://github.com/DavidSoleraRomero/sprout-it-pd](https://github.com/DavidSoleraRomero/sprout-it-pd)

---

### 🎨 Diseño de la interfaz

- 🖼️ **Prototipo en Balsamiq (solo visualización)**  
  [https://balsamiq.com/example/sprout-it](https://balsamiq.com/example/sprout-it)

- 📁 **Archivos descargables de Balsamiq (Google Drive)**  
  *(Pendiente de añadir enlace)*

- 🎯 **Diseño en Figma (modo solo visualización)**  
  [https://www.figma.com/proto/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1](https://www.figma.com/proto/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1)

- 🛠️ **Diseño en Figma (modo edición)**  
  [https://www.figma.com/design/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1](https://www.figma.com/design/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1)

---

### 📊 Análisis de datos

- 📥 **Power BI + CSV (descarga desde Drive)**  
  Incluye el archivo `.pbix` y los CSV exportados desde la app.  
  *(Pendiente de añadir enlace)*

---

## 🧑‍💻 Desarrollador Principal

**David Solera Romero**  
*Estudiante de 2º Desarrollo de Aplicaciones Multiplataforma*

🏛️ CPIFP Alan Turing  
✉️ **Contacto:** soleraromerodavid@gmail.com  
💻 **GitHub:** [DavidSoleraRomero](https://github.com/DavidSoleraRomero)

---

> 🌿 *"Programar es como regar una planta; con paciencia y dedicación, crece algo extraordinario."*  
> — *Filosofía de desarrollo de **Sprout It***
