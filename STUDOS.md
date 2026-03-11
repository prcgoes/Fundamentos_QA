# Quando o assunto é QA... surgem muitas duvidas?!
### Vamos estudar para entender :)

##  Definição e Importância Estratégica da Garantia de Qualidade

**Introdução ao conceito:**
 A garantia de qualidade (do inglês **Qualyt Assurence (QA)**)  é um conjunto de atividades sistemáticas planejadas para garantir que um produto ou serviço atenda aos requisitor especificados e ás expectativas do cliente.  No contexto de software, o QA não foca apenas no "produto pronto", mas  em todo o **processo** de fabricação.

#### Na prtatica: O que é QA?
* **Prevenção:** O foco principal é evitar que o erro aconteça; 
O cara avisa: "Cuido, se fizermos assim, vai dar erro la na frente"
* **Processo:** Analise desde a clareza dos documentos até a forma como os desenvolvedores escrevem o codigo. Ele olha como o trabalho está sendo feito para garantir que o resultado seja bom de primeira.
*  **Cultura:** É uma mentalidade de "qualidade  em primeiro lugar" compartilhada por todo o time. 
É o selo de garantia de que o que está sendo entregue funciona de verdade.

#### O que não é QA? (Quebrando mitos)

Para entender o que é QA é preciso diferenciar de concetos comumentes confundidos.
* **Não é apenas "Caçar Bugs":** Encontrar erros é tarefa do _Testing_. O QA quer entender como o erro apareceu e como mudar o porcesso para que ele não volte a acontecer.
O teste é só uma parte. O QA quer evitar que o erro sequer exista.
* **Não é o chato do time:**  O QA não te que ser a pessoa que diz apenas "SIM" ou "Não" ao final do projeto, ele deve ser um colaborador desde o dia 1.
Ele não quer apontar o dedo pro erro do colega, ele quer garantir que o cliente não receba um produto ruim.
* **Não é burocracia:** Embora utilize processos, o objetivo é a eficiencia e a segurança, não a criação de documentos inúteis.
Se o QA só aparece no último dia, ele vira um "bombeiro" apagando incêndio, e não um garantidor de qualidade.

#### A Importancia Fundamental nas Empresas
A presença de um area ou mentalidade QA é um divisor de aguas entre empresas amadoras e empresas de alta performance.

* **Viabilidade economica** - A economia é o argumento mais forte para o QA. BAesado na curva de **Custo de Defeito** , quanto mai cedo um deifeito é detectado, mais barato é o seu concerto.  
	
* **Mantém o cliente feliz**- O QA garante que, quando o usuário clicar no botão, a mágica aconteça. Isso cria confiança. Cliente confio é cliente que continua pagando a mensalidade e indica para os amigos.

* **Deixa o trabalho mais rápido**- Parece loucura, mas testar faz o processo andar mais rápido. Por quê? Porque o time não precisa ficar parando toda hora para consertar coisas que já deveriam estar prontas. O fluxo flui melhor.

### *Exemplo prático*:


| Situação | QuanO que o QA faz | O que a Empresa ganha |
| :--- | :---: | ---: |
| App de BAnco | Testa dse o pix cai na contacerta mesmo com internet lenta | O banco não perde a confiança do cliente com o dinheiro sumido  |
| BananasSistemas de compras | Garante que o sistema não de um cupo de desconto de 100% em uma compra | A emprea não irá a falencia por um erro de digitação |
| Instagran/TikTok | Testa se um video carrga sem travar o celular | o usuário continua usando app sem passar raiva |

# QA vs. QC vs. Testes: Quem faz o quê?

Duvida frequente, é muito comum fazermos *confusão* e não saber quem exerce cada papel.

Para melhor entendimento, vamos relacionar com coisas do mundo real. 
imagine uma **Fabrica de sucos**;

* **QA** (Quality Assurance) - A Garantia
O QA é o "dono da receita" e dos processos. Ele não está preocupado com uma garrafa específica, mas sim com a fábrica inteira.

*Foco: No PROCESSO.*

**O que faz:** Cria as regras. "As frutas devem ser lavadas assim", "As máquinas precisam de manutenção todo mês".

