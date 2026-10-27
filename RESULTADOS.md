# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 7 correctas de 12 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.26 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.16 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.17 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1 @@
 nombre | apellido1 | apellido2 | nif
-Antonio | Fahey | Considine | 10485008K
-Guillermo | Ruecker | Upton | 85869555K
```

⏱ Tiempo: 0.16 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.19 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 6: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-apellido1 | apellido2 | nombre | departamento
+apellido1 | apellido2 | nombre | nombre
 Fahey | Considine | Antonio | Economía y Empresa
 Hamill | Kozey | Manolo | Informática
 Kohler | Schoen | Alejandro | Matemáticas
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY,nif, PRIMARY, PRIMARY,id_asignatura,id_curso_escolar

---

## ❌ Query 8: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1 @@
 nombre
-Informática
```

⏱ Tiempo: 0.22 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY, id_profesor,id_grado

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
-departamento | apellido1 | apellido2 | nombre
-Agronomía | Monahan | Murray | Micaela
-Economía y Empresa | Fahey | Considine | Antonio
-Economía y Empresa | Lemke | Rutherford | Cristina
-Educación | Ruecker | Upton | Guillermo
-Educación | Spencer | Lakin | Esther
-Educación | Streich | Hirthe | Carmen
-Informática | Hamill | Kozey | Manolo
-Informática | Ramirez | Gea | Zoe
-Matemáticas | Kohler | Schoen | Alejandro
-Matemáticas | Schmidt | Fisher | David
-Química y Física | Schowalter | Muller | Francesca
-Química y Física | Stiedemann | Morissette | Alfredo
+nombre | apellido1 | apellido2 | nombre
+NULL | Fahey | Considine | Antonio
+NULL | Hamill | Kozey | Manolo
+NULL | Kohler | Schoen | Alejandro
+NULL | Monahan | Murray | Micaela
+NULL | Ruecker | Upton | Guillermo
+NULL | Schowalter | Muller | Francesca
+NULL | Spencer | Lakin | Esther
+NULL | Stiedemann | Morissette | Alfredo
+NULL | Streich | Hirthe | Carmen
+Agronomía | Schmidt | Fisher | David
+Derecho | Lemke | Rutherford | Cristina
+Economía y Empresa | Ramirez | Gea | Zoe
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.14 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
🚨 `JOIN` sin índice. Revisar claves foráneas e índices.

---

## ❌ Query 12: Error
- **Descripción**: 'NoneType' object is not iterable

