# Atividade 3 — Estratégia e Projeto de Testes do LocalEats

## Tarefa 1 — Planejamento dos testes

### 1.1 Objetivo dos testes

Verificar se a funcionalidade de pesquisa do LocalEats permite que o usuário encontre restaurantes de acordo com a especialidade ou localização informada, apresentando resultados compatíveis com a pesquisa realizada e evitando a exibição de restaurantes que não correspondam ao termo pesquisado.


### 1.2 Escopo

**Integrante:** Manoela
**Funcionalidade incluída:** Pesquisar restaurantes por especialidade ou localização.
**O que será verificado:** Será verificado se a pesquisa apresenta restaurantes compatíveis com a especialidade ou localização informada e como o sistema se comporta quando não existem restaurantes correspondentes ao termo pesquisado.
**Funcionalidade não incluída:** Fazer pedido.
**Justificativa:** A funcionalidade de fazer pedido não faz parte do fluxo de pesquisa escolhido como foco desta atividade.

### 1.3 Abordagem

**Nível de teste:** Sistema.
**Justificativa:** A funcionalidade será analisada pela interface da aplicação, considerando o comportamento apresentado ao usuário durante todo o fluxo de pesquisa.
**Tipo de teste:** Funcional.
**Justificativa:** O objetivo é verificar se a pesquisa realiza corretamente sua função e apresenta resultados de acordo com os dados informados pelo usuário.
**Perspectiva:** Caixa-preta.
**Justificativa:** Os testes serão planejados considerando os dados fornecidos pelo usuário e os resultados apresentados pelo sistema, sem analisar o código-fonte da aplicação.
**Técnica de teste:** Particionamento de equivalência.
**Justificativa:** A técnica permite dividir os possíveis dados de pesquisa em grupos que devem apresentar comportamentos semelhantes. Dessa forma, é possível selecionar entradas representativas sem precisar testar todas as especialidades, localizações ou termos possíveis.


### 1.4 Ambiente e responsabilidades

**Ambiente necessário:** Aplicação LocalEats disponível, navegador atualizado, computador ou notebook com conexão à internet e restaurantes cadastrados com informações de especialidade e localização.
**Responsável pelo planejamento:** Manoela.
**Responsável pela especificação dos casos de teste:** Manoela.
**Responsável pela futura execução dos testes:** Manoela.

### 1.5 Critérios

**Critério de entrada:** A aplicação deve estar disponível e possuir restaurantes cadastrados com informações de especialidade e localização que permitam realizar os testes planejados.
**Critério de saída:** Todos os casos de teste planejados deverão ser executados futuramente e seus resultados deverão ser registrados para verificar se o comportamento observado corresponde ao resultado esperado.
**Critério de suspensão:** Os testes deverão ser suspensos caso a aplicação esteja indisponível ou não existam dados cadastrados suficientes para realizar as pesquisas planejadas.

## Tarefa 2 — Riscos e técnicas de teste

### 2.1 Análise dos riscos

| ID | Integrante | Funcionalidade | Risco | Consequência | Probabilidade | Impacto | Prioridade | Justificativa |
|---|---|---|---|---|---|---|---|---|
| R01 | Manoela | Pesquisar restaurantes por especialidade ou localização | A pesquisa apresentar restaurantes que não correspondem ao termo informado | O usuário pode receber resultados incorretos e ter dificuldade para encontrar um restaurante adequado ao que está procurando | Média | Média | Média | A pesquisa é uma funcionalidade importante para a exploração dos restaurantes e resultados incorretos podem prejudicar a experiência do usuário |
| R02 | Manoela | Pesquisar restaurantes por especialidade ou localização | A pesquisa não apresentar um restaurante mesmo quando existe um cadastro correspondente ao termo pesquisado | O usuário pode concluir que não existem restaurantes daquela especialidade ou localização e deixar de utilizar uma opção que está disponível | Média | Alta | Alta | A falha impede que restaurantes existentes sejam encontrados e compromete diretamente a função principal da pesquisa |


### 2.2 Aplicação da técnica

**Integrante responsável:** Manoela
**Funcionalidade:** Pesquisar restaurantes por especialidade ou localização.
**Riscos relacionados:** R01 e R02.
**Técnica escolhida:** Particionamento de equivalência.

### Por que a técnica foi escolhida?

A técnica de particionamento de equivalência foi escolhida porque existem diferentes grupos de dados que podem ser informados na pesquisa e não é necessário testar todas as entradas possíveis.

É possível selecionar valores representativos de cada grupo e verificar se o sistema apresenta o comportamento esperado.


### Aplicação da técnica

Foram identificadas as seguintes classes de equivalência:

