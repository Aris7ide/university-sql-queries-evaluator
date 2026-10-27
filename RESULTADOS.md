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

⏱ Tiempo: 0.53 ms
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

⏱ Tiempo: 0.38 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 3: Error
- **Descripción**: 1054 (42S22): Unknown column 'fecha_de_nacimiento' in 'where clause'


## ❌ Query 4: Error
- **Descripción**: 1054 (42S22): Unknown column 'telfono' in 'where clause'


## ❌ Query 5: Error
- **Descripción**: 'NoneType' object is not iterable

