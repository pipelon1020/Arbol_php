Arbol PHP este codigo ejecuta una estructura de datos de clase Arbol

Parte 1
Cada nodo del árbol tiene tres componentes principales:
Valor: El dato que almacena el nodo (puede ser un número, texto, etc.)
Izquierda: Referencia al nodo hijo izquierdo (o null si no existe)
Derecha: Referencia al nodo hijo derecho (o null si no existe)
El constructor __construct($Valor) inicializa un nuevo nodo con el valor proporcionado y establece ambos hijos como nulos.

Parte 2
La clase ArbolBinario gestiona toda la estructura del árbol:
Raiz: Puntero al nodo raíz del árbol (el nodo superior de toda la estructura)
Al inicio, el árbol está vacío ($Raiz = null)

Operaciones principales
Insertar un valor
Se comienza desde la raíz
Si el árbol está vacío, el nuevo valor se convierte en la raíz
Si no, se compara el valor con el nodo actual:
Si es menor, se intenta insertar en el subárbol izquierdo
Si es mayor o igual, se intenta insertar en el subárbol derecho
Este proceso se repite recursivamente hasta encontrar una posición vacía

Recorridos del árbol:
InOrden: Visita primero el subárbol izquierdo, luego el nodo actual, y finalmente el subárbol derecho. Muestra los valores ordenados.
PreOrden: Visita primero el nodo actual, luego el subárbol izquierdo y finalmente el subárbol derecho. Muestra la estructura jerárquica.
PostOrden: Visita primero el subárbol izquierdo, luego el subárbol derecho, y finalmente el nodo actual. Útil para operaciones como eliminar nodos.
