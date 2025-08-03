# 🏦 Desafio: Fila Inteligente do Banco

## 🎯 Objetivo
### Você vai construir um sistema simples para simular a **fila de atendimento de um banco.**

Mas esse banco tem um detalhe especial:
Ele **respeita quem precisa de prioridade,** mas **não deixa ninguém esperando demais.**

## 🔎 Detalhes 
### 👩‍💻 Quem usa esse sistema?
A **atendente do banco.**

Ela é a única que mexe no sistema.

Ela:
 - Gera as senhas para quem chega para o atendimento
 - Chama as pessoas para serem atendidas
 - Pode ver como está o estado da fila no momento

### 🧠 Como funciona a fila?
Todos os clientes entram em **uma única fila,** mas com um detalhe:

 - Alguns têm **SENHA NORMAL**

 - Outros têm **SENHA PRIORITÁRIA (idosos, gestantes etc.)**

A atendente **NUNCA** escolhe quem vai ser chamado.
O **sistema decide automaticamente** quem deve ser o próximo a ser chamado

### 📋 Regras da fila

O banco quer **equilibrar a fila para ninguém esperar demais.**
O sistema segue essa ordem de chamadas (ou fórmula):

```
2 prioridades → 1 normal → 1 prioridade → 2 normais → (repete)
```

Isso significa:
 - Se tiver gente com prioridade, eles serão chamados de acordo com essa ordem acima.
 - Se não tiver prioridade na fila, atende quem tiver.
 - Se só tiver prioridades, atende eles sem problema.
 - Se a fila estiver vazia, mostra uma mensagem dizendo isso.

### 💬 Comandos Esperados


```
> GERAR PRIORIDADE Ana

> GERAR NORMAL Thiago

> GERAR NORMAL Maria

> GERAR PRIORIDADE José

> GERAR NORMAL Lucas

> GERAR PRIORIDADE Rebeca

```

```

> CHAMAR
# => Ana

> CHAMAR
# => José

> CHAMAR
# => Thiago

> CHAMAR
# => Rebeca

> CHAMAR
# => Maria

> CHAMAR
# => Lucas

> CHAMAR
# => Fila está vazia!
```

```
> FILA

# => Ana, José, Thiago, Rebeca, Maria, Lucas
```

Para sair basta um `SAIR` implementado aí no seu código

### 🧑‍⚖️  Porém, temos regras QUE VALEM PONTOS
#### ❌ NÃO PODE:
- usar loops de repetiçao (while, do..while, for, each, times, etc etc etc) em nenhum momento no código!
- usar libs ou ferramentas prontas para organização da fila (por exemplo usar `.sort()` ou `.organize()` nada disso!) Tem que fazer a organização na mão!
- Usar entrada interativa via console

#### 📌 E SEU CÓDIGO DEVE:
- Apresentar TODOS os comandos funcionando corretamente
- Atender os critérios acima para ser minimamente qualificado

**ESSES SÃO OS REQUISITOS MÍNIMOS PARA A COMPETIÇÃO**

#### ✅ Vai ter pontos extras SE o projeto:
- Estiver acessível no GitHub
- Ter uma Arquitetura de código entendível e não tudo em um só arquivo
- NÃO conter código comentado que NÃO é usado (boa higiene de código)
- Conter um `Dockerfile` para facilitar o avaliador rodar localmente
- Conter um `README.md` documentando o seu código
- Ter testes unitários e com cobertura acima de 90%

**MAS NÃO É OBRIGATÓRIO, É APENAS UM EXTRA QUE VAI VALER PONTOS**

#### 🚫 Será desclassificado se:
- O código usar qualquer forma de loop proibido como descrito acima
- O repositório for **apagado ou recriado** após o início
- For entregue e **commits continuarem sendo feitos**

### 🏆 ENTÃO VAI TER PREMIAÇÃO?

### `SIM!! 150 REAIS NO PIX OU QUALQUER LIVROS ou CURSOS DE ATÉ 150 REAIS (somando tudo, incluindo o frete)! PARA O VENCEDOR QUE OBTIVER MAIS PONTOS`

### Como se inscrever:

Aqui nessa thread,
- comentar **com tudo maiusculo** a seguinte palavra
`DESAFIO ACEITO`
- Assim que comentar, já começar algum repositório Github do projeto, com um README.md com alguma frase de DESAFIO ACEITO ou algo assim (exemplo: [Clique aqui pra ver](https://github.com/thiagochirana/desafio-fila-inteligente)) e me marca com @. É falar que vai começar o desafio e rapidamente já criar um repo no github com um commit pelo menos
- NÃO PODE APAGAR O SEU REPOSITÓRIO OU COMEÇAR OUTRO senão é desclassificação, leia as regras

e para entregar, mande ele aqui me marcando também com o @ com a frase `DESAFIO ENTREGUE`

### PRAZO PRA ENTREGA: 

`SÁBADO, 9 DE AGOSTO DE 2025, ATÉ AS 23:59 DO HORÁRIO DE BRASILIA`

`RESULTADO SAI DIA 10 DE AGOSTO DE 2025, HORÁRIO AINDA A DEFINIR`


### FAQ
#### Quem pode participar?
- TODOS! **PORÉM QUEM TEM MENOS DE 3 MESES DE PROFISSÃO (NA ÁREA DE TI) OU NUNCA INGRESSOU NA ÁREA TEM PESO MAIOR NA PONTUAÇÃO**

#### Qual tecnologia usar?
- Qualquer uma é válido! O importante é fazer funcionar!

#### Como participar?
- Me marca aqui com @ e coloca a frase `DESAFIO ACEITO` e já começa o repositório no github, manda o link dele aqui e me marca também, Um pouco mais acima tem detalhes

#### Quais são as tabelas de pontos?
- Isso será revelado ao final da competição

#### Qual o critério de desempate?
- O tempo desde do `DESAFIO ACEITO` até o momento da última entrega do projeto com `DESAFIO ENTREGUE`. Atente-se para NÂO FAZER COMMITS DEPOIS DE AVISAR QUE ENTREGOU
