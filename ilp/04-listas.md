---
layout: remark
title:
---

{::nomarkdown}
template: inverse

# Listas em Python

{% include_relative footer.txt %}

---

# Motivação

Suponha que você precisa ler 5 números e escrevê-los na ordem inversa:

```python
# Lê 5 números
a, b, c, d, e = map(float, input().split())

# Imprime na ordem inversa
print(e)
print(d)
print(c)
print(b)
print(a)
```
- E se fossem 10 mil números?

---

# Listas

A **lista** é um tipo de dados usado para armazenar coleções de dados.

- Listas podem conter 0, 1 ou mais elementos
   - **tamanho** da lista
- Uma lista com 0 elementos é chamada de **lista vazia**
- Os elementos da lista podem ser de tipos diferentes:
   - Por exemplo, uma lista pode conter um elemento do tipo `str`, um elemento do tipo `int` e um elemento do tipo `float` 
- Elementos da lista podem ser outras listas
- É possível *adicionar* elementos ou *remover* elementos de listas.

---

# Listas (Python)

- A lista é representada entre `[` e `]', e seus elementos são separados por vírgulas (`,`)/
   - Lista vazia: `[]`
   - Uma lista com 1 elemento: `[10]`
   - Uma lista com 2 elementos: `[10,20]`
   - Uma lista com 3 elementos de tipos diferentes: `["Maria", 10, 20.0]`

---

# Inicialização 

- vazia = []
- notas = [9.8, 7.5, 8.3]
- nomes = ["Fulano", "Sicrana", "Beltrana"]
- notas_nomes = [notas, nomes]
- usuarios = [["usuario", "senha"], ["admin", "123"]]

--- 

# Inicialização
 
- Operador "*":  usado para criar uma lista maior a partir da repetição dos elementos de uma lista menor.

```python
>>> [0] * 4
[0,0,0,0]

>>> ["a", "b"] * 2
[ 'a', 'b', 'a', 'b']
```

{:/}



