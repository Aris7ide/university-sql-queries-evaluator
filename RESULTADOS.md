# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 0 correctas de 5 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,7 @@
 apellido1 | apellido2 | nombre
-Domínguez | Guerrero | Antonio
 Gea | Ruiz | Sonia
-Gutiérrez | López | Juan
 Heller | Pagac | Pedro
-Herman | Pacocha | Daniel
 Hernández | Martínez | Irene
-Herzog | Tremblay | Ramón
-Koss | Bayer | José
 Lakin | Yundt | Inma
 Saez | Vega | Juan
 Sánchez | Pérez | Salvador
-Strosin | Turcotte | Ismael
```

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 2: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,4 @@
 nombre | apellido1 | apellido2
 Pedro | Heller | Pagac
-Ismael | Strosin | Turcotte
+Pedro | Heller | Pagac
+Pedro | Heller | Pagac
```

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1 @@
-id | nombre | apellido1 | apellido2 | fecha_nacimiento
-7.00 | Ismael | Strosin | Turcotte | 1999-05-24
-22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
+nombre | apellido1 | apellido2
```

⏱ Tiempo: 0.19 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1 @@
-nombre | apellido1 | apellido2 | nif
-Antonio | Fahey | Considine | 10485008K
-Guillermo | Ruecker | Upton | 85869555K
+id_profesor | id_departamento
```

⏱ Tiempo: 0.22 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
🚨 `JOIN` sin índice. Revisar claves foráneas e índices.

---

## ❌ Query 5: Error
- **Descripción**: 'NoneType' object is not iterable

