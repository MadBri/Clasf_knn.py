from sklearn.neighbors import KNeighborsClassifier


X = [[2, 0], [4, 4], [1, 0], [4, 1], [2, 2], [3, 1], [3, 4], [3, 1]]  # Coordenadas X1 y X2
y = [0, 1, 0, 1, 0, 1, 0, 1]  # Clases correspondientes

nuevo_caso = [[2.5, 2.5]]


clasificador_knn = KNeighborsClassifier(n_neighbors=1, metric='manhattan')

clasificador_knn.fit(X, y)

clase_predicha = clasificador_knn.predict(nuevo_caso)

print("El nuevo caso:", nuevo_caso[0], "pertenece a la clase:", clase_predicha[0])

git branch
git checkout main
git checkout -b main
git checkout -b experimental
git push -u origin experimental
