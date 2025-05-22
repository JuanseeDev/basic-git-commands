# 📘 Guía Básica de Git

Este archivo explica de forma sencilla y técnica los comandos principales de Git, para ayudarte a entender y aplicar control de versiones en tus proyectos.

---

## 🔧 Comandos Principales

### 1️⃣ `git init`
Inicializa un repositorio de Git en la carpeta actual.

- **¿Qué hace?**  
  Crea una carpeta oculta `.git` que empieza a rastrear los cambios en tu proyecto.

- **¿Para qué sirve?**  
  Le indica a Git que comience a llevar el historial de versiones.

    ```bash
    git init

---

### 2️⃣ `git add`
Agrega archivos al área de preparación (staging area).

- **¿Qué hace?**
  Marca archivos para incluirlos en el próximo commit.

- **¿Para qué sirve?**
  Te permite seleccionar los archivos que deseas guardar como parte de un cambio.

    ```bash
    git add archivo.html
    git add .

---

### 3️⃣ `git commit -m "mensaje"`
Guarda los cambios preparados con un mensaje que describa lo que hiciste.

- **¿Qué hace?**
  Crea un “punto de control” o snapshot en la historia del proyecto.

- **¿Para qué sirve?**
  Permite llevar un registro de qué cambió y por qué.

    ```bash
    git commit -m "Agregué el archivo HTML inicial"

---

### 4️⃣ `git push origin main`
Envía tus commits locales al repositorio remoto (por ejemplo, en GitHub).

- **¿Qué hace?**
  Sube tus cambios al repositorio en línea.

- **¿Para qué sirve?**
  Para respaldar tu trabajo o colaborar con otras personas.

    ```bash
    git push origin main

---

### 🔄 `Cómo subir un cambio a un archivo ya existente`
Supón que editaste un archivo. Los pasos serían:

    ```bash
    git add archivo.html
    git commit -m "Actualicé el contenido del archivo"
    git push origin main

---

### 🔐 `Seguridad al usar Git en computadoras públicas`
-⚠️ Git recordará la URL del repositorio, pero no tus credenciales si estás en un PC público.

-🔑 Usa un token de acceso personal (PAT) en lugar de tu contraseña.

-❌ Nunca guardes las credenciales en el navegador o en el sistema.

-✅ Al terminar, puedes ejecutar:

    ```bash
    git remote remove origin

Y también puedes eliminar el token desde tu cuenta de GitHub para mayor seguridad.

---

¡Listo! Con estos comandos ya puedes trabajar con Git de forma segura y profesional 🚀