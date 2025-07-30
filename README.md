# 📊 Proyecto de Normalización de Bases de Datos

Este repositorio muestra cómo aplicar la **normalización** (1NF, 2NF, 3NF) a diferentes escenarios reales de manejo de datos, con ejemplos prácticos para:

- 🛒 **Control de Compras de una tienda**
- 🎓 **Historial Académico universitario**
- 📚 **Sistema de Préstamos de una Biblioteca educativa**

---

## 🧾 Descripción General

En cada caso se parte de una **base de datos desnormalizada** (con datos redundantes y mezclados) y se realiza la transformación para cumplir con las tres primeras formas normales, eliminando redundancias, mejorando la integridad y la eficiencia del modelo.

**Cada ejemplo incluye:**
- 📂 Dataset original (Excel) con todos los datos mezclados  
- 🧱 Tablas resultantes tras aplicar 1NF, 2NF y 3NF  
- 📌 Explicaciones y justificaciones del proceso  
- 🧠 Modelado conceptual de entidades y relaciones  

---

## 🔍 Casos de Estudio

### 1️⃣ Control de Compras

- 📋 Tabla original: clientes, productos, compras y pagos mezclados.  
- ✔️ **1NF**: Celdas atómicas sin listas ni datos combinados.  
- ✔️ **2NF**: Separación de clientes y productos en tablas independientes (eliminando dependencias parciales).  
- ✔️ **3NF**: Eliminación de campos derivados como `total_price` para evitar datos inconsistentes.  
- 🧾 Entidades resultantes: `Customers`, `Products`, `Purchases`.

---

### 2️⃣ Historial Académico Universitario

- 📋 Tabla inicial: registro combinado de estudiantes, cursos, notas, profesores y periodos.  
- ✔️ **1NF**: Extracción de datos atómicos en tablas separadas.  
- ✔️ **2NF**: Separación de estudiantes, profesores y cursos; inscripción vinculada a semestre y curso.  
- ✔️ **3NF**: Solo quedan atributos que dependen directamente de la clave primaria en cada entidad.  
- 🧾 Entidades resultantes: `Students`, `Courses`, `Professors`, `Enrollment`.

---

### 3️⃣ Préstamos en Biblioteca Educativa

- 📋 Tabla original: préstamos, estudiantes, libros y bibliotecarios mezclados.  
- ✔️ **1NF**: División inicial entre entidades básicas (libros, estudiantes, miembros, préstamos).  
- ✔️ **2NF**: Eliminación de dependencias parciales, creación de `Library_Staff`.  
- ✔️ **3NF**: Únicamente dependencias de clave primaria, referencia a todas las claves externas.  
- 🧾 Entidades resultantes: `Students`, `Books`, `Librarians`, `Loans`.

---

## 🛠️ Tecnologías y Herramientas

- 📊 Microsoft Excel para la manipulación y transformación de datos.  
- 🧩 Fundamentos de diseño y modelado relacional.  
- 🖼️ Diagramas Entidad-Relación (ER) para visualizar la estructura final.

---

## 🚀 Contribuciones

Este proyecto tiene fines educativos y puede extenderse con:

- 🧬 Scripts SQL para crear e implementar las tablas normalizadas  
- ⚙️ Automatización de cálculos derivados  
- 📈 Consultas de ejemplo para análisis y reportes  
- 💽 Un modelo físico listo para cargar en sistemas gestores de bases de datos (DBMS)

---

## 👥 Colaboradores

- 👩‍💻 Susana  
- 👩‍💻 Daniela  
- 👨‍💻 Sebastián  