| Classe | Situação | Valor representativo |
|---|---|---|
| CE01 — Com correspondência | Especialidade que possui restaurante cadastrado | Uma especialidade existente na aplicação |
| CE02 — Com correspondência | Localização que possui restaurante cadastrado | Uma localização existente na aplicação |
| CE03 — Sem correspondência | Termo que não corresponde a nenhum restaurante cadastrado | Um termo inexistente na aplicação |

### Casos derivados

**CE01:** CT01 — Pesquisar restaurante por uma especialidade existente.

**CE02:** CT02 — Pesquisar restaurante por uma localização existente.

**CE03:** CT03 — Pesquisar utilizando um termo sem correspondência.


## Tarefa 3 — Casos de teste e rastreabilidade

### 3.1 Especificação dos casos de teste

### CT01 — Pesquisar por uma especialidade existente

**Integrante responsável:** Manoela
**Funcionalidade:** Pesquisar restaurantes por especialidade ou localização.
**Risco relacionado:** R01 e R02.
**Técnica utilizada:** Particionamento de equivalência — CE01.
**Pré-condição:** A aplicação LocalEats deve estar disponível e deve existir pelo menos um restaurante cadastrado com a especialidade escolhida para o teste.
**Dados de entrada:** Uma especialidade existente entre os restaurantes cadastrados na aplicação.

**Passos:**

1. Acessar a página inicial do LocalEats.
2. Localizar o campo de pesquisa.
3. Informar uma especialidade existente.
4. Realizar a pesquisa.
5. Verificar os restaurantes apresentados.

**Resultado esperado:** O sistema deve apresentar restaurante(s) correspondente(s) à especialidade pesquisada e não deve apresentar como resultado restaurantes incompatíveis com o termo informado.


### CT02 — Pesquisar por uma localização existente

**Integrante responsável:** Manoela
**Funcionalidade:** Pesquisar restaurantes por especialidade ou localização.
**Risco relacionado:** R01 e R02.
**Técnica utilizada:** Particionamento de equivalência — CE02.
**Pré-condição:** A aplicação LocalEats deve estar disponível e deve existir pelo menos um restaurante cadastrado com a localização utilizada no teste.
**Dados de entrada:** Uma localização existente entre os restaurantes cadastrados na aplicação.

**Passos:**

1. Acessar a página inicial do LocalEats.
2. Localizar o campo de pesquisa.
3. Informar uma localização existente.
4. Realizar a pesquisa.
5. Verificar os restaurantes apresentados.

**Resultado esperado:** O sistema deve apresentar restaurante(s) correspondente(s) à localização pesquisada e não deve apresentar como resultado restaurantes incompatíveis com o termo informado.


### CT03 — Pesquisar utilizando um termo sem correspondência

**Integrante responsável:** Manoela
**Funcionalidade:** Pesquisar restaurantes por especialidade ou localização.
**Risco relacionado:** R01.
**Técnica utilizada:** Particionamento de equivalência — CE03.
**Pré-condição:** A aplicação LocalEats deve estar disponível.
**Dados de entrada:** Um termo que não corresponda à especialidade ou localização de nenhum restaurante cadastrado.

**Passos:**

1. Acessar a página inicial do LocalEats.
2. Localizar o campo de pesquisa.
3. Informar um termo sem correspondência com os restaurantes cadastrados.
4. Realizar a pesquisa.
5. Verificar o comportamento apresentado pelo sistema.

**Resultado esperado:** O sistema não deve apresentar como resultado restaurantes que não correspondam ao termo pesquisado.


### 3.2 Matriz de rastreabilidade

| Integrante | Funcionalidade | Risco ou requisito | Técnica utilizada | Casos de teste |
|---|---|---|---|---|
| Manoela | Pesquisar restaurantes por especialidade ou localização | R01 — Apresentar restaurantes que não correspondem ao termo pesquisado | Particionamento de equivalência | CT01, CT02 e CT03 |
| Manoela | Pesquisar restaurantes por especialidade ou localização | R02 — Não apresentar um restaurante que corresponde ao termo pesquisado | Particionamento de equivalência | CT01 e CT02 |


## Uso de inteligência artificial

**Ferramenta utilizada:** ChatGPT.

**Como foi utilizada:** A ferramenta foi utilizada como apoio na organização da documentação, estruturação das informações e revisão da clareza dos casos de teste.

**Uma sugestão que precisou ser alterada ou rejeitada:** Foi sugerido testar também uma pesquisa com o campo vazio, mas esse caso foi retirado para manter o foco nos três casos definidos para a funcionalidade escolhida.

**Como as respostas foram verificadas:** O conteúdo foi revisado com base nas orientações da atividade, nas funcionalidades informadas para o LocalEats e na relação entre funcionalidade, riscos, técnica escolhida e casos de teste.
