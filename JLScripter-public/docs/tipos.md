# 🏷️ Tipos de Dados - JLScript

Os tipos de dados definem qual informação uma variável pode armazenar. A JLScript possui tipos simples, intuitivos e fáceis de utilizar.

---

# String

Armazena textos.

```jls
let nome = "Lucas";
```

Também pode utilizar aspas simples.

```jls
let linguagem = 'JLScript';
```

---

# Integer (int)

Armazena números inteiros.

```jls
let idade = 19;
```

Exemplos

```jls
0
10
-25
999
```

---

# Float

Armazena números com casas decimais.

```jls
let altura = 1.75;
```

Exemplos

```jls
3.14
0.5
-12.75
```

---

# Boolean

Representa verdadeiro ou falso.

```jls
let ativo = true;
```

```jls
let desligado = false;
```

---

# Null

Representa a ausência de valor.

```jls
let usuario = null;
```

---

# Array

Armazena vários valores em uma única variável.

```jls
let numeros = [1, 2, 3];
```

Também pode conter textos.

```jls
let nomes = [
    "Lucas",
    "João",
    "Maria"
];
```

---

# Object (Planejado)

Armazena informações em formato de chave e valor.

```jls
let pessoa = {

    nome: "Lucas",
    idade: 19

};
```

---

# Conversão de Tipos

Converter para inteiro.

```jls
int("10");
```

Converter para decimal.

```jls
float("10.5");
```

Converter para texto.

```jls
str(10);
```

Converter para booleano.

```jls
bool(1);
```

---

# Descobrindo o Tipo

Utilize `tipo()` para descobrir o tipo de um valor.

```jls
let nome = "Lucas";

mostrar(tipo(nome));
```

Saída

```text
string
```

---

# Exemplos

```jls
let nome = "Lucas";

let idade = 19;

let altura = 1.75;

let estudante = true;

let endereco = null;

let notas = [10, 9, 8];
```

---

# Tabela de Tipos

| Tipo | Descrição | Exemplo |
|------|-----------|----------|
| string | Texto | `"Olá"` |
| int | Número inteiro | `10` |
| float | Número decimal | `3.14` |
| bool | Verdadeiro ou falso | `true` |
| null | Sem valor | `null` |
| array | Lista de valores | `[1,2,3]` |
| object | Chave e valor *(Planejado)* | `{ nome: "Lucas" }` |

---

# Boas Práticas

- Utilize **string** para textos.
- Utilize **int** para números inteiros.
- Utilize **float** para números decimais.
- Utilize **bool** para decisões lógicas.
- Utilize **array** para armazenar coleções de dados.
- Utilize **null** quando uma variável ainda não possuir valor.

---

> Os tipos da **JLScript** foram projetados para serem simples e familiares, inspirados em linguagens como JavaScript, Python e C++, mantendo uma sintaxe limpa e intuitiva.