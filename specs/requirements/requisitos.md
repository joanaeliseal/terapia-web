<h1>Requisitos de Software</h1>

<h2>TerapiaWeb</h2>

<small>Versão 1.0</small>

## Histórico de revisões

|    Data    | Versão |           Descrição           |      Autor       |
| :--------: | :----: | :---------------------------: | :--------------: |
| 25/05/2025 |  1.0   |     Criação do documento      | Joana Elise, Jonata Barbosa, Matheus Barbosa, Leidiana Nascimento |
| 08/06/2025 |  1.1   | Adição de novas informações | Joana Elise, Jonata Barbosa, Matheus Barbosa, Leidiana Nascimento |

---

## Introdução

Este documento descreve os requisitos do sistema **TerapiaWeb**, uma aplicação voltada à gestão de atendimentos e informações clínicas em consultórios de Terapia Ocupacional. O sistema será acessado por terapeutas ocupacionais, assistentes administrativos (se houver) e administradores do sistema.

---

## Definições, Acrônimos e Abreviações

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

- Identificação dos requisitos: por convenção, a referência a requisitos é feita através do identificador de requisitos, de acordo como descrito abaixo:

  `[IDENTIFICADOR DO TIPO DE REQUISITOS]`

  O identificador do tipo de requisitos é conforme abaixo:

  - RF – Requisito Funcional
  - RNF – Requisito Não-Funcional

  O identificador do requisito será uma sequência numérica. Esse número sequencial será único para todo o conjunto de tipos de requisitos.

  **Exemplo**: RF0001, RF1234, RNF1234.

# Usuários identificados

Os seguintes usuários foram identificados para o sistema:

- Usuário do sistema
  - Usuários comuns
    - Terapeuta Ocupacional (TO): responsável por realizar os atendimentos e registrar informações clínicas.
    - Assistente Administrativo (opcional): auxilia no agendamento de sessões, controle de cadastros e documentos.
  - Administrador do Sistema: gerencia usuários, permissões, configurações gerais e backups do sistema.

### Abreviações

| Termo | Definição                                    |
| :---: | -------------------------------------------- |
|  TO   | Terapeuta Ocupacional                        |
| LGPD  | Lei Geral de Proteção de Dados (Lei nº 13.709/2018)     |
| PII   | Plano de Intervenção Individualizado         |
| TCLE  | Termo de Consentimento Livre e Esclarecido   |
| PDF   | Portable Document Format                     |
| JPG / PNG  | Joint Photographic Experts Group / Portable Network Graphics   |
| MP4 / AVI  | MPEG-4 Part 14 / Audio Video Interleave   |

---

## Requisitos Funcionais

Os requisitos funcionais são descritos a seguir.

### Módulo 1: Pacientes e Prontuários

- **RF000** - Como TO, quero cadastrar um novo paciente com informações pessoais básicas, contendo nome, CPF, certidão de nascimento ou casamento, data de nascimento, telefone, e-mail.
- **RF001** - Como TO, quero registrar o endereço do paciente, incluindo localização para atendimento domiciliar. Deve incluir: rua ou avenida, número, bairro, cidade, CEP, ponto de referência.
- **RF002** - Como TO, quero registrar e atualizar a anamnese clínica do paciente com histórico de saúde e condições atuais.
- **RF003** - Como TO, quero registrar o diagnóstico clínico do paciente, com base em observações ou laudos médicos. Pode ser em formato de texto ou anexo de documento (laudo emitido por médicos).
- **RF004** - Como TO, quero gerar e editar o Plano de Intervenção Individualizado (PII), com metas, objetivos e estratégias terapêuticas ocupacionais.
- **RF005** - Como TO, quero anexar documentos (podendo ser atestados, laudos, autorizações) ao prontuário eletrônico do paciente em formato: JPG, PNG ou PDF.
- **RF006** - Como TO, quero registrar a evolução terapêutica do paciente a cada sessão realizada.
- **RF007** - Como TO, quero anexar vídeos de avaliação funcional ou motoras ao prontuário, com armazenamento seguro. Em formatos compatíveis como MP4 ou AVI, com limite de até 50MB por vídeo.
- **RF008** - Como TO, quero visualizar o histórico clínico completo do paciente por meio de um painel (dashboard) com resumos de anamnese, PII, sessões realizadas e documentos anexados.
- **RF009** - Como TO, quero registrar o documento de alta do paciente, contendo a assinatura do mesmo ou responsável (em caso de pacientes pediátricos), que contém um resumo terapêutico, objetivos alcançados e encerramento do PII. O documento pode ser exportado em formato PDF, com possibilidade de inserção de assinatura digital ou digitalizada.
- **RF010** - Como TO, quero anexar ou gerar relatórios do prontuário em formato PDF para compartilhar com médicos ou equipes multiprofissionais. Os relatórios são escritos em texto livre, com formato semelhante, contendo alguns dados pessoais do paciente (nome completo, idade, diagnóstico).
- **RF011** - Como TO, quero registrar os dados do responsável legal do paciente (em caso de menor de idade ou curatela). Deve conter nome completo, CPF, grau de parentesco, contatos.
- **RF012** - Como terapeuta ocupacional, quero arquivar o cadastro de pacientes que não estejam mais em acompanhamento ativo, seja por abandono, transferência ou alta terapêutica, para manter o sistema organizado sem perder o histórico de atendimentos realizados.
- **RF013** - Como TO, quero reaver prontuários arquivados, caso o paciente retorne ao acompanhamento.
- **RF014** - Como TO, quero que todos os prontuários do sistema sejam tratados como confidenciais por padrão, assegurando que apenas profissionais autorizados tenham acesso aos dados clínicos dos pacientes, em conformidade com a ética profissional e a LGPD.

### Módulo 2: Agendamento e Sessões

### Módulo 3: Financeiro e Convênios

### Módulo 4: Administração e Configurações
---

## Requisitos Não Funcionais

Os requisitos não-funcionais são descritos a seguir.

