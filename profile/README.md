<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1220,50:123B66,100:1E6FB8&height=220&section=header&text=WEG%20Selection&fontSize=42&fontColor=F4F7FA&fontAlignY=38&desc=Sistema%20de%20gestão%20e%20seleção%20de%20aprendizes&descSize=16&descAlignY=58&descColor=F4F7FA" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code\&size=16\&pause=1000\&color=6FA8DC\&center=true\&vCenter=true\&width=700\&lines=Gestão+de+aprendizes+🎓;Seleção+orientada+por+dados+📊;Inteligência+Artificial+como+apoio+à+decisão+🤖;Projeto+Integrador+CentroWEG+💻)](https://git.io/typing-svg)

<br>

![Status](https://img.shields.io/badge/STATUS-EM%20DESENVOLVIMENTO-6FA8DC?style=flat-square\&labelColor=0B1220)
![Projeto](https://img.shields.io/badge/PROJETO-INTEGRADOR-1E6FB8?style=flat-square\&labelColor=0B1220)
![CentroWEG](https://img.shields.io/badge/CENTROWEG-INFORMÁTICA%20PARA%20INTERNET-6FA8DC?style=flat-square\&labelColor=0B1220)
![WEG](https://img.shields.io/badge/WEG-SELECTION-1E6FB8?style=flat-square\&labelColor=0B1220)

<br>

</div>

---

# 👋 Sobre o projeto

O **WEG Selection** é uma aplicação desenvolvida como **Projeto Integrador do CentroWEG**, criada para apoiar o processo de indicação e seleção de aprendizes para oportunidades dentro da empresa.

A plataforma centraliza informações que antes ficam distribuídas entre diferentes etapas do processo, permitindo acompanhar **oportunidades, aprendizes, indicações, entrevistas e resultados** em um único ambiente.

<br>

> **A IA recomenda. O coordenador decide.**

A Inteligência Artificial atua como apoio à análise de compatibilidade entre aprendizes e oportunidades, enquanto a decisão final permanece com o responsável pelo processo.

---

<br>

# 🎯 O problema

O processo de seleção de aprendizes envolve diferentes informações, pessoas e etapas.

A necessidade de consultar dados acadêmicos, acompanhar oportunidades, analisar o perfil dos aprendizes e registrar as decisões pode tornar o processo mais complexo e dificultar a rastreabilidade das informações.

O **WEG Selection** surge como uma proposta para centralizar esse processo e facilitar a tomada de decisão.

---

<br>

# 💡 A proposta

A plataforma reúne em um único sistema:

* 👥 Informações dos aprendizes
* 🎓 Dados acadêmicos e desempenho técnico
* 💼 Oportunidades disponíveis
* 📊 Ranking técnico dos aprendizes
* 🤖 Recomendações de compatibilidade por IA
* 📝 Histórico de conversas e acompanhamentos
* 📋 Indicações
* 🗓️ Entrevistas
* ✅ Resultados e alocações
* 📈 Indicadores do processo

---

<br>

# 🔄 Como funciona

```text
Oportunidade
     ↓
Cadastro no sistema
     ↓
Análise dos aprendizes elegíveis
     ↓
Ranking técnico
     ↓
Análise de compatibilidade por IA
     ↓
Avaliação do coordenador
     ↓
Indicação
     ↓
Entrevista
     ↓
Resultado
     ↓
Alocação
```

A recomendação gerada pela IA **não substitui a análise humana** e não impede que outros aprendizes sejam considerados.

---

<br>

# 👥 Perfis

### 👨‍💼 Coordenador

Responsável pela análise dos aprendizes e das oportunidades.

* Consulta aprendizes e turmas
* Visualiza desempenho acadêmico
* Consulta histórico de conversas
* Analisa rankings
* Consulta recomendações da IA
* Realiza indicações
* Acompanha o processo

### 📋 Autor do Processo

Responsável pela centralização e acompanhamento das oportunidades.

* Cadastra oportunidades
* Consulta indicações
* Agenda entrevistas
* Registra retornos
* Acompanha resultados
* Consulta indicadores

### 📊 Gestão CTW

Acompanha informações consolidadas do processo.

* Visualiza indicadores
* Consulta aprendizes aprovados
* Acompanha resultados da gestão

### ⚙️ Administrador

Responsável pelo gerenciamento dos usuários e permissões de acesso.

---

<br>

# 🤖 Inteligência Artificial

A IA é utilizada como **apoio à tomada de decisão**.

A análise considera informações relacionadas à oportunidade e ao perfil do aprendiz para gerar uma recomendação de compatibilidade.

```text
Oportunidade
     +
Dados técnicos
     +
Histórico
     +
Áreas de interesse
     ↓
Análise de IA
     ↓
Recomendação de compatibilidade
```

### ⚠️ Decisão humana

A IA **não seleciona, indica ou elimina aprendizes automaticamente**.

> **A IA recomenda. O coordenador decide.**

---

<br>

# 💻 Tecnologias

<p align="center">

<img src="https://skillicons.dev/icons?i=java,spring,mysql,maven,docker,react,ts,html,css,git,github,idea,vscode,figma" />

</p>

<p align="center">

<img src="https://img.shields.io/badge/REST%20API-123B66?style=for-the-badge"/>
<img src="https://img.shields.io/badge/JPA-1E6FB8?style=for-the-badge"/>
<img src="https://img.shields.io/badge/JUnit-6FA8DC?style=for-the-badge&logo=junit5&logoColor=0B1220"/>
<img src="https://img.shields.io/badge/Swagger-123B66?style=for-the-badge&logo=swagger&logoColor=white"/>

</p>

---

<br>

# 🏗️ Arquitetura

O sistema segue uma arquitetura baseada na separação de responsabilidades:

```text
┌──────────────────────────────┐
│          Front-end           │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│          REST API            │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│          Services            │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│         Repositories         │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│           MySQL              │
└──────────────────────────────┘
```

---

<br>

# 📚 Documentação

A documentação do projeto está organizada no repositório para facilitar o acompanhamento do desenvolvimento.

| Documento                    | Descrição                          |
| :--------------------------- | :--------------------------------- |
| 📋 Requisitos Funcionais     | Funcionalidades do sistema         |
| ⚙️ Requisitos Não Funcionais | Requisitos de qualidade            |
| 👤 User Stories              | Necessidades dos usuários          |
| 🗺️ Roadmap                  | Planejamento das entregas          |
| 🔄 Fluxogramas               | Processos e fluxos do sistema      |
| 🏗️ Arquitetura              | Estrutura técnica da aplicação     |
| 🗄️ Banco de Dados           | Modelo e estrutura dos dados       |
| 📖 API                       | Endpoints e contratos da aplicação |
| 📝 ADRs                      | Decisões arquiteturais             |

---

<br>
