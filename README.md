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
- Ter uma Arquitetura **bem estruturado** em **arquivos separados**
- **Não** houver código comentado que não esteja sendo usado
- Houver um **Dockerfile** para facilitar a execução local
- Houver um **README.md** explicando o projeto
- Tiver **testes automatizados**, com **cobertura acima de 90%**

### 🚫 Será desclassificado se:
- Usar **qualquer forma de loop proibido** como descrito acima
- **Apagar ou recriar** o repositório depois de começar
- **Entregar e continuar fazendo commits** depois do envio
- O projeto apresentar indícios de uso de **IA**

## 🏆 Premiação

**R\$ 150 via PIX** ou **livros/cursos no valor de até R\$ 150 (frete incluso)**

Resaltando que o vencedor é: quem tiver **maior pontuação final**

## ✅ Como Participar

1. Crie um repositório no **Github**
2. Adicione a tag/tópico `codify` ao repositório **Sem a tag não conseguiremos encontrar seu projeto!**

## 🕒 Prazo para Entrega

🗓️ **Sábado, 9 de Agosto de 2025**
⏰ **Até as 23:59 (horário de Brasília)**

📢 **Resultado: 10 de Agosto de 2025**

## ❓ FAQ

<details open>
 <summary><strong>Como participar?</strong></summary>

 Crie um repositório no **Github** e adicione a tag/tópico `codify` ao repositório **Sem a tag não conseguiremos encontrar seu projeto!**
</details>

<details open>
 <summary><strong>Quem pode participar?</strong></summary>

 **TODOS** podem participar!
 Mas quem tem **menos de 3 meses de experiência na área de TI** ou **ainda não ingressou profissionalmente**, terá **um peso maior na pontuação final**.
</details>

<details open>
 <summary><strong>Qual tecnologia usar?</strong></summary>

 Use **a linguagem ou stack que preferir!**
 O importante é que o sistema funcione com todos os comandos obrigatórios implementados corretamente.
</details>

<details open>
 <summary><strong>Quais são as tabelas de pontos?</strong></summary>

 Serão divulgadas **ao final da competição**, junto com o resultado.
</details>
