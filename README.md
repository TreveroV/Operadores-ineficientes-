# Operadores ineficientes
📘 Descripción del proyecto.
El contexto es el siguiente: El servicio de telefonía virtual CallMeMaybe está desarrollando una nueva función que brindará a los supervisores y las supervisores información sobre los operadores menos eficaces. Se considera que un operador es ineficaz si tiene una gran cantidad de llamadas entrantes perdidas (internas y externas) y un tiempo de espera prolongado para las llamadas entrantes. Además, si se supone que un operador debe realizar llamadas salientes, un número reducido de ellas también será un signo de ineficacia.

⚙️ Herramientas y tecnologías usadas.
1.-pandas
2.-numpy
3.-seaborn
4.-scipy
5.-statsmodel
5.-Tableau

💡 Desafío o caso de uso.
Para este trabajo me tocó definir el plan de actividades, quedó de esta forma:

1.- Análisis Exploratorio de Datos (EDA)
Distribuciones generales: duración de llamadas, llamadas perdidas, proporción entrantes/salientes/internas.

Tendencias temporales: evolución de llamadas por día/mes.

Comparación entre operadores:

Boxplots o barras para ver quiénes concentran más llamadas perdidas.

Heatmap de correlación entre métricas (missed_rate, avg_wait, outgoing_rate).

2.- Identificación de operadores ineficaces
Definir reglas:

Muchos missed calls (ej. >25% de llamadas entrantes).

Alto tiempo de espera promedio.

Pocas llamadas salientes en clientes que deberían hacerlas.

Crear un ranking de operadores con un score de ineficiencia.

Visualización: gráfico de barras con top operadores menos eficaces.

3.- Pruebas de hipótesis estadísticas
Con los Resultados anteriores determinar algunas hipotesis y comprobarlas.

4.- Conclusiones y Recomendaciones
Resumir hallazgos clave: qué características tienen los operadores ineficaces, qué patrones se observan.

Proponer acciones

5.- Visualización final
Realizar un Dashboard en Tableu para que se pueda monitorear de fforma dinamica a los operadores.


📊 Resultados o aprendizajes.
Hicimos una exploración y encontramos varias cosas, enumeremoslas:

1.- El plan A es que contiene mas operadores ineficaces.
2.- Hay varios factores que influyen en que definimos como ineficaz pero el que mas afecta al plan A es el tiempo de espera.
3.- El plan C es el que mayor llamadas perdidas tiene.
4.- El plan A tiene el mayor numero de llamadas totales pero no es el que tiene el mayor numero de llamadas salientes.


Con esto podemos hacer algunas recomendaciones (y tal vez unas cuantas hipotesis mas)

Parece que lo que más afecta a la empresa son los tiempos de espera, pero también pareciera que con el plan A hay muchos casos de llamadas internas, habrá algún factor que provoque que los operadores de este plan no hagan menos llamadas de salida? y que esto está provocando que generen demasiados tiempo de espera?, como también pudimos observar el plan A tiene mayoy número de llamadas, habra una forma de que podamos equilibrar el número de llamadas entre los 3 planes? porque este puede ser un factor al aumento de tiempos de espera en este plan y por lo tanto saturación de los operadores de este plan.

Se complemento una visualización con Tableau de los datasets https://public.tableau.com/views/ProyectoFinal_17590201621790/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
