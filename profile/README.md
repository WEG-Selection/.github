<p align="center">
  <img src="assets/banner.svg" alt="WEG Selection — Gestão de oportunidades e indicação de aprendizes" width="100%" />
</p>
<p align="center">
  <strong>Uma plataforma para centralizar e acompanhar o processo de indicação de aprendizes às oportunidades da empresa.</strong>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-0B65B1?style=flat-square" alt="Status: em desenvolvimento" />
  <img src="https://img.shields.io/badge/projeto-integrador-0A3D75?style=flat-square" alt="Projeto Integrador" />
  <img src="https://img.shields.io/badge/IA-apoio%20%C3%A0%20decis%C3%A3o-18A6B7?style=flat-square" alt="IA como apoio à decisão" />
</p>
> **Projeto Integrador — CentroWEG** · Engenharia de Software
---
Visão geral
O WEG Selection é um sistema web corporativo criado para organizar o processo de encaminhamento de aprendizes para oportunidades nas áreas da empresa.
A plataforma reúne em um só lugar as informações sobre aprendizes, oportunidades, indicações, entrevistas e resultados. Assim, reduz a dependência de informações distribuídas em planilhas, e-mails e outros canais de comunicação, além de facilitar o acompanhamento de cada etapa.
O problema que queremos resolver
O encaminhamento de aprendizes exige analisar diferentes informações antes de realizar uma indicação, como:
desempenho técnico e acadêmico;
turma e situação do aprendiz;
áreas de interesse;
histórico de conversas com a coordenação;
requisitos da oportunidade;
resultados de entrevistas.
Quando essas informações ficam distribuídas em diferentes fontes, o processo pode se tornar mais trabalhoso, dificultando a comparação entre aprendizes e o acompanhamento das etapas posteriores à indicação.
A proposta
O WEG Selection centraliza os dados e organiza o fluxo de trabalho em etapas rastreáveis.
<p align="center">
  <strong>Oportunidade</strong> &nbsp; → &nbsp; <strong>Análise</strong> &nbsp; → &nbsp; <strong>Ranking</strong> &nbsp; → &nbsp; <strong>Recomendação</strong><br />
  ↓<br />
  <strong>Indicação</strong> &nbsp; → &nbsp; <strong>Entrevista</strong> &nbsp; → &nbsp; <strong>Resultado</strong> &nbsp; → &nbsp; <strong>Alocação</strong>
</p>
A Inteligência Artificial atua como recurso de apoio à decisão, sugerindo compatibilidades entre os requisitos de uma oportunidade e as informações disponíveis sobre os aprendizes. A decisão final permanece com o responsável pelo processo.
---
Como funciona
<table>
  <thead>
    <tr><th align="center">Etapa</th><th>O que acontece</th></tr>
  </thead>
  <tbody>
    <tr><td align="center"><strong>01 · Oportunidade</strong></td><td>O Autor do Processo cadastra no sistema a oportunidade recebida por canais externos, como e-mail ou Teams.</td></tr>
    <tr><td align="center"><strong>02 · Análise</strong></td><td>O coordenador consulta os aprendizes de seu escopo e analisa informações acadêmicas e de desempenho.</td></tr>
    <tr><td align="center"><strong>03 · Recomendação</strong></td><td>O sistema apresenta um ranking técnico e uma recomendação de compatibilidade baseada nos dados disponíveis.</td></tr>
    <tr><td align="center"><strong>04 · Indicação</strong></td><td>O coordenador avalia as informações e registra a indicação do aprendiz.</td></tr>
    <tr><td align="center"><strong>05 · Entrevista</strong></td><td>O Autor do Processo acompanha o agendamento e as informações necessárias para a entrevista.</td></tr>
    <tr><td align="center"><strong>06 · Resultado</strong></td><td>O resultado é registrado para que o processo avance para uma nova indicação ou para a etapa de alocação.</td></tr>
  </tbody>
