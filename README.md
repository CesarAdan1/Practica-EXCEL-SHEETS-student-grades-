# Práctica: Cálculo de Promedio y Filtros Avanzados

¡Bienvenidos a la práctica de gestión de datos académicos! En este ejercicio aprenderás a utilizar **Excel** o **Google Sheets** para automatizar el cálculo de calificaciones y analizar el rendimiento de un grupo de estudiantes.

---

## Descripción
Aprenderás a registrar datos, aplicar fórmulas lógicas y utilizar herramientas de ordenamiento y filtrado para obtener información valiosa de una lista de 30 alumnos.

## Objetivos
* Dominar funciones básicas: `PROMEDIO()` y `SI()`.
* Aprender a arrastrar fórmulas para automatizar procesos.
* Utilizar filtros para segmentar datos (alumnos aprobados, reprobados y sobresalientes).

---

## 1. Estructura de la Tabla
Crea una hoja de cálculo con las siguientes columnas. Debes registrar **30 alumnos** con datos inventados.

| Alumno | Grupo | Materia | Parcial 1 | Parcial 2 | Parcial 3 | Promedio | Calificación Final |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: | :---: |
| Ejemplo: Juan Pérez | A | Física | 10 | 9 | 8 | *Fórmula* | *Fórmula* |

---

## 2. Fórmulas a Utilizar

### A. Calcular el Promedio
En la celda **G2** (debajo de la columna "Promedio"), ingresa la siguiente fórmula:
```excel
=PROMEDIO(D2:F2)

Luego, selecciona la esquina inferior derecha de la celda y arrastra hacia abajo hasta el alumno 30.

B. Determinar Calificación en Letra
En la celda H2 (debajo de "Calificación Final"), utilizaremos una función lógica para asignar una letra según el promedio:

```
=SI(G2>=9,"A",SI(G2>=8,"B",SI(G2>=7,"C",SI(G2>=6,"D","F"))))
```excel

Escala de conversión:

9.0 a 10: A

8.0 a 8.9: B

7.0 a 7.9: C

6.0 a 6.9: D

Menor a 6.0: F

3. Filtros y Análisis
Para activar los filtros, selecciona los encabezados de tu tabla y ve a:

En Excel: Pestaña Datos > Filtro.

En Google Sheets: Menú Datos > Crear un filtro.

Ejemplos de Visualización:
🔝 Ordenar por Mejores Promedios
Haz clic en el filtro de la columna Promedio y selecciona "De mayor a menor". Debería verse así:

```
Alumno,Grupo,Promedio,Calif. Final
Ana García,A,10.0,A
Luis Pérez,B,9.5,A
```excel

❌ Filtrar Reprobados
En el filtro de la columna Calificación Final, desmarca todas las opciones y deja solo la "F".
```
Alumno,Grupo,Promedio,Calif. Final
Carlos Ruiz,C,5.4,F
```excel

4. Entregables (Checklist)
Asegúrate de incluir lo siguiente en tu reporte o carpeta de evidencias:

[ ] Archivo de Excel/Link de Sheets con los 30 alumnos y fórmulas aplicadas.

[ ] Captura 1: Tabla completa ordenada por promedio (de mayor a menor).

[ ] Captura 2: Filtro aplicado para mostrar solo alumnos con Promedio de 10.

[ ] Captura 3: Filtro aplicado para mostrar solo alumnos con Calificación A.

[ ] Captura 4: Filtro aplicado para mostrar solo alumnos reprobados (F).

Nota: Si tu computadora está configurada en español de España o México, es posible que debas usar punto y coma (;) en lugar de coma (,) en las fórmulas. Ejemplo: =PROMEDIO(D2;F2).
