# Tech Career Mentor AI

<a href="https://github.com/sthefanyalaminos/tech-career-mentor/blob/main/README_EN.md">Translate to English</a>

> Sistema de orientação de carreira em tecnologia com dois agentes de IA encadeados — do autoconhecimento ao plano de ação.

---

## Sobre o Projeto

O **Tech Career Mentor AI** é um sistema multi-agente que guia o usuário desde a descoberta do seu perfil profissional até a criação de um roadmap de estudos personalizado em tecnologia.

O projeto foi desenvolvido como parte do aprendizado em desenvolvimento de sistemas e inteligência artificial, e utiliza dois agentes especializados que trabalham em sequência:

| Agente | Função |
|--------|--------|
| **Agent 1 - Entrevistador** | Conduz uma entrevista estruturada de 7 perguntas e sugere as 3 melhores carreiras em tech para o perfil do usuário |
| **Agent 2 - Planejador** | Recebe o perfil do Agent 1 e gera um plano completo de estudos com roadmap de 90 dias, projeto de portfólio e roteiro de entrevistas |

---

## Fluxo do Sistema

```
Usuário
   │
   ▼
┌─────────────────────────────────┐
│         AGENT 1                 │
│       Entrevistador             │
│                                 │
│  • 7 perguntas estruturadas     │
│  • Análise de perfil            │
│  • Ranking de 3 carreiras       │
└────────────────┬────────────────┘
                 │  handoff com dados do perfil
                 ▼
┌─────────────────────────────────┐
│         AGENT 2                 │
│        Planejador               │
│                                 │
│  • Visão do dia a dia           │
│  • Mapa de skills               │
│  • Roadmap de 90 dias           │
│  • Projeto de portfólio         │
│  • Roteiro de entrevistas       │
│  • Trilha DIO recomendada       │
└─────────────────────────────────┘
```

---

## Funcionalidades

### Agent 1 - Entrevistador de Carreira

- Entrevista conversacional com 1 pergunta por vez;
- Cobre: motivações, experiência prévia, disponibilidade, preferências de trabalho e objetivos;
- Aplica uma matriz de decisão interna (0–20 pontos) para ranquear carreiras;
- Apresenta as 3 carreiras com vantagens, desafios e contexto de mercado;
- Realiza o handoff estruturado de dados para o Agent 2.

### Agent 2 - Planejador de Roadmap

- Recebe os dados do perfil e personaliza o plano com base em:
  - Horas disponíveis por semana;
  - Nível de experiência (zero / iniciante / alguma);
  - Objetivo (primeiro emprego / transição / crescimento).
- Gera:
  - Visão do dia a dia na carreira escolhida;
  - Mapa de skills essenciais e complementares;
  - Roadmap detalhado de 90 dias (semana a semana);
  - Projeto de portfólio com entregáveis e critérios de aceitação;
  - Roteiro de entrevistas com 5 perguntas e como respondê-las;
  - Trilha DIO recomendada com próximos passos.

---
## Tecnologias e Conceitos Utilizados

- **Prompt Engineering** — Design de prompts estruturados com instruções de comportamento, fluxo condicional e formatação de output.
- **Arquitetura Multi-Agente** — Dois agentes com responsabilidades separadas e comunicação via handoff de dados.
- **UX Conversacional** — Fluxo de perguntas sequenciais para melhor experiência do usuário.

---
## Como Usar

1. Cole o prompt do **Agent 1** em seu ambiente de IA preferido (ChatGPT, Claude, Gemini, etc.).
2. Responda as 7 perguntas da entrevista.
3. Escolha uma das 3 carreiras sugeridas.
4. Cole o prompt do **Agent 2** em uma nova conversa, junto com os dados do handoff.
5. Receba seu plano de estudos personalizado.

---

## Autoria
Desenvolvido por Sthefany Alaminos, durante o Bootcamp CI&T – Do Prompt ao Agente, realizado pela DIO.