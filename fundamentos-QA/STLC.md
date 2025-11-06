# 🔁 Ciclo de Vida do Teste (STLC)

O Ciclo de Vida do Teste, ou **Software Testing Life Cycle (STLC)**, é o conjunto de etapas que guiam o processo de teste de software de forma estruturada. Cada fase tem objetivos e entregas específicas, garantindo que o sistema seja testado de maneira eficiente e que a qualidade seja validada desde o início do desenvolvimento até a entrega final.

### Diferença entre o STLC e o SDLC

Embora os dois ciclos de vida sejam semelhantes, pois ambos são geralmente descritos como tendo seis etapas e são centrados em um software, existem diferenças significativas entre o **STLC** e o **SDLC.**

A principal diferença entre esses dois ciclos de vida é que o **SDLC (Ciclo de Vida de Desenvolvimento de Software)** se concentra na criação de um software e no gerenciamento dos requisitos e responsabilidades associados a ele. Já o **STLC (Ciclo de Vida de Teste de Software)** se concentra em testar um software para encontrar e corrigir quaisquer defeitos que possam existir, atuando como um reflexo da maturidade e da qualidade em cada etapa do processo.

---

## 1️⃣ Planejamento de Testes

**Objetivo:** Definir a estratégia e o escopo dos testes para garantir que o processo seja organizado, mensurável e alinhado aos objetivos do projeto.

- Definição do escopo e dos objetivos dos testes.
- Seleção dos tipos e níveis de teste apropriados.
- Estimativa de esforço, recursos e cronograma.
- Definição dos critérios de entrada e saída.
- Escolha de ferramentas e definição do ambiente.
- Identificação de métricas e indicadores.

**Saídas:** Plano de teste, estratégia de teste, cronograma e estimativas.

---

## 2️⃣ Análise de Requisitos

**Objetivo:** Compreender e validar os requisitos para garantir que todos sejam claros, testáveis e livres de ambiguidades.

- Entendimento detalhado dos requisitos funcionais e não funcionais.
- Identificação de pontos críticos, riscos e dependências.
- Revisão junto ao time de desenvolvimento e ao Product Owner.
- Verificação da testabilidade dos requisitos.
- Criação de uma matriz de rastreabilidade inicial.

**Saídas:** Documento de análise, riscos identificados, matriz de rastreabilidade preliminar.

---

## 3️⃣ Design e Desenvolvimento de Casos de Teste

**Objetivo:** Criar casos de teste claros e completos que assegurem cobertura total dos requisitos e permitam detectar falhas com eficiência.

- Criação de cenários e casos de teste com base nos requisitos.
- Utilização de técnicas de design (particionamento de equivalência, valor limite, tabelas de decisão, etc.).
- Desenvolvimento de scripts de automação, se aplicável.
- Revisão e validação dos casos de teste por pares.
- Criação de dados e massa de teste.

**Saídas:** Casos de teste, dados de teste, scripts automatizados e matriz de rastreabilidade atualizada.

---

## 4️⃣ Configuração do Ambiente de Teste

**Objetivo:** Garantir que o ambiente de teste esteja corretamente configurado e represente as condições reais de uso do sistema.

- Configuração do ambiente onde os testes serão executados, garantindo que ele reflita as condições reais de uso do sistema.
- Instalação das versões corretas de software, dependências, bancos de dados e ferramentas necessárias.
- Criação ou carga dos dados de teste definidos na fase anterior.
- Verificação dos acessos, permissões, integrações e disponibilidade de serviços externos.
- Validação do ambiente com uma execução preliminar (smoke test) para confirmar estabilidade antes do início oficial dos testes.

**Saídas:** Ambiente configurado e validado, com acesso liberado para execução de testes.

---

## 5️⃣ Execução do Teste

**Objetivo:** Executar os testes planejados, registrar os resultados e reportar defeitos para garantir que o sistema funcione conforme esperado.

- Execução dos casos de teste planejados, manuais e/ou automatizados.
- Registro detalhado dos resultados obtidos (aprovado, reprovado, bloqueado, em andamento).
- Coleta e armazenamento das evidências de cada execução (prints, logs, vídeos, relatórios).
- Reporte imediato de defeitos identificados, com descrição clara, impacto, passos para reprodução e anexos.
- Acompanhamento das correções e reexecução dos testes (reteste e regressão) após cada ajuste.
- Atualização contínua da matriz de rastreabilidade, garantindo que cada requisito tenha sido devidamente validado.

**Saídas:** Relatórios de execução, defeitos documentados, evidências registradas e status de testes atualizados.

---

## 6️⃣ Encerramento do Teste

**Objetivo:** Avaliar os resultados, consolidar métricas e documentar aprendizados para garantir a melhoria contínua do processo de teste.

- Análise dos resultados globais, avaliando cobertura de testes, taxa de aprovação e criticidade dos defeitos encontrados.
- Verificação do cumprimento dos critérios de saída definidos no planejamento.
- Consolidação das métricas e indicadores de desempenho (taxa de defeitos, tempo médio de correção, cobertura funcional, etc.).
- Registro de lições aprendidas e identificação de oportunidades de melhoria para próximos ciclos.
- Elaboração do relatório final de testes, incluindo conclusão e recomendação sobre a liberação do sistema.
- Armazenamento de todos os artefatos de teste (casos, scripts, evidências e relatórios) em repositório versionado para rastreabilidade futura.

**Saídas:** Relatório final de testes, indicadores consolidados, lições aprendidas e encerramento formal do ciclo de testes.

---

## 🧩 Conclusão

O Ciclo de Vida do Teste é mais do que uma sequência de etapas - é um processo contínuo de aprendizado e aprimoramento.  
Cada fase influencia diretamente a qualidade final do produto e a satisfação do usuário.  
Um QA que compreende o STLC não apenas encontra erros, mas **ajuda a prevenir falhas e a construir software com propósito e valor.**