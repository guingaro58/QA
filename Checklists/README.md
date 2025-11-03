# 🧾 Checklist de Qualidade de Software (QA)

Este repositório tem como objetivo **compartilhar boas práticas e checklists essenciais** para garantir a qualidade em todas as etapas do ciclo de vida de testes.  
O objetivo é ajudar QAs (e times de desenvolvimento) a **não esquecer pontos críticos** que fazem diferença entre um teste “feito” e um **teste bem-feito** ✅

---

## 📋 Checklists

- [1️⃣ Planejamento de Testes](#-planejamento-de-testes)  
- [2️⃣ Preparação do Ambiente](#-preparação-do-ambiente)  
- [3️⃣ Execução dos Testes](#-execução-dos-testes)  
- [4️⃣ Registro e Evidências](#-registro-e-evidências)  
    - [🧩 Avaliação de Impacto do Bug](#-avaliação-de-impacto-do-bug)
- [5️⃣ Comunicação e Entrega](#-comunicação-e-entrega)  
- [6️⃣ Pós-Teste e Melhoria Contínua](#-pós-teste-e-melhoria-contínua)

---

## 1️⃣ Planejamento de Testes

Antes de começar a testar, garanta que tudo está **bem definido e compreendido**.

- [ ] O escopo dos testes está claro (o que será e o que **não será** testado)?  
- [ ] As **histórias de usuário** ou **requisitos** estão completos e compreensíveis?  
- [ ] Critérios de aceitação foram revisados e estão bem definidos?  
- [ ] Há **dependências externas** (APIs, integrações, dados, ambiente)?  
- [ ] A estratégia de testes foi definida (manual, automatizado, exploratório)?  
- [ ] Foram definidas **prioridades** (Smoke, Regressão, Sanidade, etc.)?  
- [ ] O cronograma de execução é realista e alinhado com o time?  

---

## 2️⃣ Preparação do Ambiente

Ambiente bem configurado = menos falsos positivos e retrabalho.

- [ ] O ambiente de teste está **estável** e atualizado com a versão correta?  
- [ ] Dados de teste foram criados ou validados?  
- [ ] Acesso aos sistemas e ferramentas foi testado (login, VPN, tokens)?  
- [ ] Logs e monitoramentos estão ativos (para facilitar análise de erros)?  
- [ ] Ferramentas de bug tracking (ex: Jira, Azure, Trello) estão configuradas?  
- [ ] Scripts ou pipelines de automação foram validados?  

---

## 3️⃣ Execução dos Testes

Hora de colocar a mão na massa — mas com método e registro!

- [ ] Casos de teste estão atualizados e revisados?  
- [ ] Foram priorizados os testes mais críticos?  
- [ ] Cada execução está sendo registrada com **status e evidências**?  
- [ ] Bugs estão sendo documentados e reportados de forma **clara e reprodutível**?  
- [ ] Testes negativos (validações de erro) estão sendo considerados?  
- [ ] O comportamento do sistema foi validado em diferentes **navegadores/dispositivos**?  
- [ ] Houve testes exploratórios para identificar cenários não mapeados?  

---

## 4️⃣ Registro e Evidências

Tudo que não é documentado, **não existe** em QA.

- [ ] Foram anexadas **capturas de tela** ou **gravações** das execuções?  
- [ ] Há logs ou prints dos erros ocorridos?  
- [ ] Cada bug possui **passos para reprodução**, **resultado esperado** e **resultado obtido**?  
- [ ] Evidências estão organizadas em pastas acessíveis ao time?  
- [ ] Foram gerados **relatórios de execução** ou métricas de cobertura?  

### 🧩 Avaliação de Impacto do Bug

- [ ] Ao registrar o bug, descreva **o impacto potencial** no sistema e no negócio.  
- [ ] Classifique o impacto em categorias:
  - 🔴 Crítico: perda financeira, falha em processo vital, vazamento de dados.  
  - 🟠 Alto: causa instabilidade, impede parte do fluxo principal.  
  - 🟡 Médio: afeta experiência, mas possui alternativa ou não bloqueia uso.  
  - 🟢 Baixo: erro visual, pequeno ajuste, texto incorreto.  
- [ ] Inclua no ticket: *“Impacto: perda de transação, instabilidade em módulo X, afeta 100% dos usuários.”*  
- [ ] Valide o impacto com o PO ou líder técnico, se houver dúvida.

---

## 5️⃣ Comunicação e Entrega

QA também é **colaboração e clareza**.

- [ ] Todos os bugs foram revisados antes de enviar para o dev?  
- [ ] A gravidade e prioridade estão bem classificadas?  
- [ ] O status dos testes foi comunicado ao time (Daily, Review, Retrospective)?  
- [ ] O ambiente de teste foi liberado com as devidas instruções?  
- [ ] Foram registradas observações ou riscos relevantes para o projeto?

---

## 6️⃣ Pós-Teste e Melhoria Contínua

Depois do ciclo de testes, vem o aprendizado.

- [ ] Houve análise de **métricas** (ex: taxa de bugs, tempo de correção)?  
- [ ] O time discutiu o que pode ser **melhorado no próximo ciclo**?  
- [ ] Casos de teste foram atualizados com base nos bugs encontrados?  
- [ ] Novas automações foram identificadas e priorizadas?  
- [ ] O repositório de testes está atualizado e versionado?  

---

## 🧠 Dica Extra

> “QA não é achar defeito, é garantir valor.”

Um checklist não serve apenas para lembrar tarefas — ele ajuda a criar **consistência e maturidade** no processo de qualidade.  
Adapte os itens conforme seu contexto (área de negócio, tipo de sistema, metodologia, etc.), e compartilhe melhorias com a comunidade   

---

📌 **Contribua!**  
Sinta-se à vontade para abrir um `Pull Request` com sugestões, novos checklists ou templates específicos (ex: mobile, API, automação, regressão).

