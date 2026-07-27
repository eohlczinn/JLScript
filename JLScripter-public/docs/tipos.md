# Tipos de dados JLScript

Os tipos de dados definem quais valores uma variável pode armazenar.

No JLScript, as variáveis possuem tipagem dinâmica, isso significa que o
interpretador identifica o tipo automaticamente pelo valor recebido.

Exemplo:

jls

va idade = 19

O interpretador entende que:

idade → número
Número (Number)

Representa valores numéricos.

Pode ser usado para:

cálculos;
contagens;
operações matemáticas.

Exemplo:

# va idade = 19
# va altura = 1.75

Valores:

idade = 19
altura = 1.75

Operações:

va soma = 10 + 5
mostrar(soma)

Resultado:

15
Texto (String)

Representa uma sequência de caracteres.

Textos devem estar entre aspas.

Exemplo:

va nome = "Lucas"

O valor armazenado é:

nome → "Lucas"

Pode ser usado para:

nomes;
mensagens;
textos.

Exemplo:

mostrar("Olá mundo")

Saída:

Olá mundo
Booleano (Boolean)

Representa valores de verdadeiro ou falso.

Possui dois valores:

verdadeiro
falso

Exemplo:

va ligado = verdadeiro

O interpretador guarda:

ligado → true

Muito usado em condições:

va maior = verdadeiro

se maior
{
    mostrar("Sim")
}
Nulo (Null)

Representa ausência de valor.

É usado quando uma variável existe, mas ainda não possui informação.

Exemplo:

va resultado = nulo

Estado:

resultado → vazio
Array (Lista)

Arrays armazenam vários valores dentro de uma única variável.

Exemplo:

va numeros = [1,2,3,4]

Representação:

numeros

[
  1
  2
  3
  4
]

Podem armazenar vários tipos:

va dados = [
    "Lucas",
    19,
    verdadeiro
]
Objeto

Objetos armazenam informações organizadas em propriedades.

Exemplo:

va pessoa =
{
    nome: "Lucas",
    idade: 19
}

Representação:

pessoa

nome → Lucas
idade → 19

Objetos permitem criar estruturas mais complexas.

Função

Funções também podem ser consideradas valores.

Elas armazenam blocos de código que podem ser executados.

Exemplo:

funcao mensagem()
{
    mostrar("Olá")
}

A função pode ser chamada:

mensagem()
Conversão de tipos

Em alguns casos pode ser necessário transformar um tipo em outro.

Exemplo:

Número para texto:

19
↓
"19"

Texto para número:

"50"
↓
50

Essas conversões serão realizadas através das funções da biblioteca padrão.

Resumo dos tipos
Tipo	Exemplo	Uso
Number	10	números e cálculos
String	"Olá"	textos
Boolean	verdadeiro	decisões
Null	nulo	ausência de valor
Array	[1,2,3]	listas
Object	{nome:"Ana"}	dados organizados
Function	funcao(){}	código reutilizável
Tipos internos do interpretador

Internamente o JLScript representa esses valores através do sistema de runtime.

Local:

src/runtime/

Arquivos relacionados:

value.hpp
value.cpp
object.hpp
object.cpp

O runtime é responsável por armazenar e manipular os valores durante a execução do programa.


---


---

Uma observação importante: pelo código que você mostrou antes, seu `Value` provavelmente ainda está nos tipos básicos (`number`, `string`, `boolean` etc.). Então **Array, Object e Function podem ficar documentados como recursos planejados** até você implementar no runtime. Melhor uma documentação menor e verdadeira do que uma enciclopédia de coisas que o interpretador ainda olha e fala "não faço ideia do que é isso". 😄