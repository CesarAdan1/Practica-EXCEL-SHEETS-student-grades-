# Práctica: Cálculo de Promedio de 3 Parciales, Calificación Final y Filtros Avanzados (Excel / Google Sheets)

Descripción

En esta práctica aprenderás a: 
Registrar datos académicos de 30 alumnos
Calcular el promedio de los 3 parciales
Obtener la calificación final en letra (A–F)
Aplicar filtros y ordenamiento por promedio, grupo, materia
Filtrar alumnos con calificación perfecta (10 o A)
Analizar el rendimiento académico

Objetivos

Dominar el uso de fórmulas básicas en hojas de cálculo.

Utilizar correctamente PROMEDIO(), SI() y CONTAR.SI().

Ordenar datos según criterios académicos.

Analizar resultados por grupo o materia.

Filtrar estudiantes sobresalientes o reprobados.

Estructura de la Tabla (con 30 alumnos)

Crea una hoja con las siguientes columnas:

Alumno	Grupo	Materia	Parcial 1	Parcial 2	Parcial 3	Promedio	Calificación Final

Llena mínimo 30 alumnos con datos inventados.

Instrucciones:

1. Registrar los datos de los 30 alumnos

Llena las columnas:

Alumno (nombre completo)

Grupo (ej. A, B, C)

Materia (ej. Matemáticas, Español, Física)

Parciales 1, 2 y 3

2. Calcular el Promedio

En la columna Promedio, celda G2, escribe:

```js
=PROMEDIO(D2:F2)
```

Explicación rápida:

D2 = Parcial 1

E2 = Parcial 2

F2 = Parcial 3

Arrastra hacia abajo hasta el alumno #30.

3. Calificación Final en Letra (A, B, C, D, F)

En la columna Calificación Final, celda H2 escribe:

```js

=SI(G2=10,"A",SI(G2>=9,"A",SI(G2>=8,"B",SI(G2>=7,"C",SI(G2>=6,"D","F")))))
```

Esto convierte el promedio numérico a letra según la escala:

10 = A

9 = A

8 = B

7 = C

6 = D

<6 = F

Arrastra hacia abajo hasta el alumno #30.
 4. Activar Filtros
En Excel

Selecciona toda la tabla.

Datos → Filtro.

En Google Sheets

Selecciona la tabla.

Datos → Crear filtro.

Aparecerá un icono de embudo (▼) en cada columna.

5. Ordenar por Promedio

Haz clic en ▼ de la columna Promedio →

Ordenar de mayor a menor (mejores alumnos primero)

Ordenar de menor a mayor (alumnos que necesitan apoyo)

6. Filtrar alumnos con 10 de promedio o calificación A
Opción 1: Filtrar 10 en Promedio

En el filtro de la columna Promedio:

Desmarca todos

Deja solo marcado 10

Opción 2: Filtrar por calificación A

En la columna Calificación Final, filtro ▼:

Deja únicamente seleccionada A

Esto mostrará únicamente a los alumnos con desempeño sobresaliente.

7. Filtrar alumnos reprobados (<6)

Columna Promedio:

Filtro → dejar solo valores de 0 a 5.9

Columna Calificación Final:

Filtro → seleccionar F

** Entregables:

Tabla con 30 alumnos completos.

Promedio calculado correctamente.

Calificación final en letra.

Captura de pantalla de la tabla ordenada por promedio.

Captura filtrando solo alumnos con 10.

Captura filtrando solo alumnos con A.

Captura filtrando solo reprobados.

(Opcional) Ordenar por Grupo → Promedio.

