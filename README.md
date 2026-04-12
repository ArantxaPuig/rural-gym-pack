# 🏋️‍♂️ RURAL GYM · Base de Datos de Práctica

Proyecto desarrollado durante el **Bootcamp Data Analyst · Semana 06 (Jueves)**, enfocado en el diseño y explotación de una base de datos relacional normalizada (3FN).

---

## 📌 Descripción

Este proyecto simula la gestión de un gimnasio rural en Asturias, permitiendo trabajar con estructuras reales de datos: socios, centros, clases y reservas.

El objetivo principal es practicar:
- Modelado de bases de datos
- Normalización (3ª Forma Normal)
- Relaciones entre tablas
- Consultas SQL (JOIN, agregaciones, vistas)

---

## 🧱 Estructura de la Base de Datos

### 🔹 Tablas principales

- **centros**  
  Sedes rurales donde se realizan las actividades.

- **socios**  
  Personas inscritas (alumnado y profesorado).

- **clases**  
  Actividades disponibles en los centros.

- **reservas**  
  Cabecera de cada reserva (una por visita).

- **detalle_reserva**  
  Clases incluidas en cada reserva.  

  🔑 Clave primaria compuesta:
id_reserva + id_clase


---

## 📊 Vistas (Views)

Diseñadas para facilitar el análisis de datos:

- **vista_reservas_completas**  
Información desnormalizada de reservas.

- **vista_clases_demanda**  
Ranking de clases más populares.

- **vista_socios_por_centro**  
Número de socios por sede.

- **vista_socios_activos**  
Socios que han realizado al menos una reserva.

- **vista_actividad_semanal**  
Tendencia de reservas por fecha.

---

## 🔍 Concepto clave: LEFT JOIN vs INNER JOIN

Este dataset incluye un caso práctico muy útil:

### 🧪 Socios sin reservas
- Francisco Jimenez (id 214)  
- Lucia Llaneza (id 221)  
- Oksana Tokmakova (id 224)

👉 **Comportamiento:**
- Con `INNER JOIN` → NO aparecen  
- Con `LEFT JOIN` → SÍ aparecen  

💡 Ideal para entender cómo afectan los JOIN en los resultados.

---

## 🎯 Objetivos de aprendizaje

- Comprender relaciones entre entidades
- Aplicar correctamente JOINs
- Analizar datos con vistas SQL
- Detectar casos reales (datos faltantes, relaciones incompletas)

---

## 🛠️ Tecnologías utilizadas

- SQL
- DB Browser (SQLite)
- Git
- GitHub

---

## 🚀 Cómo usar este proyecto

1. Clona el repositorio:
```bash
git clone https://github.com/ArantxaPuig/kepler-lab.git