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

## 🔗 Enlaces del proyecto

### 🌍 Aplicación Web

- 🔗 **Aplicación desplegada en Netlify (redirige a HOME)**  
  [https://sprout-it.netlify.app](https://sprout-it.netlify.app/)

- 💻 **Repositorio (Ionic + Angular)**  
  [https://github.com/DavidSoleraRomero/sprout-it](https://github.com/DavidSoleraRomero/sprout-it)

---

### 📱 Aplicación Móvil

- 📱 **Repositorio (Kotlin)**  
  [https://github.com/DavidSoleraRomero/sprout-it-android](https://github.com/DavidSoleraRomero/sprout-it-android)

---

## 📝 Instrucciones Generales

Estas instrucciones aplican tanto a la **aplicación web** como a la **aplicación móvil**. En los videos a continuación se mencionan detalles específicos para cada plataforma:

1. **Registro de Usuario:**  
   Puedes registrarte en la aplicación, y si eres un *sprouter privilegiado*, tendrás la capacidad de editar y eliminar especies y fertilizantes.

2. **Iniciar Sesión:**  
   Puedes iniciar sesión y disfrutar de una función de *autologin* que mantiene tu sesión abierta para facilitar el uso.

3. **Gestión de Plantas:**  
   Puedes regar tus plantas, visualizarlas, editarlas y eliminarlas según lo desees.

4. **Gestión de Especies:**  
   Visualiza la ubicación de las especies, edítalas o elimínelas.

5. **Gestión de Fertilizantes:**  
   Puedes visualizar, editar y eliminar los fertilizantes asociados a las plantas.

6. **Perfil de Usuario:**  
   Modifica tu foto de perfil, nombre, apellido, usuario y consulta tu correo electrónico.

---

## 🔍 Detalles Específicos

### 🌍 **Aplicación Web (Ionic + Angular)**

- **Envío de correos:**  
  Se manda un correo al usuario al registrarse, al iniciar sesión y al intentar un inicio de sesión.

- **IA Generativa:**  
  Se ha implementado **IA generativa** sobre cada colección (plantas, especies y fertilizantes) para proporcionar descripciones e información más detallada y precisa.

- **Vista 3D de Plantas:**  
  La aplicación web incluye una vista 3D interactiva de las plantas, mejorando la experiencia visual y de usuario.

---

### 📱 **Aplicación Móvil (Kotlin)**

- **Compartir Información:**  
  En la versión móvil, los usuarios pueden **compartir** información sobre plantas, especies y fertilizantes mediante **Intents**.

- **Almacenamiento Local:**  
  Los datos de la aplicación se pueden **almacenar localmente** en el dispositivo para un acceso rápido y sin conexión.

---

## 📹 Manual Detallado

Para más detalles, consulta el **manual completo** en los videos siguientes:

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
