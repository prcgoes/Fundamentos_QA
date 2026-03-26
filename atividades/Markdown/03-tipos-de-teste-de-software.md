# Testes de Software

#### Vamos classificar para melhorar o entendimento.

1. [Testes Funcionais vs. Não Funcionais](#1-testes-funcionais-vs-não-funcionais)
2. [Execução: Manual vs. Automatizada](#2-execução-manual-vs-automatizada)
3. [Matriz de Decisão](#3-matriz-de-decisão)

---

## 1. Testes Funcionais vs. Testes Não Funcionais 

Esta classificação foca no **objetivo** do teste, basicamente (o "quê" estamos testando).

### 🟢 Funcionais - O que o sistema FAZ
Focam nos requisitos de negócio e nas funcionalidades.
* **Exemplo:** O botão "Enviar" realmente manda o formulário? O login funciona com a senha correta?

* **Tipos comuns de testes funcionais:**     Testes unitários, integração, fumaça (smoke test) e aceitação (UAT).

#### Podemos apronfudar mais nesses exemplos

**Integração**
O que é? 
Eles verificam se dois ou mais módulos do sistema funcionam bem quando juntos.

**_Exemplo:_** O sistema de "Login" consegue buscar e validar a senha corretamente no "Banco de Dados"?

**Fumaça (Smoke Test)**
O que é?
É um conjunto de testes rápidos nas funções críticas. Se ele falha, o sistema nem é testado, volta para o desenvolvedor na hora.

**_Exemplo:_** O aplicativo abre? Consigo logar? Consigo chegar na tela principal? Se sim, a "fumaça" passou.

**Aceitação (UAT - User Acceptance Testing)**
O que é?
 É a última etapa. O usuário final ou o cliente testa o sistema para confirmar se atende às necessidades do negócio dele.

**_Exemplo:_** O dono da empresa usa o sistema e diz: "Sim, isso resolve o meu problema, podem lançar".

### 🟡 Não Funcionais - Como o sistema SE COMPORTA
Focam em aspectos de qualidade, experiência e segurança.

* **Exemplo:** O site aguenta 1000 pessoas acessando ao mesmo tempo? Como ele se comporta se essa quantidade for muito maior ou muito menor? O sistema é seguro contra hackers? As cores são acessíveis?

* **Tipos comuns de testes não funcionais:** Testes de performance, carga, segurança, usabilidade e portabilidade.

**Performance**
O que é?
Avalia o tempo de resposta e estabilidade sob condições normais.

**_Exemplo:_** O site demora quanto tempo para carregar uma foto? 
(O padrão é ser rápido).

**Carga (Load Test)**
O que é?
Verifica como o sistema se comporta com um número alto de acessos simultâneos.

**_Exemplo:_** O site do governo aguenta 1 milhão de pessoas tentando declarar o imposto de renda ao mesmo tempo?

**Segurança**
O que é?
Identifica brechas, invasões ou vazamento de dados confidenciais.

**_Exemplo:_** Um hacker consegue descobrir a senha de um usuário apenas olhando o link da página?

**Usabilidade**
O que é?
Foca na facilidade de aprendizado e satisfação do usuário.

**_Exemplo:_** O botão "Comprar" está visível? É fácil para um idoso usar o aplicativo sem treinamento?

**Portabilidade**
O que é?
Garante que o software funcione em diferentes ambientes, sistemas ou dispositivos.

 **_Exemplo:_** O sistema funciona igual no seu Ubuntu (Linux), no Windows de um colega e no Android do celular?

---

## 2. Execução: Manual vs. Automatizada 

Esta classificação foca na **forma** como o teste é feito.

### Testes Manuais
Feitos por um humano que interage com o software como se fosse o usuário.

* **Vantagens:** Ótimo para avaliar usabilidade (olhar humano), testes exploratórios e validar ideias novas rapidamente.

* **Desvantagem:** Lento, cansativo para tarefas repetitivas e sujeito a erro humano.

### Testes Automatizados

Scripts ou ferramentas (como Selenium ou Cypress) que executam os passos sozinhos.

* **Vantagens:** Extremamente rápidos, podem rodar 24h por dia e são perfeitos para **testes de regressão** (garantir que nada quebrou após uma mudança).

* **Desvantagem:** Custo inicial alto (tempo para escrever o código) e exige manutenção constante.

---

## 3. Matriz de Decisão ✅

| Cenário | Melhor Opção | Por quê? |
| :--- | :--- | :--- |
| **Nova Funcionalidade** |  Manual | Entender o fluxo antes de codar o teste. |
| **Teste de Carga** |  Automatizado | Impossível simular 5000 usuários manualmente. |
| **Interface/Design** |  Manual | O computador não sabe se o botão está "feio". |
| **Rotina Diária** |  Automatizado | Libera o QA para tarefas mais inteligentes. |

