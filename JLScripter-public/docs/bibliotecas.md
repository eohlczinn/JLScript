# Biblioteca padrão JLScript

A biblioteca padrão do JLScript contém recursos que já vêm incluídos
na linguagem.

Ela permite realizar tarefas comuns sem precisar criar tudo do zero.

As bibliotecas podem ser importadas usando:

```jls
importar nome_da_biblioteca
Console

Biblioteca responsável por interação com o terminal.

Arquivo interno:

src/std/console.cpp
Funções
mostrar()

Exibe informações na tela.

Exemplo:

mostrar("Olá JLScript")

Saída:

Olá JLScript
Math

Biblioteca de operações matemáticas.

Arquivo interno:

src/std/math.cpp

Usada para cálculos e operações numéricas.

Possíveis operações:

soma
subtração
multiplicação
divisão
arredondamentos
potência
raiz

Exemplo futuro:

importar math

va resultado = math.raiz(25)

mostrar(resultado)

Saída:

5
Random

Biblioteca para geração de valores aleatórios.

Arquivo interno:

src/std/random.cpp

Usada para criar números aleatórios.

Exemplo:

importar random

va numero = random.numero()

mostrar(numero)

Pode ser usada para:

jogos;
sorteios;
testes;
simulações.
NumAleatorio

Biblioteca auxiliar para números aleatórios.

Arquivo interno:

src/std/numAleatorio.cpp

Responsável por funções específicas de geração de números.

Exemplo:

va valor = aleatorio(1,100)

Resultado possível:

73
File

Biblioteca para manipulação de arquivos.

Arquivo interno:

src/std/file.cpp

Permite trabalhar com arquivos do computador.

Possíveis recursos:

criar arquivos;
ler arquivos;
escrever arquivos;
verificar existência.

Exemplo futuro:

importar file

file.escrever(
    "teste.txt",
    "Olá"
)
Time

Biblioteca relacionada a tempo e datas.

Arquivo interno:

src/std/time.cpp

Possui recursos como:

obter horário atual;
medir tempo;
trabalhar com datas.

Exemplo:

importar time

time.agora()
String

Biblioteca para manipulação de textos.

Arquivo interno:

src/std/string.cpp

Recursos:

tamanho de texto;
alteração de caracteres;
divisão de textos;
união de textos.

Exemplo:

va nome = "JLScript"

string.tamanho(nome)
Array

Biblioteca para trabalhar com listas.

Arquivo interno:

src/std/array.cpp

Recursos:

adicionar valores;
remover valores;
acessar posições;
organizar listas.

Exemplo:

va numeros = [1,2,3]

array.adicionar(numeros,4)
Organização interna

As bibliotecas ficam localizadas em:

src/std/

├── console.cpp
├── file.cpp
├── math.cpp
├── random.cpp
├── numAleatorio.cpp
├── time.cpp
├── string.cpp
└── array.cpp
Futuras bibliotecas

Planejamento:

rede (network)
JSON
banco de dados
gráficos
interface gráfica
sistema operacional

A biblioteca padrão tem como objetivo transformar o JLScript em uma linguagem completa,
fornecendo ferramentas prontas para os programas.


Eu deixaria esse arquivo como **versão 0.1 da documentação**. Depois, conforme você terminar cada função em