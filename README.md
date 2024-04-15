# Árvore Binária Simples

Este repositório contém uma implementação simples de uma árvore binária em C++. Uma árvore binária é uma estrutura de dados hierárquica na qual cada nó tem no máximo dois filhos, conhecidos como filho esquerdo e filho direito.

## Estrutura do Nó

A estrutura `No` é definida com três membros:
- `int data`: Valor inteiro que o nó armazena.
- `No* esquerda`: Ponteiro para o filho esquerdo.
- `No* direita`: Ponteiro para o filho direito.

## Funções

### criarNo

```cpp
No* criarNo(int dado);
```
Cria um novo nó com o dado fornecido, inicializando os ponteiros dos filhos como `nullptr`.

### imprimir

```cpp
void imprimir(No* root);
```
Realiza uma travessia in-order da árvore e imprime os dados de cada nó.

## Uso

Para usar este código, crie uma instância da árvore e insira os nós desejados. Por exemplo:

```cpp
int main() {
    No* root = criarNo(10);
    root->direita = criarNo(5);
    root->esquerda = criarNo(4);
    
    imprimir(root);
    
    return 0;
}
```

Este exemplo cria uma árvore com um nó raiz contendo o valor 10 e dois filhos com valores 5 e 4, respectivamente.
