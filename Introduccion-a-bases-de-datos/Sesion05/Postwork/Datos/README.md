(1) Base de Datos
Aquí pongan el nombre de su base de datos y la o las colecciones que crearon.
-auto-mpg1.csv

Base de datos: DAVID94
Colección:     auto-mpg

(2) Estructura del archivo CSV (auto-mpg1.csv)
Aquí pongan el header del archivo CSV que usaron como dataset. La idea es que contrasten los documentos cargados en MongoDB con este header para asegurar que la carga fue correcta.

-MPG,Cylinders,Displacement,horsepower,Weight,Acceleration,Model_year,Origin,Car_Name

(3) Consultas
Aquí pongan las consultas que pensaron y como primera línea pongan con qué la van a ejecutar, es decir, un filtro, proyección, ordenamiento, etc.

¿Pregunta 1?
¿cuántos registros hay de cierto tipo o categoría?

// SORT
{Car_Name:1}
            Respuesta = 398

¿Pregunta 2?
¿cuántos registros hay donde el nummero de clindros sea igual a 8?


//FILTER
{Cylinders: "8"}
          Respuesta = 103

¿Pregunta 3?
¿Que vehiculo tiene el menor tiempo de aceleracion?


//SORT
{Acceleration: -1}
          Respuesta = MPG:"15"
                      Cylinders:"8"
                      Displacement:"390"
                      horsepower:"190"
                      Weight:"3850"
                      Acceleration:"8.5"
                      Model_year:"70"
                      Origin:"1"
                      Car_Name:"amc ambassador dpl"
          
