# 🤖 Plano de Teste — Localiza Pesados

## 📘 Informações Gerais
- *Projeto:* Localiza Pesados  
- *Responsável:* Victor  
- *Data de Criação:* 2025-10-30  
- *Versão:* 1.0  

---

## 🎯 Objetivo
Validar o fluxo principal do usuário para localizar e solicitar locação de um veículo pesado (caminhão): acesso ao site, busca/listagem, visualização de detalhes do veículo e acionar contato/solicitação de locação.

---

## 📦 Resumo do Projeto
Aplicação web pública para consulta e solicitação de locação de veículos pesados. Testes cobrem funcionalidades de navegação, filtragem básica, visualização de detalhamento do veículo e acionamento do contato/solicitação.

---

## ⚙ Ambiente de Execução
- *Sistema Operacional:* Windows 10/11 (primário)  
- *Navegador / Versão:* Chrome (última); também testar em Edge/Firefox conforme necessidade 
- *Base de Dados:* Ambiente de homologação (staging) conectado ao backend de catálogo  
- *API / Serviços:* Endpoint de catálogo e endpoint de envio de contato/solicitação (staging)  
- *Ferramentas de Teste:* Manual (E2E), Chrome DevTools

---

## 🔗 Dependências e Pré-Requisitos
- Ambiente de homologação disponível e populado com catálogo de veículos  
- Endpoints de envio de contato/solicitação habilitados no ambiente de teste  
- Acesso à internet e máquinas com navegadores suportados

---

## 🏗 Níveis de Teste
- [ ] Unitário  
- [x] Integração (para API de catálogo/solicitação)  
- [x] Sistema / E2E (fluxo usuário)  
- [ ] Aceitação

---

## 🧩 Tipos de Teste
- [x] Funcional – valida fluxo de busca, detalhe e contato  
- [x] Regressão – scripts automatizados para verificar quebra do fluxo  
- [ ] Performance – (opcional) validar tempo de resposta da listagem em cargas maiores  
- [ ] Segurança – (opcional) validações básicas de sanitização de inputs  
- [x] Usabilidade – verificar presença de informações críticas no detalhe do veículo  
- [ ] Automatizado – Cypress E2E  
- [x] Manual – checklist de verificação visual e contato real

---

## 📋 Casos de Teste (detalhados)

Caso TST-001 — Acessar página inicial
- Pré-condição: ambiente staging disponível
- Passos:
  1. Acessar URL base do site (ex.: https://staging.localizapesados.com)
- Resultado esperado:
  - Página carregada sem erro 4xx/5xx
  - Campo/botão de busca e lista de veículos em destaques visível

Caso TST-002 — Buscar/listar veículos e selecionar 1 item (caminhão)
- Pré-condição: página inicial carregada
- Passos:
  1. Usar busca ou filtros para localizar caminhões
  2. Verificar que a listagem mostra pelo menos um caminhão
  3. Clicar no item desejado para abrir detalhes
- Resultado esperado:
  - Listagem presente com cards contendo nome, foto e preço/valor
  - Clique no item abre a página de detalhe

Caso TST-003 — Visualizar detalhes do caminhão
- Pré-condição: detalhe do produto aberto
- Passos:
  1. Verificar título, descrição, especificações técnicas, imagens e disponibilidade
  2. Verificar preço/tabela e condições de locação
- Resultado esperado:
  - Todos os campos essenciais visíveis e com dados consistentes
  - Imagens carregam com alt/text e navegação entre imagens funcional

Caso TST-004 — Entrar em contato / solicitar locação
- Pré-condição: detalhe do caminhão exibido
- Passos:
  1. Clicar em "Entrar em contato" ou "Solicitar locação"
  2. Preencher formulário de contato (nome, e-mail, telefone, mensagem) ou acionar CTA de contato (telefone / e-mail)
  3. Enviar formulário
- Resultado esperado:
  - Formulário validado (campos obrigatórios)
  - Ao enviar, receber confirmação de envio (mensagem de sucesso) e ver no backend/endpoint um registro de solicitação (ou e-mail simulado)
  - Não ocorrer erros de validação inesperados

Caso TST-005 — Fluxo negativo: formulário inválido
- Pré-condição: formulário de contato aberto
- Passos:
  1. Enviar formulário com campos obrigatórios vazios ou e-mail inválido
- Resultado esperado:
  - Mensagens de erro exibidas por campo
  - Envio bloqueado até correção dos campos

---

## ✅ Checklist de Aprovação do Plano
- [x] Projeto preenchido  
- [x] Níveis de teste selecionados  
- [x] Tipos de teste selecionados  
- [x] Casos de teste prontos  
- [ ] Métricas de QA incluídas (p.ex. tempo médio do fluxo, taxa de sucesso)  
- [ ] Registro de defeitos configurado (ex.: JIRA/GitHub Issues)

---

## 📊 Métricas e Critérios de Aceitação
- Tempo de carregamento da listagem: < 3s em ambiente de homologação (média)  
- Fluxo de solicitação: 100% de sucesso nas requisições em staging (sem erros 5xx)  
- Defeitos críticos: 0 bloqueadores antes de liberar para QA de aceitação

---

## 🔗 Links Úteis
- Repositório: (preencher)  
- Endpoint catálogo (staging): (preencher)  
- Endpoint contato/solicitação (staging): (preencher)  
- Relatório de bugs: (preencher)

---