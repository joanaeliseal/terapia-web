# 🧠 TerapiaWeb

**TerapiaWeb** é um sistema web desenvolvido como projeto da disciplina de **Análise e Projeto de Sistemas (APS)** no curso de Tecnologia em Sistemas para Internet – IFPB. O objetivo é atender às demandas de terapeutas ocupacionais autônomos, oferecendo uma plataforma organizada, segura e acessível para gerenciar pacientes, prontuários, sessões e dados administrativos.

---

## 📁 Estrutura de Pastas

A organização do projeto segue a estrutura proposta pela disciplina, com pastas voltadas à documentação, análise e modelagem:

```
/                                   # Raiz do projeto
├── .git/                           # Criado automaticamente pelo Git
├── specs/                          # Especificações do projeto
│   └── casos-de-uso/
│       ├── analise_casos_de_uso.png          
│       ├── especificacao_Administracao_caso_de_uso.md                
│       └── especificacao_Financeiro_caso_de_uso.md
│       └── especificacao_Paciente_caso_de_uso.md        
│       └── especificacao_Sessao_caso_de_uso.md    
│   └── logica/                     
│       └── analise_logica_diagrama_classes.md  # Diagrama de Classes
│       └── arquivos com diagramas de atividades dos métodos das classes 
│   └── requirements/
│       ├── entrevista.pdf          # Formulário de entrevista com o cliente
│       ├── visao.md                # Documento de Visão do Sistema
│       └── requisitos.md           # Documento de Requisitos (Funcionais e Não Funcionais)
│
├── ui/                             # Interfaces visuais de baixa fidelidade (protótipos)
│   ├── 01-dashboard.pdf            # exemplo 1
│   └── 02-cadastro-usuario.pdf     # exemplo 2
│
├── design/                         # Artefatos de análise e projeto de sistemas
│   ├── ui/                         # Interface visual de alta fidelidade (ex: Figma)
│   ├── logic-vision/               # Visão lógica do sistema
│   └── use-case-vision/            # Visão de casos de uso
│
└── src/                            # Código-fonte (não será desenvolvido nesta fase)
```

---

## 📌 Visão Geral

TerapiaWeb visa facilitar o gerenciamento das atividades diárias dos profissionais de Terapia Ocupacional, promovendo uma melhor organização de dados clínicos e administrativos. O sistema será documentado e modelado com foco em boas práticas de engenharia de software, mas **não contará com a implementação do código nesta disciplina**.

---

## 🔍 Módulos Planejados

O sistema está dividido em quatro módulos principais:

1. **Pacientes e Prontuários**
2. **Agendamento e Sessões**
3. **Financeiro e Convênios**
4. **Administração e Configurações**

---

## 📝 Documentação

Os documentos obrigatórios estão sendo produzidos em formato `.md` ou `.pdf` e organizados conforme solicitado:

- **Entrevista com o cliente** – `entrevista.pdf`
- **Documento de Visão** – `visao.md`
- **Documento de Requisitos** – `requisitos.md`
- **Protótipos de baixa fidelidade** – arquivos `.pdf` exportados do Figma
- **Artefatos de análise** – diagramas e descrições lógicas e de casos de uso

---
## 📊 Artefatos de Análise e Modelagem

Durante a disciplina foram produzidos diversos diagramas para apoiar a especificação do sistema:

- **Diagramas de Casos de Uso** – visão geral dos módulos.
- **Especificação detalhada de Casos de Uso** – descrição textual no formato padrão, por módulo.
- **Diagrama de Classes** – visão estrutural do sistema.
- **Diagramas de Atividades** – fluxos detalhados de cada método das classes.
- **Relacionamento entre Módulos** – integração entre classes e módulos.
---

## 🛠 Diagramas de Atividades

Cada método das classes principais foi detalhado por meio de um **Diagrama de Atividades UML**.  
O objetivo é facilitar a compreensão do fluxo de execução e das decisões envolvidas, antes da implementação.

**Padrões adotados:**
- Símbolos de decisão com losango e fundo branco.
- Representação de retornos como nós de junção (merge).
- Atividades com cantos arredondados por módulo.
---

## 👩‍💻 Equipe

Projeto desenvolvido por estudantes do IFPB – Campus João Pessoa:

- [Joana Elise](https://github.com/joanaeliseal)  
- [Jonata Barbosa](https://github.com/iamjonn)
- [Leidiana Nascimento](https://github.com/Leidianapatricio)
- [Matheus Barbosa](https://github.com/themattery)

---

## 📚 Disciplina

📘 **Análise e Projeto de Sistemas (APS)**  
🗓 Período: 2025.1  
🎓 Curso: Tecnologia em Sistemas para Internet – IFPB  
👩‍🏫 Professor: [Maxwell Anderson](https://github.com/maxwellamaral)

---

## 📌 Observações

- O projeto está em fase de levantamento, análise e documentação.
- A implementação do sistema poderá ser realizada em disciplinas futuras.

---
