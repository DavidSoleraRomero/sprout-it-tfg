# 🌱 Sprout It - TFG DAM

**Gestión gamificada de plantas** | *Proyecto fin de grado - CPIFP Alan Turing*

---

## ☘ Descripción

**Sprout It** es una aplicación diseñada para ayudar a los usuarios a gestionar sus plantas de una forma práctica y gamificada. Los usuarios podrán registrar sus plantas, asociarlas a una especie y un fertilizante, y realizar acciones como crear, leer, actualizar y eliminar plantas, especies y fertilizantes. Además, podrán llevar un control de los riegos realizados, sumando experiencia y subiendo de nivel con cada riego, lo que incentiva el cuidado de las plantas. 

**Funcionalidades principales:**

- 📝 Registrar plantas con sus especies y fertilizantes asociados  
- 💧  Llevar control de riegos con sistema de experiencia  
- 📊 Visualizar progreso mediante niveles  
- ☁️ Sincronización en la nube para acceso multiplataforma  

## 🎯 Objetivos del proyecto

| Objetivo | Beneficio |
| ------- | --------- |
| **Simplificar gestión** | Registro intuitivo de plantas y cuidados |
| **Gamificar experiencia** | Sistema de niveles por riegos realizados |
| **Multiplataforma** | Acceso desde cualquier dispositivo |
| **Educación botánica** | Recomendaciones personalizadas gracias a IA Generativa |

## 💻 Tecnologías utilizadas

### 📱 Frontend Web

| `Tecnología` | `Uso` |
| ---------- | --- |
| `Ionic + Angular` | `Desarrollo híbrido para Web, iOS y Android` |

### 🤖 Android Nativo

| `Tecnología` | `Uso` |
| ---------- | --- |
| `Kotlin` | `Funcionalidades específicas Android` |

### ☁️ Backend

| `Tecnología` | `Uso` |
| ---------- | --- |
| `Firebase Firestore` | `Base de datos en tiempo real` |
| `Firebase Auth` | `Autenticación` |

## 🛡 Esquema E/R de la base de datos

### Colecciones principales

1. **sprouters**: Extensión del perfil de usuario  
2. **species**: Datos de especies de plantas  
3. **plants**: Plantas registradas por usuarios  
4. **fertilizers**: Fertilizantes disponibles  
5. **experiences**: Registro de experiencia y niveles  
6. **locations**: Ubicaciones geográficas  

### 1. `sprouters`

| `Campo`         | `Tipo`      | `Descripción`              |
| --------------- | ----------- | -------------------------- |
| `id`            | `string`    | `ID del documento`         |
| `email`         | `string`    | `Email del usuario`        |
| `name`          | `string`    | `Nombre`                   |
| `surnames`      | `string`    | `Apellidos`                |
| `username`      | `string`    | `Nombre de usuario`        |
| `isPrivileged`  | `boolean`   | `Privilegios especiales`   |
| `image`         | `string`    | `Foto de perfil`           |
| `user`          | `string`    | `ID de Firebase Auth`      |

### 2. `species`

| `Campo`                    | `Tipo`      | `Descripción`                  |
| -------------------------- | ----------- | ------------------------------ |
| `id`                       | `string`    | `ID del documento`             |
| `commonName`               | `string`    | `Nombre común`                 |
| `scientificName`           | `string`    | `Nombre científico`            |
| `environmentType`          | `string`    | `"Interior"` o `"Exterior"`    |
| `lightRequirement`         | `string`    | `Requerimiento lumínico`       |
| `wateringFrequency`        | `number`    | `Días entre riegos`            |
| `recommendedFertilizer`    | `string`    | `Referencia a fertilizante`    |
| `recommendedFertilizerId`  | `string`    | `ID de fertilizante`           |
| `image`                    | `string`    | `Imagen de la especie`         |

### 3. `plants`

| `Campo`              | `Tipo`      | `Descripción`                  |
| -------------------- | ----------- | ------------------------------ |
| `id`                 | `string`    | `ID del documento`             |
| `name`               | `string`    | `Nombre asignado`              |
| `specie`             | `string`    | `Referencia a especie`         |
| `specieId`           | `string`    | `ID de especie`                |
| `sprouter`           | `string`    | `Referencia a usuario`         |
| `currentEnvironment` | `string`    | `Ambiente actual`              |
| `currentFertilizer`  | `string`    | `Referencia a fertilizante`    |
| `currentFertilizerId`| `string`    | `ID de fertilizante`           |
| `currentLightLevel`  | `string`    | `Nivel de luz`                 |
| `description`        | `string`    | `Descripción`                  |
| `lastWatered`        | `timestamp` | `Último riego`                 |
| `registerDate`       | `timestamp` | `Fecha de registro`            |
| `image`              | `string`    | `Foto de planta`               |

### 4. `fertilizers`

| `Campo` | `Tipo`    | `Descripción`           |
| ------- | --------- | ----------------------- |
| `id`    | `string`  | `ID del documento`      |
| `name`  | `string`  | `Nombre del fertilizante` |

### 5. `experiences`

| `Campo`                     | `Tipo`    | `Descripción`               |
| --------------------------- | --------- | --------------------------- |
| `id`                        | `string`  | `ID del documento`          |
| `currentSprouterExperience` | `number`  | `Puntos de experiencia`     |
| `sprouter`                  | `string`  | `Referencia a usuario`      |

### 6. `locations`

