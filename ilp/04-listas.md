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

- A lista é representada entre `[` e `]`, e seus elementos são separados por vírgulas (`,`)
   - Lista vazia: `[]`
   - Uma lista com 1 elemento: `[10]`
   - Uma lista com 2 elementos: `[10,20]`
   - Uma lista com 3 elementos de tipos diferentes: ```['Maria', 10, 20.0]```

---

# Inicialização de listas

- Exemplos

```python
vazia = []
notas = [9.8, 7.5, 8.3]
nomes = ['Fulano', 'Sicrana', 'Beltrana']
notasenomes = [notas, nomes]
usuarios = [['usuario', 'senha'], ['admin', '123']]
```

--- 

# Inicialização com repetição
 
- Operador "\*":  usado para criar uma lista maior a partir da repetição dos elementos de uma lista menor.

```
>>> [0] * 4
[0,0,0,0]

>>> ['a', 'b'] * 2
[ 'a', 'b', 'a', 'b']
```

---

# Comprimento da lista (len)

Use a função `len(x)` para obter o comprimento de uma lista `x`.

```
>>> lista = [2,2,2,2]
>>> print(lista)
[2, 2, 2, 2]
>>> len(lista)
4
``` 

---

# Índices: acesso a elementos da lista

- Cada elemento da lista possui um **índice** (ou **posição**):
   - o primeiro elemento possui índice 0
   - o segundo elemento possui índice 1
   - o terceiro elemento possui índice 2
e assim por diante.

- Uma lista `L` possui tamanho `len(L)` e os índices variam de 0 até `len(L)-1`

---

# Acesso a elementos da lista

Para acessar o elemento `i` de uma lista `L`, onde `i` varia de 0 até `len(L)-1`, use `L[i]`:

```python
x = ['a', 'b', 'c']
print(x[0])
print(x[1])
print(x[2])
print(x[3])   # IndexError: list index out of range
```

---

# Atribuição múltipla

Se o número de elementos de uma lista for conhecido, 
pode-se usar uma atribuição com diversas variáveis.

```python
lista = [2, 4, 6]
x, y, z = lista     # sabe-se que a lista possui 3 elementos
```

Se o número de variáveis do lado esquerdo do símbolo `=` não coincidir com 
o número de elementos da lista, o erro `ValueError` será reportado.

---

# Alteração de valor de elemento da lista

Pode-se alterar um elemento da lista realizando uma atribuição:

```python
x = ['a', 'b', 'c']  # lista original com 3 elementos
x[0] = 'Z'   # modifica apenaso valor  do primeiro elemento da lista
x[3] = 'W'   # IndexError: list assignment index out of range
```

--- 

# split(): retorna uma lista de strings

- Considere a entrada ```a b c```, 
com três caracteres separados por " ".

```python
>>> letras = input().split()
a b c
>>> letras
['a', 'b', 'c']
```

---

template: inverse
# Operações sobre Listas

Sugestão: Visualizar operações sobre listas usando o [PythonTutor](https://pythontutor.com/)


{:/}



