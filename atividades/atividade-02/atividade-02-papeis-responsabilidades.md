# Atividade 2 — Organização da Qualidade no LocalEats

## Tarefa 1 — Diagnóstico da situação

**Problema identificado:** Os critérios para considerar uma funcionalidade pronta não estão claramente definidos.  
**Possível consequência para o produto ou para a equipe:** Funcionalidades podem ser disponibilizadas sem atender a todos os requisitos ou sem passar pelas verificações necessárias, aumentando a possibilidade de defeitos chegarem aos usuários e gerando retrabalho para a equipe.

**Problema identificado:** Alguns integrantes consideram que somente o QA deve realizar testes.  
**Possível consequência para o produto ou para a equipe:** A responsabilidade pela qualidade fica concentrada em apenas um papel. Problemas que poderiam ser identificados durante o desenvolvimento acabam sendo encontrados somente mais tarde, tornando as correções mais demoradas.

**Problema identificado:** Os defeitos encontrados nem sempre são registrados e acompanhados.  
**Possível consequência para o produto ou para a equipe:** Problemas podem ser esquecidos, permanecer sem correção ou voltar a acontecer. Além disso, a equipe perde informações importantes sobre o histórico e a situação de cada defeito.

### A qualidade do LocalEats deve ser responsabilidade exclusiva do profissional de QA?

Não. A qualidade deve ser uma responsabilidade compartilhada por toda a equipe. O QA atua de forma especializada nos testes e na avaliação da qualidade, enquanto produto, desenvolvimento e liderança técnica também contribuem para prevenir defeitos e garantir que as funcionalidades atendam aos requisitos.


## Tarefa 2 — Papéis e competências

### Responsável pelo Produto

**Integrante:** Manoela
**Responsabilidades relacionadas à qualidade:** Definir e esclarecer requisitos, estabelecer critérios de aceitação, priorizar funcionalidades e defeitos e verificar se as entregas atendem às necessidades do produto e dos usuários.
**Competências técnicas:** Levantamento e análise de requisitos, definição de critérios de aceitação, priorização de backlog e conhecimento das funcionalidades do sistema.
**Competências comportamentais:** Comunicação, organização, tomada de decisão, negociação, empatia e visão do usuário.

### Desenvolvedor
**Integrante:** Manoela
**Responsabilidades relacionadas à qualidade:** Implementar as funcionalidades, realizar testes unitários, corrigir defeitos, participar das revisões de código e seguir os padrões técnicos definidos pela equipe.
**Competências técnicas:** Programação, Git, testes unitários, depuração de código e boas práticas de desenvolvimento.
**Competências comportamentais:** Colaboração, responsabilidade, atenção aos detalhes, comunicação e resolução de problemas.

### QA / Analista de Qualidade

**Integrante:** Manoela
**Responsabilidades relacionadas à qualidade:** Planejar e executar testes, elaborar cenários e casos de teste, verificar critérios de aceitação, registrar e acompanhar defeitos e comunicar riscos de qualidade à equipe.
**Competências técnicas:** Técnicas de teste, testes funcionais e exploratórios, criação de casos de teste, análise de requisitos e gerenciamento de defeitos.
**Competências comportamentais:** Pensamento crítico, atenção aos detalhes, comunicação, organização e colaboração.

### Liderança Técnica
**Integrante:** Manoela
**Responsabilidades relacionadas à qualidade:** Orientar decisões técnicas, garantir padrões de desenvolvimento, apoiar revisões de código, avaliar riscos técnicos e acompanhar a qualidade técnica das entregas.
**Competências técnicas:** Desenvolvimento de software, arquitetura, revisão de código, Git, integração de sistemas e boas práticas de desenvolvimento.
**Competências comportamentais:** Liderança, comunicação, pensamento analítico, tomada de decisão, colaboração e resolução de problemas.

### Justificativa dos papéis escolhidos

Os quatro papéis foram escolhidos porque possuem responsabilidades diferentes e complementares na construção da qualidade do LocalEats.

O **Responsável pelo Produto** contribui principalmente para a definição do comportamento esperado das funcionalidades e para a priorização das necessidades do sistema.

O **Desenvolvedor** atua diretamente na implementação das funcionalidades e na prevenção de defeitos por meio de boas práticas de programação, testes unitários e revisão de código.

O **QA / Analista de Qualidade** possui foco especializado na validação do sistema, planejando testes, identificando problemas e acompanhando defeitos.

A **Liderança Técnica** auxilia na garantia da qualidade técnica, orientando decisões de implementação, padrões de código e riscos relacionados às entregas.

## Tarefa 3 — Matriz de responsabilidades

### Legenda

**R — Responsável:** executa a atividade.  
**A — Aprovador:** responde pelo resultado final ou toma a decisão.  
**C — Consultado:** contribui antes da execução ou decisão.  
**I — Informado:** precisa conhecer o resultado.

