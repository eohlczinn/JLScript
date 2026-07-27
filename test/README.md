# Testes da JLScript

Os testes da JLScript têm como objetivo verificar se todos os recursos da linguagem estão funcionando corretamente após alterações no interpretador, parser, lexer ou runtime.

## Estrutura

A pasta `examples/` contém exemplos que também servem como testes da linguagem.

```
examples/
├── olamundo.jls
├── variaveis.jls
├── funcoes.jls
├── condicoes.jls
├── loops.jls
├── api.jls
├── biblioteca.jls
```

## Executando um teste

Para executar um arquivo:

```bash
jls run examples/olamundo.jls
```

Ou:

```bash
jls run examples/variaveis.jls
```

## O que deve ser testado

### Saída

Verifique se os valores exibidos no terminal estão corretos.

### Erros

Confirme que erros de sintaxe e execução exibem mensagens claras.

### Performance

Verifique se loops, funções e operações executam corretamente sem lentidão inesperada.

### Compatibilidade

Teste em diferentes sistemas operacionais suportados pela JLScript.

## Adicionando novos testes

Sempre que um novo recurso for implementado, adicione um arquivo de exemplo na pasta `examples/`.

Exemplo:

```
classes.jls
```

```
arrays.jls
```

```
modulos.jls
```

```
threads.jls
```

## Boas práticas

- Um arquivo deve testar apenas um recurso principal.
- Use nomes simples e descritivos.
- Inclua comentários explicando cada exemplo.
- Evite misturar muitos recursos em um único teste.

## Objetivo

Os exemplos da JLScript funcionam como documentação e testes ao mesmo tempo. Assim, qualquer usuário pode aprender a linguagem enquanto verifica que seus recursos estão funcionando corretamente.