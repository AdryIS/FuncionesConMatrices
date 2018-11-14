# FuncionesConMatrices

Las matrices son espacios contíguos de memoria, en los cuales se puede acceder a un elemento deseado utilizando la posición del elemento.
Usar funciones en forma de matrices, nos ayuda a obtener cosas como la suma entre estás funciones, multiplicación, obtener la menor, determinante, la adyacente, transpuesta o inversa.

En el código se convierte una función en matriz, con los coeficientes de las funciones a crear.
Antes de crear la matriz, se debe de tener en cuenta lo que se puede hacer y a partir de esta decisión se resuelve la matriz

Suma:
  Con las dimensiones de las matrices, se checa primero que se puedan sumar, si no tienen las mismas dimensiones no se puede resolver
  Si se tienen las mismas dimensiones, se crea una matriz a partir de estas y se entra a un loop que suma cada número con la segunda 
  matriz tomando en cuenta la posición y el orden
  
Multiplicación:
  Al igual que la suma, con las dimensiones se checa si se puede resolver la multiplicación
  Si se tienen las mismas dimensiones, se crea una matriz a partir de estas y se entra a un loop que multiplica cada número con la segunda 
  matriz tomando en cuenta la posición y el orden
  
Obtener el menor valor:
  Primero se checan los valores de la matriz y si uno de los valores es igual 

Determinante:
  Este nos permite solucionar un sistema de ecuaciones
  Si la matriz es diagonal, el determinante es el producto de los elementos de la diagonal
  Primero se comprueba que la matriz no sea cuadrada con la longitud de esta
  Si la longitud de la matriz es 1 se regresa la longitud
  Si es de 2 se multiplican las matrices A[0][0] * A[1][1] y se restan con la mutltiplicacion de A[0][1] * A[1][0]
  La determinante se obtiene con la fórmual escrita en el código y aquí: det += (-1)^(j) * A[0][j] * detMatriz(getMenorMatriz(A,0,j))
  
Adyacente:
  A partir de la dimensiones de la matriz, se va recorriendo estas y crean una nueva matriz a partir de la siguiente fórmula en la que C 
  es nuestra nueva matriz : C[i][j] = (-1)^(i+j) * detMatriz(getMenorMatriz(A,i,j))
  
Transpuesta:
  Esta matriz se obtiene cambiando ordenadamente las filas por las columnas de la matriz
  Se recorre la matriz y se van agregando los valores de esta a la nueva matriz de manera horizontal
  
Inversa:
  
