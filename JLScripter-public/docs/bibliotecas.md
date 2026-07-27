# 🌍 Bibliotecas Open Source

A JLScript incentiva a criação e o compartilhamento de bibliotecas open source pela comunidade.

Qualquer desenvolvedor pode criar, publicar e manter bibliotecas compatíveis com a JLScript.

---

# Objetivo

As bibliotecas permitem expandir as funcionalidades da linguagem sem modificar seu núcleo.

Elas podem ser utilizadas em projetos pessoais, comerciais ou educacionais.

---

# Publicando uma biblioteca

Após desenvolver sua biblioteca, publique-a em um repositório Git (como GitHub) e registre-a no gerenciador de pacotes da JLScript.

Exemplo:

```bash
jls lib publish
```

---

# Instalando

```bash
jls lib install nome-da-biblioteca
```

---

# Importando

```jls
import #nome-da-biblioteca
```

Com apelido:

```jls
import #nome-da-biblioteca como #lib
```

---

# Estrutura recomendada

```
minha-biblioteca/
├── src/
├── examples/
├── tests/
├── README.md
├── LICENSE
├── manifest.json
└── CHANGELOG.md
```

---

# Manifesto

Toda biblioteca deve possuir um arquivo `manifest.json`.

Exemplo:

```json
{
  "name": "minha-biblioteca",
  "version": "1.0.0",
  "author": "Seu Nome",
  "description": "Descrição da biblioteca.",
  "license": "MIT"
}
```

---

# Licença

Escolha uma licença open source compatível, como:

- MIT
- Apache 2.0
- BSD-3-Clause
- GPL-3.0

---

# Boas práticas

- Escreva código limpo.
- Documente todas as funções.
- Utilize versionamento semântico.
- Adicione exemplos de uso.
- Escreva testes sempre que possível.
- Evite quebrar compatibilidade entre versões.

---

# Comunidade

Contribuições são bem-vindas.

Toda biblioteca publicada ajuda a fortalecer o ecossistema da JLScript e beneficia toda a comunidade.

---

**Desenvolvido para a comunidade. Compartilhado com a comunidade.**