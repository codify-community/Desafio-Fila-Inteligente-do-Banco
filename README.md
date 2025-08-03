# 🏦 Desafio: Fila de Banco Inteligente

## 🎯 Objetivo
Você vai construir um sistema simples para simular a **fila de atendimento de um banco**.

Mas esse banco tem um detalhe especial:
Ele **respeita quem precisa de prioridade**, mas **não deixa ninguém esperando demais**.

## 🔎 Detalhes

### 👩‍💻 Quem usa esse sistema?

A **atendente do banco**.

Ela é a única que usa o sistema, e pode:

- [X] Gerar senhas para os clientes que chegam
- [X] Chamar os clientes para atendimento
- [X] Ver como está a fila no momento

## 🧠 Como funciona a fila?

Todos os clientes entram em **uma única fila**, mas existem dois tipos de senha:

* **SENHA NORMAL**
* **SENHA PRIORITÁRIA** (para idosos, gestantes etc.)

A atendente **não escolhe quem será chamado**.
O **sistema decide automaticamente** quem será o próximo a ser atendido.

## 📋 Regras da Fila

O banco quer equilibrar a fila para que **ninguém espere demais**, e ainda assim **priorizar quem precisa**.
A ordem de chamadas segue este padrão fixo:

```
(2) prioridades → (1) normal → (1) prioridade → (2) normais → (repete)
```

**O que isso significa?**

Se houver pessoas com prioridade, elas serão chamadas seguindo essa ordem:

- Se **não houver prioridade**, o sistema chama quem estiver na fila.
- Se **só houver prioridades**, o sistema chama só elas, sem problemas.
- Se **a fila estiver vazia**, o sistema exibirá um aviso.

## 💬 Comandos Esperados

### ✅ Gerar senhas:

```
> GERAR PRIORIDADE Ana
> GERAR NORMAL Thiago
> GERAR NORMAL Maria
> GERAR PRIORIDADE José
> GERAR NORMAL Lucas
> GERAR PRIORIDADE Rebeca
```

### ✅ Chamar próximo cliente:

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

### ✅ Ver estado da fila:

```
> FILA
# => Ana, José, Thiago, Rebeca, Maria, Lucas
```

### ✅ Sair do sistema:

Para sair basta um `SAIR` implementado aí no seu código:

```
> SAIR
```

## 🧑‍⚖️ Regras que Valem Pontos

### ❌ NÃO PODE:

- Usar **laços de repetição** como `while`, `for`, `do..while`, `each`, `map`, etc.
- Usar bibliotecas ou funções prontas para organizar a fila (ex: `.sort()` ou similares). **Você precisa organizar a fila na mão!**

### ✅ O código DEVE:

* Funcionar com a **entrada interativa do console**
* Ter **todos os comandos funcionando corretamente**
* Seguir as **regras da fila** descritas acima

### ⭐ Vai ganhar pontos extras se:
- O projeto estiver no **GitHub**
- Ter uma Arquitetura **bem estruturado** em **arquivos separados**
- **Não** houver código comentado que não esteja sendo usado
- Houver um **Dockerfile** para facilitar a execução local
- Houver um **README.md** explicando o projeto
- Tiver **testes automatizados**, com **cobertura acima de 90%**

### 🚫 Será desclassificado se:
- Usar **qualquer forma de loop proibido** como descrito acima
- **Apagar ou recriar** o repositório depois de começar
- **Entregar e continuar fazendo commits** depois do envio

## 🏆 Premiação

**R\$ 150 via PIX** ou **livros/cursos no valor de até R\$ 150 (frete incluso)**

Resaltando que o vencedor é: quem tiver **maior pontuação final**

## ✅ Como Participar

Aqui nessa thread,
- comentar **com tudo maiusculo** a seguinte palavra
`DESAFIO ACEITO` marcando o DevCurumin
- Assim que comentar, já começar algum repositório Github do projeto, com um README.md com alguma frase de DESAFIO ACEITO ou algo assim (exemplo: [Clique aqui pra ver](https://github.com/thiagochirana/desafio-fila-inteligente)) e marca o DevCurumin. É falar que vai começar o desafio e rapidamente já criar um repo no github com um commit pelo menos
- NÃO PODE APAGAR O SEU REPOSITÓRIO OU COMEÇAR OUTRO senão é desclassificação, leia as regras

e para entregar, mande ele aqui me marcando também com o @ com a frase `DESAFIO ENTREGUE`

## 🕒 Prazo para Entrega

🗓️ **Sábado, 9 de Agosto de 2025**
⏰ **Até as 23:59 (horário de Brasília)**

📢 **Resultado: 10 de Agosto de 2025**

### FAQ
<details open>
 <summary>Quem pode participar?</summary>
 TODOS! **PORÉM QUEM TEM MENOS DE 3 MESES DE PROFISSÃO (NA ÁREA DE TI) OU NUNCA INGRESSOU NA ÁREA TEM PESO MAIOR NA PONTUAÇÃO**
</details>

<details open>
 <summary>Qual tecnologia usar?</summary>
 Qualquer uma é válido! O importante é funcionar!
</details>

<details open>
 <summary>Como participar?</summary>
 Me marca aqui com @ e coloca a frase `DESAFIO ACEITO` e já começa o repositório no github, manda o link dele aqui e me marca também, Um pouco mais acima tem detalhes
</details>

<details open>
 <summary>Quais são as tabelas de pontos?</summary>
 Isso será revelado ao final da competição
</details>
