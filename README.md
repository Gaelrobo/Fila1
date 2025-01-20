# Fila1

#include <stdio.h>
#include <stdlib.h>
#include <stdbool.h>

typedef struct nodo {
    int info;
    struct nodo *prox;
} NODO;

typedef struct {
    NODO *ini;
    NODO *fim;
    int tam;
} Fila;

void inic_fila(Fila *F) {
    F->ini = F->fim = NULL;
    F->tam = 0;
}

bool fila_vazia(Fila *F) {
    return (F->tam == 0);
}
