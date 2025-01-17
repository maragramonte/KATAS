FUNCION distinct(array: LISTA DE ENTEROS) RETORNA LISTA DE ENTEROS
    DECLARAR seen COMO CONJUNTO DE ENTEROS
    DECLARAR resultList COMO LISTA DE ENTEROS

    PARA CADA num EN array HACER
        SI num NO ESTÁ EN seen ENTONCES
            AGREGAR num A seen
            AGREGAR num A resultList
        FIN SI
    FIN PARA

    DECLARAR result COMO LISTA DE ENTEROS CON TAMAÑO IGUAL A tamaño DE resultList
    PARA i DESDE 0 HASTA tamaño DE resultList - 1 HACER
        result[i] = resultList[i]
    FIN PARA

    RETORNAR result
FIN FUNCION

Desglose del Pseudocódigo
Definición de la Función:

FUNCION distinct(array: LISTA DE ENTEROS) RETORNA LISTA DE ENTEROS: Se define una función llamada distinct que toma como parámetro una lista de enteros (array) y devuelve una lista de enteros.
Inicialización de Estructuras:

DECLARAR seen COMO CONJUNTO DE ENTEROS: Se crea un conjunto llamado seen que se utilizará para almacenar los números que ya han sido encontrados. Un conjunto es útil aquí porque no permite duplicados.
DECLARAR resultList COMO LISTA DE ENTEROS: Se crea una lista llamada resultList que almacenará los números únicos que se encuentren en el arreglo original.
Iteración sobre el Arreglo:

PARA CADA num EN array HACER: Se inicia un bucle que recorre cada número (num) en el arreglo de entrada (array).
SI num NO ESTÁ EN seen ENTONCES: Se verifica si el número actual (num) ya ha sido visto (es decir, si ya está en el conjunto seen).
AGREGAR num A seen: Si el número no ha sido visto, se agrega al conjunto seen.
AGREGAR num A resultList: También se agrega a la lista resultList, ya que es un número único.
Creación del Arreglo de Resultado:

DECLARAR result COMO LISTA DE ENTEROS CON TAMAÑO IGUAL A tamaño DE resultList: Se crea un nuevo arreglo llamado result que tendrá el mismo tamaño que resultList, para almacenar los números únicos.
PARA i DESDE 0 HASTA tamaño DE resultList - 1 HACER: Se inicia otro bucle que recorre los índices de resultList.
result[i] = resultList[i]: Se copia cada elemento de resultList al arreglo result.
Retorno del Resultado:

RETORNAR result: Finalmente, la función devuelve el arreglo result, que contiene solo los números únicos del arreglo original.