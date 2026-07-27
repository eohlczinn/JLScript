# 📝 Sintaxe - JLScript

A sintaxe da **JLScript** foi projetada para ser simples, intuitiva e fácil de aprender, utilizando palavras em português sempre que possível.

---

# Olá Mundo

```jls
mostrar("Olá, Mundo!");
```

---

# Comentários

Comentário de uma linha:

```jls
// Isto é um comentário
```

Comentário de múltiplas linhas:

```jls
/*
Comentário
de várias
linhas
*/
```

---

# Variáveis

Variável mutável:

```jls
let nome = "Lucas";
```

Outra forma de variável:

```jls
va idade = 19;
```

Constante:

```jls
ins PI = 3.14159;
```

---

# Tipos de dados

```jls
let texto = "Olá";

let numero = 10;

let decimal = 10.5;

let ativo = true;

let vazio = null;
```

---

# Operadores

## Matemáticos

```jls
+
-
*
/
%
**
```

Exemplo:

```jls
mostrar(10 + 5);
```

---

## Comparação

```jls
==
!=
>
<
>=
<=
```

---

## Lógicos

```jls
&&
||
!
```

---

# Entrada e saída

Mostrar informações:

```jls
mostrar("Olá");
```

Receber entrada:

```jls
let nome = chat("Digite seu nome:");
```

---

# Condições

```jls
se (idade >= 18) {

    mostrar("Maior de idade");

}
```

---

## Senão

```jls
se (idade >= 18) {

    mostrar("Maior");

} senao {

    mostrar("Menor");

}
```

---

## Senão se

```jls
se (nota >= 9) {

    mostrar("Excelente");

} senao se (nota >= 6) {

    mostrar("Aprovado");

} senao {

    mostrar("Reprovado");

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

# Laço enquanto

```jls
enquanto(i < 10){

    mostrar(i);

    i++;

}
```

---

# Laço repita

```jls
repita(let i = 0; i < 10; i++){

    mostrar(i);

}
```

---

# Funções

```jls
func soma(a, b){

    retorne a + b;

}
```

Chamando:

```jls
let resultado = soma(5, 10);

mostrar(resultado);
```

---

# Importação

Importar biblioteca:

```jls
import #math;
```

Importar com apelido:

```jls
import #panda as #pd;
```

---

# Conversões

```jls
int(valor);

float(valor);

str(valor);

bool(valor);
```

---

# Arrays (Planejado)

```jls
let numeros = [1,2,3];
```

Métodos planejados:

```jls
numeros.adicionar(10);

numeros.remover();

numeros.inserir(1, 50);

numeros.removerEm(0);

numeros.tamanho();

numeros.limpar();

numeros.contem(5);

numeros.indiceDe(3);

numeros.inverter();

numeros.ordenar();
```

---

# Estrutura de um programa

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

- Utilize nomes descritivos.
- Finalize instruções com `;`.
- Utilize indentação de 4 espaços.
- Organize funções em arquivos separados quando o projeto crescer.
- Prefira constantes (`ins`) para valores que não mudam.

---

# Resumo

| Elemento | Sintaxe |
|----------|---------|
| Variável | `let nome = "";` |
| Constante | `ins PI = 3.14;` |
| Mostrar | `mostrar();` |
| Entrada | `chat();` |
| Função | `func nome(){}` |
| Retorno | `retorne` |
| Se | `se` |
| Senão | `senao` |
| Enquanto | `enquanto` |
| Repita | `repita` |
| Import | `import #biblioteca;` |

---

> **JLScript** possui uma sintaxe moderna, legível e inspirada em linguagens como JavaScript, Python e C++, adaptada para o português e voltada à produtividade e ao aprendizado.