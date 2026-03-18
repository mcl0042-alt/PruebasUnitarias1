 README.md — Proyecto ValidadorRegistro
# 🧪 Proyecto: ValidadorRegistro con JUnit 5

Este proyecto implementa un sistema básico de validación de datos para un registro de usuario, junto con una batería de pruebas unitarias usando **JUnit 5**.

---

## 📥 Instalación

Sigue estos pasos para clonar y ejecutar el proyecto en tu equipo:

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/tu-repo.git


2️⃣ Entrar en la carpeta del proyecto
cd tu-repo


3️⃣ Abrir el proyecto en tu IDE favorito
Puedes usar IntelliJ IDEA, Eclipse, VS Code o cualquier entorno compatible con Java.
4️⃣ Asegurar dependencias
Si usas Maven, asegúrate de tener JUnit 5 en tu pom.xml.
Si usas Gradle, revisa tu build.gradle.
5️⃣ Ejecutar los tests
Con Maven:
mvn test


Con Gradle:
gradle test



📸 Capturas de pantalla
<img width="591" height="565" alt="image" src="https://github.com/user-attachments/assets/77a22ad8-2991-48d4-9ba0-d058427401b3" />

✔️ Estructura del proyecto


📂 Estructura del proyecto
src/
 ├── main/java/instituto/
 │      └── ValidadorRegistro.java
 └── test/java/instituto/
        └── ValidadorRegistroTest.java



🧠 Funcionalidades del ValidadorRegistro
La clase ValidadorRegistro valida:
- ✔️ Nombre (no vacío)
- ✔️ Contraseña (mínimo 8 caracteres)
- ✔️ Email (debe contener '@')
- ✔️ Edad (mínimo 16 años)

🧪 Pruebas unitarias
En ValidadorRegistroTest se incluyen los siguientes tests:
✔️ Test de ejemplo
- Acepta un nombre válido.
🧩 Retos implementados
- ❌ Rechazar nombre vacío
- ✔️ Aceptar contraseña de exactamente 8 caracteres
- ❌ Rechazar contraseña demasiado corta
- ❌ Rechazar email sin arroba
- ✔️ Aceptar edad mínima legal (16 años)

📌 Objetivo del proyecto
Este ejercicio sirve para aprender:
- Cómo diseñar validaciones básicas
- Cómo crear pruebas unitarias con JUnit 5
- Cómo escribir asserts correctos
- Cómo estructurar un proyecto Java limpio y mantenible

👨‍💻 Autor
Proyecto realizado por Mcl como práctica de testing y validación en Java
