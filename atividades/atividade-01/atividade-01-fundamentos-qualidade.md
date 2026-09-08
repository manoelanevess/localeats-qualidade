# Atividade 01 - Fundamentos e Características da Qualidade no LocalEats

## Tarefa 1 - Fundamentos da Qualidade

### Necessidades explícitas e implícitas

**Tipo:** Explícita
**Necessidade:** Permitir que o usuário entre no sistema utilizando e-mail e senha
**Interessado:** Usuário
**Consequência de não for atendida:** O usuário não conseguirá acessar sua conta e utilizar as funcionalidades vinculadas a ela

**Tipo:** Explícita
**Necessidade:** Permitir que um novo usuário crie uma conta
**Interessado:** Novo usuário
**Consequência de não for atendida:** O usuário não conseguirá se cadastrar para utilizar o sistema

**Tipo:** Implícita
**Necessidade:** Informar de forma clara o motivo de uma falha ao tentar entrar no sistema
**Interessado:** Usuário
**Consequência de não for atendida:** O usuário pode não entender o que ocorreu nem saber como corrigir o problema

**Tipo:** Implícita
**Necessidade:** Proteger as credenciais e os dados da conta contra acesso indevido
**Interessado:** Usuário e responsável pelo sistema
**Consequência de não for atendida:** Pode ocorrer comprometimento dos dados e perda de confiança na aplicação


### Análise

**Um sistema que implementa todas as funcionalidades explicitamente solicitadas pode, ainda assim, apresentar baixa qualidade? Justifique utilizando pelo menos uma necessidade implícita identificada.**

Sim. Um sistema pode implementar todas as funcionalidades solicitadas e ainda apresentar baixa qualidade. Por exemplo, o LocalEats pode permitir que o usuário entre em sua conta, mas, se uma falha ocorrer e a mensagem apresentada não explicar claramente o problema, o usuário pode não saber como resolvê-lo. Portanto, também é necessário atender às necessidades implícitas para oferecer uma boa experiência.

---

## Tarefa 2 - Exploração da Aplicação

**Integrante:** Manoela Neves
**Funcionalidade:** Buscar restaurantes 
**O que foi realizado:** Foi realizada uma busca por uma especialidade disponível no sistema ("Italiana") e uma busca utilizando um termo sem correspondência ("culinariaxyz").
**O que foi observado:** Nas duas buscas, o sistema apresentou a mensagem "Nenhum restaurante encontrado".
**Evidência:** manoela-busca-italiana.png e manoela-busca-semResultados.png

---

## Tarefa 3 - Requisitos e Características de Qualidade

**Integrante:** Manoela Neves
**Requisitos de Qualidade:** Ao pesquisar por uma especialidade disponível no sistema, o LocalEats deve apresentar os restaurantes correspondentes à busca.
**Características ou Subcaracterísticas:** Adequação funcional
**Justificativa:** A busca deve produzir resultados compatíveis com o critério informado pelo usuário. Durante a exploração, a busca por "Italiana", que é uma especialidade disponível no sistema, apresentou a mensagem "Nenhum restaurante encontrado".
**Como avaliar:** Realizar buscas utilizando especialidades disponíveis e verificar se os restaurantes correspondentes são apresentados corretamente.

---

## Uso de inteligência artificial

**Ferramenta utilizada:**  
ChatGPT

**Como foi utilizada:**  
A ferramenta foi utilizada como apoio para compreender as instruções da atividade e auxiliar na organização das respostas.

**Como as respostas foram verificadas:**  
As sugestões foram revisadas e comparadas com o comportamento observado durante a exploração do LocalEats e com os conteúdos estudados em aula.