</table>
Perfis de acesso
Perfil	Responsabilidades principais
Coordenador	Consultar turmas, aprendizes e dados acadêmicos; registrar conversas; consultar ranking e recomendações; realizar indicações e acompanhar o processo.
Autor do Processo	Cadastrar oportunidades; acompanhar indicações; organizar entrevistas; registrar retornos e resultados; consultar indicadores.
Gestão CTW	Acompanhar indicadores gerais, resultados e aprendizes aprovados dentro de seu escopo.
Administrador	Gerenciar usuários, permissões e acessos às funcionalidades.
> Gestores autorizados, como Luana e Sidney, podem acessar configurações administrativas e definir permissões dos usuários.
Funcionalidades previstas
🔐 Autenticação e controle de acesso;
👥 gerenciamento de usuários e permissões;
🎓 gerenciamento de turmas e aprendizes;
📊 consulta de dados acadêmicos e desempenho técnico;
💬 registro e histórico de conversas;
💼 cadastro e gerenciamento de oportunidades;
📈 ranking técnico de aprendizes;
🤖 recomendação de compatibilidade com apoio de IA;
📌 registro e acompanhamento de indicações;
📅 gerenciamento de entrevistas;
✅ registro de resultados;
📋 acompanhamento de alocações;
📊 indicadores e dashboards;
🧾 histórico e rastreabilidade das movimentações.
Arquitetura da aplicação
A aplicação separa as responsabilidades entre interface, API e persistência de dados. O front-end se comunica com o back-end por meio de uma API REST.
```text
┌──────────────────────────────────┐
│             FRONT-END            │
│       Next.js · React · TS       │
└────────────────┬─────────────────┘
                 │ HTTP / REST
                 ▼
┌──────────────────────────────────┐
│              BACK-END            │
│          Java · Spring Boot      │
│                                  │
│  Controllers · Services          │
│  Repositories · DTOs / Mappers   │
│  Segurança e autenticação        │
└────────────────┬─────────────────┘
                 │
                 ▼
┌──────────────────────────────────┐
│           BANCO DE DADOS         │
│               MySQL              │
└──────────────────────────────────┘
```
Tecnologias
<table>
  <thead><tr><th>Camada</th><th>Tecnologias</th></tr></thead>
  <tbody>
    <tr><td><strong>Back-end</strong></td><td>Java · Spring Boot · Spring Data JPA · Spring Security · Maven · OpenAPI / Swagger</td></tr>
    <tr><td><strong>Front-end</strong></td><td>Next.js · React · TypeScript</td></tr>
    <tr><td><strong>Banco de dados</strong></td><td>MySQL</td></tr>
    <tr><td><strong>Versionamento e planejamento</strong></td><td>Git · GitHub · GitHub Projects · Pull Requests · Conventional Commits</td></tr>
  </tbody>
</table>
Estrutura do back-end
A organização segue a separação por responsabilidades:
```text
src/
└── main/
    ├── java/
    │   └── .../
    │       ├── config/
    │       ├── controller/
    │       ├── dto/
    │       ├── entity/
    │       ├── error/
    │       ├── exception/
    │       ├── mapper/
    │       ├── repository/
    │       └── service/
    └── resources/
        └── application.properties
```
API REST
A API contempla recursos relacionados aos principais fluxos do sistema:
```text
/api/auth
/api/usuarios
/api/turmas
/api/aprendizes
/api/conversas
/api/oportunidades
/api/indicacoes
/api/entrevistas
/api/indicadores
/api/resultados
```
A documentação interativa dos endpoints será disponibilizada por meio do Swagger / OpenAPI.
Inteligência Artificial responsável
A IA do WEG Selection tem caráter assistivo. Ela pode analisar requisitos da oportunidade, desempenho técnico e acadêmico, pontos fortes, áreas de interesse e histórico de conversas registrado pela coordenação.
```text
Oportunidade
     ↓
Análise dos dados disponíveis
     ↓
Recomendação de compatibilidade pela IA
     ↓
Avaliação do coordenador
     ↓
Indicação registrada
```
A IA não seleciona nem indica aprendizes automaticamente. A recomendação é um recurso adicional para apoiar a análise humana, e não substitui a decisão do coordenador.
Organização do desenvolvimento
O projeto utiliza princípios de Scrum e acompanha o trabalho pelo GitHub Projects. A organização inclui Product Backlog, Sprint Backlog, Planning, Daily, Sprint Review, retrospectiva, Pull Requests e Code Review.
```text
Backlog
   ↓
Sprint Backlog
   ↓
In Progress
   ↓
Code Review
   ↓
In Testing / QA
   ↓
Done
```
Roadmap
MVP — Entrega 1: estrutura inicial e funcionalidades prioritárias para demonstrar o fluxo principal de oportunidades e indicação de aprendizes.
Entrega 2: evoluções e funcionalidades adicionais identificadas durante o desenvolvimento, a validação e o feedback dos stakeholders.
O roadmap poderá ser atualizado conforme novos requisitos, riscos e prioridades forem identificados.
Documentação do projeto
A documentação é organizada ao longo do desenvolvimento e contempla:
levantamento de demandas;
requisitos funcionais e não funcionais;
regras de negócio e matriz de rastreabilidade;
User Stories e critérios de aceitação;
diagramas UML e fluxos do processo;
arquitetura e protótipos;
ADRs e roadmap;
registros das cerimônias ágeis.
Recurso	Link
Fluxograma do processo	Adicionar o link definitivo do fluxograma
Planejamento do projeto	Adicionar o link do GitHub Projects
Documentação da API	Swagger / OpenAPI — disponível conforme a configuração do ambiente
Status do projeto
<p>
  <img src="https://img.shields.io/badge/WEG%20Selection-em%20desenvolvimento-0B65B1?style=for-the-badge" alt="WEG Selection em desenvolvimento" />
</p>
O desenvolvimento acontece de forma incremental, com validações periódicas de escopo e evolução contínua das funcionalidades.
Equipe
Projeto Integrador — Engenharia de Software  
Equipe responsável pelo desenvolvimento do WEG Selection no contexto do CentroWEG.
---
<p align="center">
  <sub>Projeto acadêmico desenvolvido para fins educacionais · CentroWEG</sub>
</p>
