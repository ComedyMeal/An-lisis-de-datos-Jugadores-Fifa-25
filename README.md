Proyecto de aprendizaje no supervisado que busca clasificar los jugadores del popular juego FC25 (FIFA) en 4 clusters que son los más óptimos según el método del codo, usando el algoritmo k-menas con 4 variantes del mismo, aplicando 3 tipos de métricas diferentes para medir la similitud (mahalanobis, Euclidiana y L1). Se hace la visualización usando PCA.

Descripción del grupo de datos()
Se hace un EDA: análisis

-Se hizo un análisis exploratorio de los datos FC25 borrando los que no son necesarios para el análisis, en otras palabras los datos que no son numéricos, aunque cogimos la base de datos de unos datos ya organizados asi que el trabajo fue más fácil.

-Se imputan los datos faltantes, se codifica la variable pie preferido a una variable binaria.

-Implementación del k-means usando librerías.

-implementación manual del algoritmo usando 3 tipos de distancias diferentes (mahalanobis, Euclidiana y L1) .

- el algoritmo k-means trata de agrupar los datos por su similitud con elementos muy similares entre si, el algoritmo define esta similitud cuando hay poca distancia entre ellos, el algoritmo primero escoge la cantidad de clusters(método del codo), luego se escogen los centroides y se asignan los puntos a los centroides más cercanos según el (método utilizado) y se evalúa la calidad de los clusters, se recalculan los centroides y se vuelve a repetir hasta que los cambios de los datos sean mínimos.

-se usa PCA (reducción de dimensionalidad), para visualizar la clusterizacion en 2D y 3D. Se escogen 4 componentes principales que conservan el 80% de la varianza de los datos, los centroides se transforman en dicho espacio para poderlos visualizar.
