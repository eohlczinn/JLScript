# #api

**Nome:** API
**Versão:** 1.0.0
**Autor:** JLScript Team
**Categoria:** Rede
**Licença:** MIT

---

# Descrição

A biblioteca `#api` permite realizar requisições HTTP e consumir APIs REST.

---

# Instalação

```bash
jls lib install api
```

---

# Importação

```jls
import #api
```

## Com apelido

```jls
import #api como #ap
```

---

# Funções

## get()

```jls
va res = #api.get(url)
```

Descrição...

---

## post()

```jls
#api.post(url, dados)
```

Descrição...

---

## put()

...

---

# Objetos

## Response

```jls
res.status
res.body
res.headers
res.ok
```

---

# Exemplos

```jls
import #api

va res = #api.get(
    "https://api.site.com"
)

mostrar(res.body)
```

---

# Tratamento de erros

```jls
tente{

    ...

}
pegue(erro){

    mostrar(erro)

}
```

---

# Changelog

## 1.0.0

- Primeira versão.