| `Campo`    | `Tipo`    | `Descripción`             |
| ---------- | --------- | ------------------------- |
| `id`       | `string`  | `ID del documento`        |
| `latitude` | `number`  | `Coordenada latitud`      |
| `longitude`| `number`  | `Coordenada longitud`     |

### 🔗 Relaciones

- `sprouters.user` → `Firebase Auth`  
- `plants.sprouter` → `sprouters.id`  
- `plants.specie` → `species.id`  
- `species.recommendedFertilizer` → `fertilizers.id`  
- `experiences.sprouter` → `sprouters.id`

---

> 📎 Todos estos apartados, incluyendo el desarrollo técnico, justificaciones, diseño y planificación, se encuentran explicados con detalle en el [Anteproyecto completo](https://jolly-ferret-4f4.notion.site/Sprout-It-Anteproyecto-67480a4cb7ed4ed6b85b363386838851?pvs=4).

---

## 🎥 Video Checkpoint (5 minutos)  
🔗 [Ver en YouTube](https://youtu.be/2HuGz19Bpaw)  
Resumen del estado actual del proyecto con una demostración práctica. En el video se exponen los principales avances, funcionalidades implementadas y cómo se cumplen los requisitos de prácticamente todas las asignaturas del ciclo.

---

## 📚 Historial de cambios y bibliografía  
📁 [Acceder a Google Drive](https://docs.google.com/document/d/1duXJVxwfllh2DBYBOJwPx-ZhWH_NcNUKUzaMo3aMl0U/edit?usp=sharing)  
Contiene documentación histórica, bibliografía y enlaces complementarios.

---

## 🔗 **Enlaces del Proyecto**

### 🌍 **Aplicación Web**

- 🔗 **Aplicación desplegada en Netlify (redirige a HOME)**  
  [https://sprout-it.netlify.app](https://sprout-it.netlify.app/)

- 🔗 **APK para Android de la aplicación web**  
  [Descargar en Google Drive](https://drive.google.com/file/d/1hkasUWkCA3Lv-6VoPXRQhch157X3kg1s/view?usp=sharing)

- 💻 **Repositorio (Ionic + Angular)**  
  [https://github.com/DavidSoleraRomero/sprout-it](https://github.com/DavidSoleraRomero/sprout-it)

---

### 📱 **Aplicación Móvil Android**

- 🔗 **APK para Android**  
  [Descargar en Google Drive](https://drive.google.com/file/d/1bBFZeGKTl9gY_Pl5oNLinjFYYYNMoDv7/view?usp=sharing)

- 📱 **Repositorio (Kotlin)**  
  [https://github.com/DavidSoleraRomero/sprout-it-android](https://github.com/DavidSoleraRomero/sprout-it-android)

---

### 🖥️ **Presentación del Proyecto**

- 📄 **PDF de la presentación (subido al repositorio)**  
  Disponible en el repositorio del proyecto (más arriba, junto al archivo README.md)

- 🎥 **Versión recomendada con vídeos y transiciones**  
  [Ver presentación en Canva (Opción 1)](https://www.canva.com/design/DAGn_7DdH4k/lT1p3St_KWpDTpDEwY4j0g/edit?utm_content=DAGn_7DdH4k&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)<br>
  [Ver presentación en Canva (Opción 2)](https://www.canva.com/design/DAGn_7DdH4k/R68UuyiAgjFl7b34ewgMfg/view?utm_content=DAGn_7DdH4k&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h08411931e1) <br>
  *Contiene todos los vídeos y animaciones que enriquecen la experiencia.*

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
- Se envía un correo de forma automática al usuario en tres situaciones:<br><br>
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

## 📺 **Manual Completo**

Para más detalles, consulta el **manual completo** en los siguientes videos. En estos videos encontrarás una **explicación detallada** sobre cada apartado de la aplicación, junto con su correspondiente demostración de cómo hacerlo. Se cubren todas las funcionalidades de la versión web y móvil, incluyendo el **registro**, **inicio de sesión**, gestión de **plantas**, **especies**, **fertilizantes**, características exclusivas de cada plataforma, y más detalles concretos.

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
  *Requiere de invitación al proyecto. Es preferible descargar el archivo .bmpr e importarlo directamente en Balsamiq.*

- 📁 **Archivos descargables de Balsamiq (Google Drive)**  
  [Descargar en Google Drive](https://drive.google.com/drive/folders/1jSSBkc7fMor_PphYmIKCauJaa-1RBIKC?usp=sharing)

- 🎯 **Diseño en Figma (modo solo visualización)**  
  [https://www.figma.com/proto/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1](https://www.figma.com/proto/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1)

- 🛠️ **Diseño en Figma (modo edición)**  
  [https://www.figma.com/design/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1](https://www.figma.com/design/qh59vF4jQMkRUArRqOMtrO/Sprout-It-Design?node-id=0-1&t=ETZ2eLpcvyPmhzej-1)

---

### 📊 Análisis de datos

- 📥 **Power BI + CSV (descarga desde Drive)**  
  Incluye el archivo `.pbix` y los CSV exportados desde la app.  
  [Descargar en Google Drive](https://drive.google.com/file/d/1MRItQrWM2B0W5DgkuhnRBqVsNCiYA8pu/view?usp=sharing)<br>
  > ⚠️ **IMPORTANTE:**  
  > El informe fue desarrollado **en la misma versión de Power BI Desktop: 2.141.1253.0 (64-bit, marzo de 2025)**.  
  > Se recomienda usar esta versión o una superior; de lo contrario, **el archivo no se podrá abrir correctamente**.

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
