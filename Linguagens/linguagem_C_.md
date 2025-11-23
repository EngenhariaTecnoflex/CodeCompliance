# Linguagem de programação C

[TOC]

---

## Variáveis

1. **Tipos padrão**
Tipos padrão (int, double, char ...) devem ser **evitados**.
Como alternativa é **desejável** o uso dos tipos padronizados na biblioteca <stdint.h> e <stdbool.h> (uint16_t, int8_t, uint8_t)

1. **Tipos definidos**
Tipos definidos pelo desenvolvedor deverão **obrigatoriamente** ser finalizados com o sufixo "_t" ou "_h". Sufixos terminados por "_t" são destinados a tipos alocados diretamente na declaração da variável. Já o sufixo "_h" é destinado à ponteiros (handlers) e usualmente apontam para uma variável de tipo "_t". Como no exemplo:

    ```C
    typedef struct mystruct_{
        uint16_t u16Myint;
        int32_t  i32MyOtherInt;
    }mystruct_t;

    typedef mystruct_t *mystruct_h;

    ```

1. **Inicialização**

1. **Nomenclatura**

1. **Comentários**

1. **Constantes**

1. **Objetos**

---

## Funções

---

## Alocação dinâmica

---

## Compiladores

---

## Identação

---

## Warnings e Erros

---

## Comentários

---

## Acesso ao hardware

---
