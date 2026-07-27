# 📚 Funções - JLScript

As funções permitem organizar o código em blocos reutilizáveis, tornando os programas mais limpos, fáceis de manter e reutilizar.

---

# Criando uma função

Utilize a palavra-chave `func`.

```jls
func ola() {
    mostrar("Olá, Mundo!");
}
```

---

# Chamando uma função

Após criada, basta utilizar seu nome.

```jls
ola();
```

Saída:

```text
Olá, Mundo!
```

---

# Parâmetros

As funções podem receber valores.

```jls
func saudacao(nome) {
    mostrar("Olá " + nome);
}

saudacao("Lucas");
```

Saída:

```text
Olá Lucas
```

---

# Múltiplos parâmetros

```jls
func soma(a, b) {
    mostrar(a + b);
}

soma(10, 20);
```

Saída:

```text
30
```

---

# Retornando valores

Utilize `retorne`.

```jls
func soma(a, b) {
    retorne a + b;
}

let resultado = soma(5, 3);

mostrar(resultado);
```

Saída:

```text
8
```

---

# Retorno antecipado

A função pode finalizar antes utilizando `retorne`.

```jls
func verificar(idade) {

    se (idade < 18) {
        retorne "Menor de idade";
    }

    retorne "Maior de idade";
}

mostrar(verificar(20));
```

---

# Funções sem parâmetros

```jls
func dataAtual() {
    mostrar("27/07/2026");
}

dataAtual();
```

---

# Escopo

Variáveis criadas dentro da função existem apenas nela.

```jls
func teste() {

    let nome = "Lucas";

    mostrar(nome);

}
```

Após a função terminar, `nome` deixa de existir.

---

# Exemplo completo

```jls
func calcularIMC(peso, altura) {

    let imc = peso / (altura * altura);

    retorne imc;

}

let resultado = calcularIMC(70, 1.75);

mostrar(resultado);
```

---

# Boas práticas

- Dê nomes claros às funções.
- Cada função deve possuir apenas uma responsabilidade.
- Evite funções muito grandes.
- Utilize `retorne` sempre que precisar devolver um resultado.
- Reutilize funções para evitar repetir código.

---

# Resumo

| Sintaxe | Descrição |
|---------|-----------|
| `func nome(){}` | Cria uma função |
| `nome();` | Executa uma função |
| `func soma(a,b){}` | Função com parâmetros |
| `retorne valor;` | Retorna um valor |
| `let x = soma();` | Armazena o retorno |

---

## Exemplo final

```jls
func dobro(numero) {

    retorne numero * 2;

}

let valor = dobro(10);

mostrar(valor);
```

Saída:

```text
20
```

---

> **JLScript** foi criada para ser uma linguagem simples, intuitiva e acessível, permitindo que iniciantes aprendam programação com uma sintaxe clara e em português.