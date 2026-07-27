# 📝 Sintaxe - JLScript

A **JLScript** foi criada para ser uma linguagem simples, moderna e intuitiva. Ela permite escrever código em **português** ou **inglês**, facilitando tanto para iniciantes quanto para programadores experientes.

---

# Idiomas da Sintaxe

A JLScript possui duas sintaxes oficiais.

## Português

```jls
se (idade >= 18) {

    mostrar("Maior de idade");

} senao {

    mostrar("Menor de idade");

}
```

## Inglês

```jls
if (idade >= 18) {

    print("Maior de idade");

} else {

    print("Menor de idade");

}
```

---

# Regras

Você pode utilizar **português** ou **inglês**, porém **não pode misturar os dois na mesma estrutura**.

### Correto

```jls
se (ativo) {

    mostrar("OK");

} senao {

    mostrar("Erro");

}
```

```jls
if (ativo) {

    print("OK");

} else {

    print("Erro");

}
```

### Incorreto

```jls
if (ativo) {

    print("OK");

} senao {

    print("Erro");

}
```

```jls
se (ativo) {

    mostrar("OK");

} else {

    mostrar("Erro");

}
```

> Misturar palavras-chave de idiomas diferentes gera erro de sintaxe.

---

# Comentários

Comentário de uma linha

```jls
// Comentário
```

Comentário de múltiplas linhas

```jls
/*
Comentário
de várias
linhas
*/
```

---

# Variáveis

Variável mutável

```jls
let nome = "Lucas";
```

Outra variável mutável

```jls
va idade = 19;
```

Constante

```jls
ins PI = 3.14159;
```

---

# Tipos de Dados

```jls
let texto = "Olá";

let numero = 10;

let decimal = 10.5;

let ativo = true;

let vazio = null;
```

---

# Operadores Matemáticos

```text
+
-
*
/
%
**
```

Exemplo

```jls
mostrar(10 + 5);
```

---

# Operadores de Comparação

```text
==
!=
>
<
>=
<=
```

---

# Operadores Lógicos

```text
&&
||
!
```

---

# Entrada e Saída

Mostrar informações

```jls
mostrar("Olá Mundo");
```

```jls
print("Olá Mundo");
```

Receber entrada

```jls
let nome = chat("Digite seu nome:");
```

```jls
let nome = input("Digite seu nome:");
```

---

# Condições

Português

```jls
se (idade >= 18) {

    mostrar("Maior");

}
```

Inglês

```jls
if (idade >= 18) {

    print("Maior");

}
```

---

# Condição Completa

Português

```jls
se (nota >= 9) {

    mostrar("Excelente");

} senao se (nota >= 6) {

    mostrar("Aprovado");

} senao {

    mostrar("Reprovado");

}
```

Inglês

```jls
if (nota >= 9) {

    print("Excelente");

} else if (nota >= 6) {

    print("Aprovado");

} else {

    print("Reprovado");

}
```

---

# Switch

```jls
switch(opcao){

    case 1:
        mostrar("Um");
        break;

    case 2:
        mostrar("Dois");
        break;

    default:
        mostrar("Outro");

}
```

---

# Laço While

Português

```jls
enquanto(i < 10){

    mostrar(i);

    i++;

}
```

Inglês

```jls
while(i < 10){

    print(i);

    i++;

}
```

---

# Laço For

Português

```jls
repita(let i = 0; i < 10; i++){

    mostrar(i);

}
```

Inglês

```jls
for(let i = 0; i < 10; i++){

    print(i);

}
```

---

# Funções

Português

```jls
func soma(a, b){

    retorne a + b;

}
```

Inglês

```jls
function soma(a, b){

    return a + b;

}
```

Chamando

```jls
let resultado = soma(10, 5);

mostrar(resultado);
```

---

# Importação

```jls
import #math;
```

Com apelido

```jls
import #panda as #pd;
```

---

# Conversão de Tipos

```jls
int(valor);

float(valor);

str(valor);

bool(valor);
```

---

# Arrays (Planejado)

```jls
let numeros = [1, 2, 3];
```

Exemplos

```jls
numeros.adicionar(10);

numeros.remover();

numeros.inserir(1, 50);

numeros.removerEm(0);

numeros.tamanho();

numeros.limpar();

numeros.contem(5);

numeros.indiceDe(5);

numeros.inverter();

numeros.ordenar();
```

---

# Estrutura de um Programa

```jls
import #math;

func principal(){

    let nome = chat("Digite seu nome:");

    mostrar("Olá " + nome);

}

principal();
```

---

# Convenções

- Utilize indentação de 4 espaços.
- Finalize instruções com `;`.
- Escolha apenas um idioma por estrutura.
- Utilize nomes descritivos para variáveis e funções.
- Organize o código em funções para facilitar a manutenção.

---

# Palavras-chave

| Português | Inglês |
|-----------|---------|
| se | if |
| senao | else |
| senao se | else if |
| enquanto | while |
| repita | for |
| func | function |
| retorne | return |
| mostrar | print |
| chat | input |

---

> **JLScript** combina a simplicidade do português com a compatibilidade da sintaxe tradicional, permitindo escrever código da forma que você preferir, desde que cada estrutura utilize apenas um dos idiomas.