# Desafio #02: Estruturando a Área de Testes da Empresa

Este portfólio é o resultado do Desafio #2: Estruturação da Área de Testes da Empresa, parte da **Mentoria M2.0 em Testes de Software do Júlio de Lima.**
O objetivo central foi definir e formalizar os processos de QA para uma nova área de testes na empresa "Clebinho Soluções em Pagamentos". Fomos contratados como os primeiros QAs e encarregados de estruturar a área do zero, definindo as atividades de teste a serem realizadas, os responsáveis por cada atividade, o momento (sequência) de execução de cada processo e as ferramentas e dependências necessárias.

A coleta dessas informações serviram para estruturar os seguintes processos:
1. Refinamento focado em testes
2. Modelagem de testes
3. Execução com gestão de defeitos
4. Automação

### 📌**Foco e Contexto Técnico**
* **Ambiente:** 5 times ágeis, todos construindo apenas APIs.
* **Recursos:** Times compostos por Desenvolvedores Seniores, POs e Scrum Masters.
* **Processos Estruturados:** Refinamento focado em testes, modelagem de testes, execução com gestão de defeitos e automação.

---
### 💡**Abordagem e Metodologia**

Neste desafio, aplicamos os conhecimentos e a mentalidade de testes de software discutidos na mentoria ao longo dos módulos 1 ao 4, com foco em estruturar processos que garantam a qualidade e a colaboração entre QA, PO e Desenvolvedores.

### 📄**Resultado Final da Estruturação de Área de Testes**

### 1. Estrutura do Processo de Refinamento Focado em Testes

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
| :--- | :--- | :--- | :--- | :--- |
| **Entender e revisar regras de negócios** e critérios de aceite nas *user stories* | Assim que o PO finaliza a escrita das *user stories* e antes do refinamento | Objetivo e regras de negócio definidas pelo PO | Jira, Trello | QA e PO |
| **Identificar cenários de integração** com outros sistemas e dependências externas | Durante o refinamento, antes do início do desenvolvimento | Documentação de APIs e sistemas integrados | Postman, Swagger | QA + Dev |
| **Elaborar o plano de testes** e abordagem (Manual e Automatizados) | Após o refinamento da *User Story* | Critérios de aceites claros na *user story* | Jira | QA |
| **Verificar se há critérios para execução de testes não funcionais** (performance, segurança, etc) que precisam ser refinados | Durante o refinamento | Regras claras na *User Stories* | Jira, Trello | QA + PO + DEV |
| **Mapear riscos e priorizar cenários de teste** | Durante o refinamento, antes da modelagem dos testes | Critérios de aceitação e entendimento da regra de negócio | Jira, Trello | QA + PO + DEV |

---

### 2. Estrutura do Processo de Modelagem de Testes

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
| :--- | :--- | :--- | :--- | :--- |
| **Definir as técnicas de testes** a serem utilizadas para a verificação do cumprimento dos requisitos | Após a agenda de refinamento e compreensão das regras de negócio | Refinamento realizado com sucesso | Blocos de texto, planilhas | QA |
| **Documentar cenários em formato Gherkin** (Given/When/Then) | Após definição dos critérios de aceite | Critérios definidos | Jira, Bloco de notas | QA |
| **Gerar artefatos de testes** (caso de teste, Log de teste e etc) para metrificar os testes | Após os testes serem realizados | Testes realizados | Word, Bloco de nota | QA |
| **Definir prioridade dos testes** baseado em risco e criticidade | Após o refinamento, quando os cenários de teste estão definidos | Análise de riscos | Planilhas | QA |
| **Definir dados de teste** necessários para execução | Após definição e priorização dos cenários | Casos de teste documentados e fluxos de entrada/saída definidos | Planilhas, Banco de dados (SQL) | QA |

---

### 3. Estrutura do Processo de Execução com Gestão de Defeitos

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
| :--- | :--- | :--- | :--- | :--- |
| **Registrar card de defeito** no *board* do time (Descrição, Passo a Passo, Resultado Obtido/Esperado, Evidência) | Após a execução de um teste que obteve o resultado fora do esperado | *Board* para o controle e gestão de defeitos encontrados | Jira, Trello | QA |
| **Retestar funcionalidades** após correções aplicadas pelos *devs* | Após o *bug* ser corrigido e registrado no *board* | Correção entregue no *board* | Jira, Trello | QA |
| **Classificar a severidade e prioridade** dos defeitos encontrados | Após registrar o defeito no *board* | Defeito reportado | Jira | QA + PO |
| **Acompanhar status dos defeitos** até a resolução | Após a correção | Defeitos registrados no *board* | Jira, Trello | QA |

---

### 4. Estrutura do Processo de Automação

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
| :--- | :--- | :--- | :--- | :--- |
| **Identificar cenários automatizáveis (APIs)** | Antes da agenda de *planning* do time | *User stories* priorizadas | Jira, Trello, Bloco de texto | QA |
| **Criar scripts de automação e versionar** no repositório | Após levantamento dos cenários automatizáveis | Ambiente Configurado | Supertest, Postman, GitHub | QA |
| **Executar a suíte de testes de regressão de API** | Após uma nova versão ser gerada no ambiente de teste | Scripts de automação existente, Ambiente de testes configurado e com nova versão | Supertest, Github | QA |
| **Configurar geração de relatórios automatizados** | Após criação dos scripts e definição do ambiente de testes | Scripts automatizados funcionando corretamente | Mochawesome, Mocha, Node.js | QA |
| **Revisar cobertura de automação** (cenários automatizados vs. backlog) | Periodicamente (fim de *sprint* ou *release*) | Relatórios de execução e backlog atualizado | Jira, planilhas | QA + PO |
---

### 📖**Notas Adicionais**
* Pode-se notar que a definição dos responsáveis para algumas atividades incluem também o PO e DEV, pois são super importantes para a colaboração na execução de algumas atividades visando o processo de qualidade dentro do time. Isso é evidente na atividade definição da prioridade de correção de defeitos com base em sua severidade no processo de execução com gestão de defeitos, onde a visão do PO é crucial para junto à análise do QA.

### 🧠**Participantes do Desafio**

- Claudianne Vieira ([Link do LinkedIn](https://www.linkedin.com/in/claudianne-vieira/))
- Danielle Lopes([Link do LinkedIn](https://www.linkedin.com/in/danielle-c-s-lopes/))
- Leonam Galvão, ([Link do LinkedIn](https://www.linkedin.com/in/leonamg/))
- Thais Moreira ([Link do LinkedIn](https://www.linkedin.com/in/thais-moreira/))
  
### 📌README.md por:
👩🏽‍💻 Ilana Alcantara ([Link do LinkedIn](https://www.linkedin.com/in/ilana-alcantara/))
