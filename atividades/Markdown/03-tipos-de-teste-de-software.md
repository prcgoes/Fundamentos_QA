# Testes de Software

#### Vamos classificar para melhorar o entendimento.

1. [Testes Funcionais vs. Não Funcionais](#1-testes-funcionais-vs-não-funcionais)
2. [Execução: Manual vs. Automatizada](#2-execução-manual-vs-automatizada)
3. [Matriz de Decisão](#3-matriz-de-decisão)

---

## 1. Testes Funcionais vs. Testes Não Funcionais 

Esta classificação foca no **objetivo** do teste, basicamente (o "quê" estamos testando).

### 🟢 Funcionais (O que o sistema FAZ)
Focam nos requisitos de negócio e nas funcionalidades.
* **Exemplo:** O botão "Enviar" realmente manda o formulário? O login funciona com a senha correta?

* **Tipos comuns de testes funcionais:**     Testes unitários, integração, fumaça (smoke test) e aceitação (UAT).

### 🟡 Não Funcionais (Como o sistema SE COMPORTA)
Focam em aspectos de qualidade, experiência e segurança.
* **Exemplo:** O site aguenta 1000 pessoas acessando ao mesmo tempo? Como ele se comporta se essa quantidade for muito maior ou muito menor? O sistema é seguro contra hackers? As cores são acessíveis?
* **Tipos comuns de testes não funcionais:** Testes de performance, carga, segurança, usabilidade e portabilidade.

---

## 2. Execução: Manual vs. Automatizada 

Esta classificação foca na **forma** como o teste é feito.

### ✍️ Testes Manuais
Feitos por um humano que interage com o software como se fosse o usuário.
* **Vantagens:** Ótimo para avaliar usabilidade (olhar humano), testes exploratórios e validar ideias novas rapidamente.
* **Desvantagem:** Lento, cansativo para tarefas repetitivas e sujeito a erro humano.

### ⚙️ Testes Automatizados
Scripts ou ferramentas (como Selenium ou Cypress) que executam os passos sozinhos.
* **Vantagens:** Extremamente rápidos, podem rodar 24h por dia e são perfeitos para **testes de regressão** (garantir que nada quebrou após uma mudança).
* **Desvantagem:** Custo inicial alto (tempo para escrever o código) e exige manutenção constante.

---

## 3. Matriz de Decisão ✅

| Cenário | Melhor Opção | Por quê? |
| :--- | :--- | :--- |
| **Nova Funcionalidade** | ✍️ Manual | Entender o fluxo antes de codar o teste. |
| **Teste de Carga** | ⚙️ Automatizado | Impossível simular 5000 usuários manualmente. |
| **Interface/Design** | ✍️ Manual | O computador não sabe se o botão está "feio". |
| **Rotina Diária** | ⚙️ Automatizado | Libera o QA para tarefas mais inteligentes. |

---

 | CENÁRIO | EXEMPLO PRÁTICO |
  | :---: | :---: |
  | **Alta Severidade / Baixa Prioridade** | O sistema trava (crash) ao tentar gerar um relatório de 1990 que ninguém mais usa. É grave, mas não urgente |
  | **Baixa Severidade / Alta Prioridade** | O logotipo da empresa na página inicial está com as cores erradas ou o nome da marca está escrito errado. Tecnicamente não quebra nada, mas é péssimo para a imagem |

  
  ## Tipos de Teste

  De acordo com o **ISTQB**, os testes são agrupados em quatro categorias principais baseadas nos seus objetivos:

**Testes Funcionais**
Focam no "o que" o sistema faz. Eles avaliam as funções que o software deve executar (requisitos funcionais).

**Ex:** Verificar se o sistema permite realizar o login com sucesso.

**Testes Não-Funcionais**
Focam no "como" o sistema se comporta. Avaliam características como desempenho, usabilidade, segurança e confiabilidade.

**Ex:** Testar se o sistema suporta 1.000 usuários simultâneos sem ficar lento (Teste de Carga).

**Testes de Caixa-Branca (Estruturais)**
Baseiam-se na análise da estrutura interna do sistema ou componente (o código, o fluxo de dados ou a arquitetura).

**Ex:** Testar se todos os caminhos de uma instrução if/else foram percorridos pelos testes unitários.

**Testes Relacionados a Mudanças**
Esses ocorrem após a correção de um defeito ou uma alteração no sistema:

**Teste de Confirmação (Re-teste):** Executar os mesmos testes que falharam anteriormente para confirmar que o defeito foi corrigido.

**Teste de Regressão:** Testar partes do sistema que não foram alteradas para garantir que a nova mudança não introduziu novos defeitos em funcionalidades que já estavam boas.

Dica: _O Teste de Regressão pode ser aplicado a qualquer nível de teste (unitário, integração, sistema, aceite)._

