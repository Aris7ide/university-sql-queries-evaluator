# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 19 correctas de 24 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.21 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.20 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.20 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.22 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.45 ms
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

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: id_profesor,id_grado, PRIMARY, PRIMARY,id_departamento

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.23 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
🚨 `JOIN` sin índice. Revisar claves foráneas e índices.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: id_profesor, PRIMARY

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: id_profesor, PRIMARY

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: id_profesor, PRIMARY, id_departamento, id_asignatura

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.23 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.23 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_departamento

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,10 @@
 departamento | total
+Educación | 3.00
 Informática | 2.00
 Matemáticas | 2.00
 Economía y Empresa | 2.00
-Educación | 3.00
+Química y Física | 2.00
 Agronomía | 1.00
-Química y Física | 2.00
 Filología | 0.00
 Derecho | 0.00
 Biología y Geología | 0.00
```

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 20: Correcto

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 21: Correcto

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-grau | tipo | total_creditos
+grau | tipus | total_creditos
 Grado en Ingeniería Informática (Plan 2015) | básica | 72.00
 Grado en Ingeniería Informática (Plan 2015) | obligatoria | 54.00
 Grado en Ingeniería Informática (Plan 2015) | optativa | 180.00
```

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_grado

---

## ❌ Query 23: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
-anyo_inicio | total
-2014.00 | 3.00
-2018.00 | 3.00
+id | nif | nombre | apellido1 | apellido2 | ciudad | direccion | telefono | fecha_nacimiento | sexo | tipo
+12.00 | 85366986W | Carmen | Streich | Hirthe | Almería | C/ Almanzora | NULL | 1971-04-29 | M | profesor
```

⏱ Tiempo: 0.24 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 24: Error
- **Descripción**: 'NoneType' object is not iterable