| Atividade de qualidade | Responsável pelo Produto | Desenvolvedor | QA / Analista de Qualidade | Liderança Técnica |
|---|---|---|---|---|
| Definir critérios de aceitação | R/A | C | C | I |
| Revisar requisitos | A | C | R | C |
| Implementar a funcionalidade | I | R | I | A |
| Revisar o código | I | R | I | A |
| Criar testes unitários | I | R/A | C | C |
| Planejar e executar testes do sistema | C | C | R/A | I |
| Registrar e acompanhar defeitos | I | C | R/A | I |
| Priorizar a correção dos defeitos | R/A | C | C | C |
| Aprovar a disponibilização da versão | A | I | C | R |

## Lacuna ou conflito encontrado

**Lacuna ou conflito:** Não está claramente definido quem possui a responsabilidade de aprovar a disponibilização de uma nova versão do LocalEats.
**Possível consequência:** O responsável pelo produto, o QA e a liderança técnica podem interpretar que a decisão pertence a outro papel, fazendo com que uma versão seja disponibilizada sem uma aprovação claramente definida.
**Solução proposta:** A liderança técnica fica responsável por verificar se a versão possui condições técnicas para ser disponibilizada, enquanto o responsável pelo produto realiza a aprovação final. O QA participa como consultado, apresentando os resultados dos testes, defeitos encontrados e possíveis riscos da versão.

## Práticas recomendadas

### Prática 1 — Critérios de aceitação e Definition of Done

**Prática recomendada:** Definir critérios de aceitação e uma Definition of Done para as funcionalidades.
**Problema que ajuda a resolver:** A falta de clareza sobre quando uma funcionalidade pode ser considerada realmente concluída.
**Papéis envolvidos:** Responsável pelo Produto, Desenvolvedor, QA e Liderança Técnica.
**Como seria aplicada:** Antes de iniciar ou concluir uma funcionalidade, a equipe define quais condições precisam ser atendidas para que ela seja considerada pronta.

Na funcionalidade de busca do LocalEats, por exemplo, alguns critérios poderiam ser:

- permitir pesquisa por culinária;
- permitir pesquisa por localização;
- apresentar os restaurantes correspondentes à busca;
- informar quando nenhum resultado for encontrado;
- manter o funcionamento correto dos filtros.

Uma Definition of Done também poderia estabelecer que a funcionalidade só é considerada concluída quando:

- a implementação estiver finalizada;
- os critérios de aceitação forem atendidos;
- os testes necessários forem executados;
- a revisão de código for realizada;
- os defeitos críticos forem corrigidos.


### Prática 2 — Registro e acompanhamento de defeitos

**Prática recomendada:** Registrar e acompanhar de forma padronizada todos os defeitos encontrados.
**Problema que ajuda a resolver:** Defeitos identificados que não são registrados, acompanhados ou corrigidos adequadamente.
**Papéis envolvidos:** QA, Desenvolvedor, Responsável pelo Produto e Liderança Técnica.
**Como seria aplicada:** Sempre que um defeito for identificado, ele deve ser registrado com informações suficientes para que a equipe consiga reproduzir, corrigir e posteriormente testar novamente o problema.

O registro pode conter:

- título do defeito;
- funcionalidade afetada;
- descrição;
- passos para reprodução;
- resultado esperado;
- resultado obtido;
- severidade;
- prioridade;
- evidências;
- status;
- responsável pela correção.

Caso seja encontrado algum problema na busca, nos filtros, nos favoritos ou em outra funcionalidade do LocalEats, o defeito deve permanecer registrado até sua resolução e reteste.


## Exemplo de responsabilidade compartilhada no LocalEats

A funcionalidade de busca do LocalEats é um exemplo de como diferentes papéis podem contribuir para a qualidade.

**Responsável pelo Produto:** Define como a busca deve funcionar e estabelece os critérios de aceitação.
**Desenvolvedor:** Implementa a funcionalidade e realiza os testes técnicos necessários durante o desenvolvimento.
**QA / Analista de Qualidade:** Executa diferentes cenários de teste para verificar se a funcionalidade atende aos requisitos.

Alguns cenários poderiam ser:

- pesquisar uma culinária existente;
- pesquisar uma localização existente;
- realizar uma pesquisa sem resultados;
- pesquisar com o campo vazio;
- utilizar a pesquisa junto aos filtros disponíveis.

**Liderança Técnica:** Avalia a solução técnica, auxilia na revisão do código e verifica se a implementação segue os padrões definidos pela equipe.

Dessa forma, a qualidade não fica concentrada apenas no QA. Cada papel contribui em uma etapa diferente do desenvolvimento.


## Uso de inteligência artificial

**Ferramenta utilizada:** ChatGPT.

**Como foi utilizada:** A ferramenta foi utilizada como apoio na organização da documentação, revisão da redação e estruturação das informações da atividade.

**Como as respostas foram verificadas:** O conteúdo foi revisado com base nas orientações da atividade, nas funcionalidades do LocalEats e nas decisões tomadas para a organização dos papéis e responsabilidades.