**Objetivo:** Prevenir que o erro aconteça. Se o processo é bom, o suco dificilmente sairá ruim.

**É Proativo:** Ele age antes do problema existir.

* **QC** (Quality Control) - O Controle
O QC é o "inspetor da linha de produção". Ele olha para o produto final que já está pronto para sair.

*Foco: No PRODUTO.*

**O que faz:** Pega uma garrafa da esteira e verifica: "O lacre está fechado? A cor está certa? O peso está correto?".

**Objetivo:** Identificar erros no que já foi fabricado. Ele impede que o produto estragado chegue ao cliente.

**É Reativo:** Ele age depois que algo foi produzido.

* **Testes** (Testing) - A Ação
O Teste é a "ferramenta" do QC. É a parte técnica e prática de colocar a mão na massa.

*Foco: Na EXECUÇÃO.*

**O que faz:** Beber o suco para ver se o gosto está bom. Apertar a garrafa para ver se vaza.

**Objetivo:** Encontrar defeitos (bugs) através da experimentação.

**É a ferramenta:** O teste é o ato de validar se aquilo que foi construído funciona como deveria.


| Termo | Onde foca? | Qual a missão? | Analogia |
| :--- | :---: | :---: | ---: |
| **QA** | No processo | Prevenir erros | Cria a receita perfeita | 
| **QC** | No produto | Achar o erro| Conferir se o bolo solou | 
| **Teste** | Na execução | demonstrar o erro | Dar um agarfada no bolo e conferir o resultado | 


## Bugs ≠ Defeitos ≠ Falhas

### Erro
Erro ocorre por uma falha Humana, pessoas que produz um resultado incorreto. Pode-se afirmar que é a "origem de tudo".

Pode ocorrer devido a acansaço, pressão de prazos, pouca experiência ou má interpretação de requisitos.
(desenvolvedores, analistas e testadores) 

**Ex:** Um desenvolvedor esquece de considerar que o estoque pode ser zero e escreve a lógica usando apenas "maior que" ($>$) em vez de "maior ou igual a" ($\ge$).

**Erro** ---> pode produzir ---> **Defeito (s)** ---> pode prozir ---> **Falha (s)**


### Defeito
Um defeito é o resultado do Erro, imperfeição ou deficiência em um produto de trabalho (codigo, documento de requisito, design)
A manifestaçã física do erro no papel ou no código.

**Ex:** _A linha de código if (estoque > 0) gravada no arquivo, quando o requisito pedia para incluir o zero._

**OBS: Um defeito pode existir para sempre sem nunca ser "visto" se aquela linha de código específica nunca for executada.**

### Falha

A falha acontece quando um componente ou o sistema não execiuta a função exigida de acordo com o que foi especificado. Comportamento inadequado na sua execução (_ROUTINE_).

**Ex:** _O usuário tenta finalizar uma compra com o último item do estoque e o sistema exibe uma mensagem de "Erro inesperado: Produto indisponível", impedindo a venda._

  ## Severidade vs Prioridade

  **Severidade** ---> foca ---> Impacto técnico
  **Prioridade** ---> foca ---> Impacto de negócio e no cronograma

  **Severidade (Impacto Técnico)**
  Defini o impacto que o defeito tem no desenvolvimento ou na operação de um componente ou sistema.
  Uma forma de medir a "**gravidade**" do problema sob oponto de vista de software.

  **EX:** Um sistema trava

  **Severidade alta:** funcionalidades importantes deixamm de funcionar; 

  **Severidade baixa:** erro no visual;

  **Prioridade (Impacto de Negócio)**
  Define o grau de importancia aribuida a um ítem (Ex. Um defeito) para que seja corrigido. Esta atribuição esta relacionada a urgência para o negócio ou para o cliente. Impacto direto.

  **Prioridade alta:** corrigir imediatamente;

  **Prioridade média:** corrigir na proxima sprint;
  **Prioridade baixa:** corrigir quando houve tempo;


  **_Nem sempre um defeito grave precisa ser corrigido agora, e nem sempre um erro estético pode esperar._**

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


