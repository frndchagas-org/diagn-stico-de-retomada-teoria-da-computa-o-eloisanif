[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/zHqjFsRx)
# Diagnóstico de retomada - Teoria da Computação

Esta atividade serve para mapear o que você já domina sobre linguagens formais, autômatos, gramáticas e computabilidade.

Responda individualmente. Use suas palavras. Se usar IA depois da primeira tentativa, registre o uso na seção 7.

## 1. Mapa do que eu lembro

Marque cada tópico como: lembro bem, lembro parcialmente, não lembro, nunca vi ou não tenho certeza.

- alfabeto:lembro bem.
- cadeia:lembro bem.
- linguagem:lembro bem.
- gramática:lembro bem.
- autômato finito:lembro bem.
- linguagem regular:lembro bem.
- linguagem livre de contexto:lembro parcialmente.
- linguagem sensível ao contexto:lembro parcialmente.
- linguagem irrestrita: lembro parcialmente.
- hierarquia de Chomsky:não lembro.
- computabilidade:lembro parcialmente.
- máquina de Turing:lembro parcialmente.

## 2. Definições com exemplo

Explique, com suas palavras e com um exemplo simples, usando o alfabeto `Sigma = {a, b}`.

1. O que é um alfabeto? É um conjunto de símbolos usado para formar palavras, por exemplo, Sigma={a,b}.
2. O que é uma cadeia? É uma sequência de símbolos vindos do alfabeto pré-estabelecido, por exemplo: "abaabb"
3. O que é uma linguagem? É o conjunto de cadeias formadas pelo alfabeto, exemplo: a, ab, aba
4. O que é uma gramática? São regras para gerar palavras de uma linguagem.
   
## 3. Linguagens

Considere as linguagens:

```text
L1 = { w em {0,1}* | w termina com 01 }
L2 = { a^n b^n | n >= 0 }
L3 = { a^n b^n c^n | n >= 0 }
```

Para cada linguagem:

1. escreva três palavras que pertencem à linguagem;
 L1 = { w em {0,1}* | w termina com 01 } - 01; 1101.
 L2 = { a^n b^n | n >= 0 } - aabb; aaaabbbb.
 L3 = { a^n b^n c^n | n >= 0 - abc; aabbcc.
3. escreva duas palavras que não pertencem;
   L1 = 10, 111;
   L2 = abb, aabbb;
   L3 = aabccc; abbbcc;
5. diga, se souber, em qual classe ela provavelmente se encaixa;
      L1 = Linguagem regular
      L2 = Livre de contexto
      L3 = sensível ao contexto
7. explique o motivo em linguagem simples.
  L1 = basta verificar se termina o elemento termina com '01'
  L2 = a quantidade elementos de a precisa ser igual à de b
  L3 = precisa ser a mesma quantidade de a, b e c.

Não há problema em dizer "não sei". Nesse caso, escreva o que te deixou em dúvida.

## 4. Autômato finito

Considere o autômato abaixo, sobre o alfabeto `{0,1}`:

```text
Estados: q0, q1, q2
Estado inicial: q0
Estado final: q2

Transições:
q0 --0--> q1
q0 --1--> q0
q1 --0--> q1
q1 --1--> q2
q2 --0--> q1
q2 --1--> q0
```

Responda:

1. Qual linguagem esse autômato parece reconhecer? Ele reconhece cadeias que terminam em 01.
2. Execute manualmente as cadeias abaixo e diga se aceita ou rejeita:
   - `01` -> Aceita
   - `101` -> Aceita
   - `100`-> Rejeita
   - `1101` -> Aceita
   - `111` -> Rejeita
3. Monte uma tabela curta mostrando o caminho dos estados para pelo menos duas cadeias.
   - `01` - q0 -> q1 > q2
   - `100`- q0 -> q0 -> q1 -> q1

## 5. Gramática

Considere a gramática:

```text
S -> aS
S -> b
```

Responda:

1. Gere cinco cadeias produzidas por essa gramática.
   1. b / 2. ab / 3.aab / 4. aaab / 5. aaaab

3. Descreva a linguagem em palavras.
   A linguagem é formada por várias letras seguidas de um b no final de cada uma delas.
5. Essa gramática parece regular, livre de contexto ou outra classe? Justifique de forma simples.
   Regular, por seguir um padrão simples.

## 6. Ponto de dificuldade

Escolha um tópico da lista inicial e escreva:
Tópico:
Hierarquia de Chomsky
1. o que você entende dele; Lembro vagamente que está relacionada à classificação das linguagens formais.
2. onde você se confunde; Lembrar as diferenças entre cada categoria e como identificar os tipos.
3. que tipo de explicação ajudaria: desenho, exemplo, exercício guiado, analogia, prova passo a passo ou lista curta.
   Exercício guiado/analogias.

## 7. Uso de IA, se houver

Se você usou IA depois da primeira tentativa, registre:

Pergunta feita:
Pedi para que me explicasse conceitos básicos dos assuntos de forma que me ajudasse a relembrar os conceitos iniciais da disciplina.
Resumo da resposta:
A IA explicou brevemente cada tópico.
Como eu verifiquei:
Não verifiquei diretamente, mas fui relembrando dos conceitos abordados em sala.
O que eu alterei na minha resposta:
Fui reescrevendo com minhas próprias palavras e com o que eu ia lembrando e entendendo.
O que ainda não entendi:
Ainda tenho um pouco de dificuldade em Máquina de Turing.

## Submissão no Moodle

Depois de finalizar, copie no Moodle:

```text
Repositório:
Commit final:
Autoavaliação: nível atual, maior dificuldade e tópico que precisa ser retomado.
```
