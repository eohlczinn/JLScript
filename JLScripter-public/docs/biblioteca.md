# 📚 Bibliotecas na JLScript

As bibliotecas permitem adicionar novas funcionalidades aos seus projetos de forma simples e organizada.

---

# Importando uma biblioteca

Use o comando `import` seguido do nome da biblioteca.

```jls
import #api
```

---

# Importando com apelido

É possível criar um apelido para facilitar o uso da biblioteca.

```jls
import #api como #ap
```

ou

```jls
import #api ap #ap
```

Após a importação:

```jls
#ap.get("https://api.exemplo.com")
```

---

# Regra do caractere #

Toda biblioteca na JLScript deve utilizar o prefixo `#`.

Exemplos:

```jls
import #api
import #json
import #math
import #file
```

O mesmo vale para apelidos.

```jls
import #api como #ap
```

Uso:

```jls
#ap.get(...)
```

Essa regra evita conflitos entre bibliotecas, variáveis, funções e classes.

---

# Instalando bibliotecas

```bash
jls lib install api
```

Atualizar:

```bash
jls lib update api
```

Atualizar todas:

```bash
jls lib update
```

Remover:

```bash
jls lib uninstall api
```

Listar bibliotecas instaladas:

```bash
jls lib list
```

---

# Bibliotecas oficiais

A JLScript possui bibliotecas oficiais desenvolvidas e mantidas pelo projeto.

Exemplos:

- `#api`
- `#json`
- `#math`
- `#file`
- `#time`
- `#crypto`
- `#os`
- `#http`

---

# Bibliotecas da comunidade

Também é possível instalar bibliotecas criadas pela comunidade através do gerenciador de pacotes da JLScript.

Exemplo:

```bash
jls lib install minha-biblioteca
```

Importação:

```jls
import #minha-biblioteca
```

---

# Boas práticas

- Utilize nomes curtos e descritivos.
- Sempre utilize o prefixo `#`.
- Utilize apelidos apenas quando necessário.
- Evite criar bibliotecas com nomes já utilizados pelas bibliotecas oficiais.
- Mantenha sua biblioteca documentada e versionada.

---

# Exemplo completo

```jls
import #api como #ap

va resposta =
    #ap.get(
        "https://api.exemplo.com/users"
    )

mostrar(resposta.body)
```

---

© JLScript Team