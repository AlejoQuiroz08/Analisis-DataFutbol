# Analisis-DataFutbol
Este repositorio contiene un script en Python que realiza un análisis de datos sobre el ranking de clubes de fútbol.

Requisitos
Para ejecutar este script, necesitarás tener instalado lo siguiente:

Python 3.x
pandas
pymongo
Puedes instalar las dependencias usando pip:

pip install pandas pymongo
Descripción de los Scripts:
Ranking de equipos de futbol: El script realiza las siguientes tareas:

Lee un archivo CSV que contiene el ranking de clubes de fútbol.

Elimina filas duplicadas del DataFrame.

Reemplaza los valores nulos en columnas numéricas por la media de cada columna.

Calcula el máximo, mínimo y promedio del ranking de los equipos.

Convierte el DataFrame a un diccionario para facilitar su inserción en MongoDB.

Conecta con una instancia local de MongoDB.

Inserta el diccionario en una colección llamada 'RankingDeEquipos' en la base de datos 'FutbolData'.

Cierra la conexión con MongoDB.

Ranking de jugadores de futbol:

Realiza las mismas opearaciones cambiando el csv por el que contiene la informacion de los jugadores.

Inserta el diccionario en una coleccion llamada 'RankingDeJugadores' en la base de datos FutbolData.

Inserción de datos: 1.Conexión a MongoDB Local: El script se conecta a dos bases de datos locales de MongoDB (basededatos1 y basededatos2) y a sus respectivas colecciones (coleccion1 y coleccion2). 2.Conexión a MongoDB Atlas: Se establece una conexión con MongoDB Atlas utilizando las credenciales proporcionadas en la URL de conexión. 3.Copia de datos: Se copian todos los documentos de las colecciones locales a una única colección en MongoDB Atlas. 4.Cierre de Conexiones: Finalmente, se cierran todas las conexiones establecidas.
