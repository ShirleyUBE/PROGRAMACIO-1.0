#crea una matriz
def imprimir_matriz(matriz):
    for fila in matriz:
        for elemento in fila:
            print(elemento, end=" ")
        print()

def buscar_valor(matriz, valor):
    for i in range(len(matriz)):
        for j in range(len(matriz[0])):
            if matriz[i][j] == valor:
                return f"El valor {valor} se encuentra en la posición ({i}, {j})."
    return f"El valor {valor} no se encuentra en la matriz."

# Crear una matriz de 3x3 con valores numéricos
matriz = [
    [10, 20, 30],
    [44, 55, 66],
    [77, 88, 99]
]

# Imprimir la matriz
print("Matriz:")
imprimir_matriz(matriz)

# Buscar un valor en la matriz
valor_buscado = 55
resultado_busqueda = buscar_valor(matriz, valor_buscado)
print(resultado_busqueda)
