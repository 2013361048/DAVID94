(1) Base de Datos 
Aquí pongan el nombre de su base de datos y la o las colecciones que crearon. -auto-mpg1.csv

Base de datos: DAVID94 Colección: auto-mpg

(2) Consultas 
Aquí pongan las consultas que pensaron y como primera línea pongan con qué la van a ejecutar, es decir, un filtro, proyección, ordenamiento, etc.

¿Pregunta 1? ¿cuántos autos son marca Toyota?

// FILTER {Car_Name: /toyota/} 
   Respuesta:25

¿Pregunta 2? ¿cuántos autos son marca Toyota con 6 cilindros?

// FILTER {Car_Name: /toyota/, Cylinders: "6"} 
  Respuesta:3
  
¿Pregunta 3? ¿Cual es el maximo ahorro de MPG que dan los autos?

AGGREGATIONS

{
  _id: "MPG",
  Autos_Ahorradores: {
    $max: "$MPG"
  }
}

Respuesta = 9
