# Busqueda-lineal-y-binaria
🔍 1. BÚSQUEDA LINEAL

💡 ¿Qué es?
Es un algoritmo que revisa cada elemento de una lista, uno por uno, hasta encontrar el valor buscado o llegar al final.

✅ ¿Cuándo usarla?
Cuando los datos NO están ordenados.

Cuando la lista es pequeña.

Cuando quieres una solución rápida de implementar.

🧠 Lógica:
Empiezas en el primer elemento.

Lo comparas con el valor que buscas.

Si lo encuentras, devuelves el índice.

Si no, sigues hasta el final.

⏱️ Complejidad:
Tiempo promedio y peor caso: O(n)

Espacio: O(1)

🧪 Ejemplo en Python:

def busqueda_lineal(lista, objetivo):

    for i in range(len(lista)):
    
        if lista[i] == objetivo:
        
            return i
            
    return -1

🔍 2. BÚSQUEDA BINARIA

💡 ¿Qué es?
Es un algoritmo más eficiente que funciona solo en listas ORDENADAS. Divide la lista en dos mitades y decide en cuál mitad continuar la búsqueda.

✅ ¿Cuándo usarla?
Cuando los datos están ordenados (ascendente o descendente).

Cuando la lista es grande y necesitas eficiencia.

🧠 Lógica:
Verifica el elemento en el medio de la lista.

Si es el valor buscado, devuelve el índice.

Si es mayor, repite la búsqueda en la mitad izquierda.

Si es menor, repite en la mitad derecha.

Continúa hasta encontrarlo o hasta que no haya más elementos.

⏱️ Complejidad:
Tiempo promedio y peor caso: O(log n)

Espacio: O(1) (versión iterativa) / O(log n) (versión recursiva por pila de llamadas)

🧪 Ejemplo en Python:
python

def busqueda_binaria(lista, objetivo):

    inicio = 0
    
    fin = len(lista) - 1

    while inicio <= fin:
    
        medio = (inicio + fin) // 2
        
        if lista[medio] == objetivo:
        
            return medio
            
        elif lista[medio] < objetivo:
        
            inicio = medio + 1
            
        else:
        
            fin = medio - 1
            

    return -1

Gracias por ver mi trabajo.
