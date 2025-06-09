<h1>Requisitos de Software</h1>

<h2>TerapiaWeb</h2>

<small>Versão 1.0</small>

## Histórico de revisões

|    Data    | Versão |           Descrição           |      Autor       |
| :--------: | :----: | :---------------------------: | :--------------: |
| 08/06/2025 |  1.0   |     Criação do documento      | Joana Elise, Jonata Barbosa, Matheus Barbosa, Leidiana Nascimento |

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

- [**RF001**] - Como TO, quero cadastrar um novo paciente com informações pessoais básicas, contendo nome, CPF, certidão de nascimento ou casamento, data de nascimento, telefone, e-mail.
- [**RF002**] - Como TO, quero registrar o endereço do paciente, incluindo localização para atendimento domiciliar. Deve incluir: rua ou avenida, número, bairro, cidade, CEP, ponto de referência.
- [**RF003**] - Como TO, quero registrar e atualizar a anamnese clínica do paciente com histórico de saúde e condições atuais.
- [**RF004**] - Como TO, quero registrar o diagnóstico clínico do paciente, com base em observações ou laudos médicos. Pode ser em formato de texto ou anexo de documento (laudo emitido por médicos).
- [**RF005**] - Como TO, quero gerar e editar o Plano de Intervenção Individualizado (PII), com metas, objetivos e estratégias terapêuticas ocupacionais.
- [**RF006**] - Como TO, quero anexar documentos (podendo ser atestados, laudos, autorizações) ao prontuário eletrônico do paciente em formato: JPG, PNG ou PDF.
- [**RF007**] - Como TO, quero registrar a evolução terapêutica do paciente a cada sessão realizada.
- [**RF008**] - Como TO, quero anexar vídeos de avaliação funcional ou motoras ao prontuário, com armazenamento seguro. Em formatos compatíveis como MP4 ou AVI, com limite de até 50MB por vídeo.
- [**RF009**] - Como TO, quero visualizar o histórico clínico completo do paciente por meio de um painel (dashboard) com resumos de anamnese, PII, sessões realizadas e documentos anexados.
- [**RF010**] - Como TO, quero registrar o documento de alta do paciente, contendo a assinatura do mesmo ou responsável (em caso de pacientes pediátricos), que contém um resumo terapêutico, objetivos alcançados e encerramento do PII. O documento pode ser exportado em formato PDF, com possibilidade de inserção de assinatura digital ou digitalizada.
- [**RF011**] - Como TO, quero anexar ou gerar relatórios do prontuário em formato PDF para compartilhar com médicos ou equipes multiprofissionais. Os relatórios são escritos em texto livre, com formato semelhante, contendo alguns dados pessoais do paciente (nome completo, idade, diagnóstico).
- [**RF013**] - Como TO, quero registrar os dados do responsável legal do paciente (em caso de menor de idade ou curatela). Deve conter nome completo, CPF, grau de parentesco, contatos.
- [**RF014**] - Como terapeuta ocupacional, quero arquivar o cadastro de pacientes que não estejam mais em acompanhamento ativo, seja por abandono, transferência ou alta terapêutica, para manter o sistema organizado sem perder o histórico de atendimentos realizados.
- [**RF015**] - Como TO, quero reaver prontuários arquivados, caso o paciente retorne ao acompanhamento.
- [**RF016**] - Como TO, quero que todos os prontuários do sistema sejam tratados como confidenciais por padrão, assegurando que apenas profissionais autorizados tenham acesso aos dados clínicos dos pacientes, em conformidade com a ética profissional e a LGPD.

### Módulo 2: Agendamento e Sessões
- [**RF017**]: Como TO, eu gostaria de agendar uma nova sessão para um paciente já cadastrado, contendo data, horário e duração, respeitando meus horários de trabalho configurados no sistema.
- [**RF018**]: Como TO, eu gostaria de poder editar uma sessão agendada, alterando data, horário, duração ou observações clínicas, desde de que a sessão não tenha sido marcada como realizada.
- [**RF019**]: Como TO, gostaria de adicionar o documento de evolução durante ou após a realização de uma sessão.
- [**RF020**]: Como TO, quero poder cancelar uma sessão já agendada, informando opcionalmente um motivo, mas mantendo a sessão no histórico do sistema com o status de “cancelada”.
- [**RF021**]: Como TO, gostaria de reservar tempo adicional antes ou depois de sessões domiciliares para deslocamento, e que esse tempo apareça como bloqueado na agenda.
- [**RF022**]: Como TO, gostaria de visualizar minhas sessões em um calendário, semanal ou mensal, ou uma lista cronológica.
- [**RF023**]: Como TO, quero pesquisar sessões por nome do paciente, data, status da sessão (realizada, agendada ou cancelada), tipo (presencial, domiciliar, teleatendimento), ou palavra-chave, para encontrar registros anteriores com maior facilidade.
- [**RF024**]: Como TO, gostaria de confirmar manualmente a realização da sessão no momento do atendimento, para que então o sistema possa registrar as informações no prontuário.
[remete ao RNF006]
- [**RF025**]: Como TO, quero poder informar o tipo de pagamento da sessão.
- [**RF026**]: Como TO, desejo reagendar uma sessão facilmente, apenas arrastando-a para outro horário ou selecionando uma nova data ou hora.
- [**RF027**]: Como TO, quero registrar a presença ou ausência do paciente na sessão, com opções como “presente”, “ausente”, “atrasado” ou “cancelado com aviso”.
- [**RF028**]: Como TO, desejo incluir observações confidenciais visíveis apenas a mim sobre o atendimento, separadas das anotações que entram no prontuário.
- [**RF029**]: Como TO, desejo duplicar sessões anteriores com base em frequência semanal ou quinzenal para pacientes em manutenção, para facilitar o agendamento de terapias recorrentes.
- [**RF030**]: Como TO, quero que o sistema permita gerar uma notificação ao paciente em caso de reagendamento ou cancelamento da sessão.
- [**RF031**]: Como TO, desejo bloquear horários específicos da minha agenda, para que o sistema não permita agendamento de sessões nesse período.

### Módulo 3: Financeiro e Convênios
- [**RF031**]:
- [**RF032**]: 
- [**RF033**]: 
- [**RF034**]: 
- [**RF035**]: 
- [**RF036**]: 
- [**RF037**]: 
- [**RF038**]: 
- [**RF039**]: 
- [**RF040**]: 
- [**RF041**]: 
- [**RF042**]: 
- [**RF043**]: 
- [**RF044**]: 
- [**RF045**]: 

### Módulo 4: Administração e Configurações
- [**RF046**]: Como administrador, quero criar, editar e excluir perfis de usuários (terapeuta ocupacional ou assistente administrativo), definindo suas permissões de acesso aos módulos do sistema.
- [**RF047**]: Como administrador, quero configurar os horários de atendimento padrão dos profissionais, para que os agendamentos respeitem as disponibilidades individuais.
- [**RF048**]: Como administrador, quero definir os tipos de sessão disponíveis (presencial, domiciliar, teleatendimento) e associar valores ou convênios vinculados.
- [**RF049**]: Como administrador, quero criar, editar e excluir convênios ou planos de saúde aceitos pelo consultório, vinculando cada um aos procedimentos e regras de faturamento.
- [**RF050**]: Como administrador, quero configurar regras de cobrança e repasse financeiro por profissional, para que o sistema calcule automaticamente os recebimentos de cada TO.
- [**RF051**]: Como administrador, quero visualizar um painel com indicadores gerenciais como número de pacientes ativos, sessões realizadas no mês, faturamento por convênio, entre outros.
- [**RF052**]: Como administrador, quero cadastrar diferentes clínicas ou locais de atendimento (multiunidades), para que os dados possam ser filtrados por unidade.
- [**RF053**]: Como administrador, quero configurar mensagens e lembretes automáticos que serão enviados aos pacientes por e-mail, SMS ou WhatsApp em caso de agendamento, reagendamento ou cancelamento.
- [**RF054**]: Como administrador, quero definir documentos e anexos obrigatórios para cada prontuário, tais como: anamnese, PII ou termo de consentimento.
- [**RF055**]: Como administrador, quero configurar alertas automáticos em caso de prontuários incompletos, sessões em atraso ou pagamentos vencidos.
- [**RF056**]: Como administrador, quero registrar e visualizar um log de atividades do sistema, com data e horário de ações como login, criação ou alteração de registros clínicos ou financeiros.
- [**RF057**]: Como administrador, quero configurar a marca e identidade visual da clínica (nome, logotipo, cores) para refletir nos relatórios e na interface do sistema.
- [**RF058**]: Como administrador, quero importar e exportar dados de usuários, pacientes e sessões via planilhas (CSV ou Excel), para facilitar integrações com outros sistemas.
- [**RF059**]: Como administrador, quero definir o tempo máximo permitido para upload de arquivos (documentos, vídeos), para evitar sobrecarga no servidor.
- [**RF060**]: Como administrador, quero definir níveis de acesso por seção do sistema (visualizar, editar, excluir), garantindo que apenas usuários autorizados possam modificar dados sensíveis.
- [**RF061**]: Como administrador, quero cadastrar e configurar templates de relatórios (prontuários, recibos, relatórios clínicos), para padronizar os documentos emitidos.

---

## Requisitos Não Funcionais

Os requisitos não-funcionais são descritos a seguir.

## Usabilidade
- [**RNF005**]: O sistema deve emitir alertas visuais ao terapeuta ao tentar finalizar ou arquivar um prontuário sem que documentos obrigatórios estejam anexados. São considerados obrigatórios: anamnese, Plano de Intervenção Individualizado (PII), termo de consentimento e evolução clínica.
- [**RNF020**]: Todas as alterações feitas nas configurações do sistema devem ser salvas automaticamente ou com confirmação explícita do usuário, com aviso visual de sucesso.
- [**RNF007**]: O sistema deve emitir alerta minutos antes de começar a sessão.
- [**RNF008**]: O sistema deve emitir alerta caso haja conflito de horários.
- [**RNF009**]:O sistema deve emitir alerta caso a sessão ultrapasse o tempo padrão.

## Confiabilidade
- [**RNF004**]: O sistema deve manter um histórico de versões do PII, com possibilidade de restaurar versões anteriores e substituir a atual.
- [**RNF010**]: O sistema deve manter agendamentos salvos mesmo com quedas de conexão.
- [**RNF012**]: O sistema deve permitir a realização de backups automáticos e periódicos, assegurando a integridade e a recuperação dos dados em caso de falhas.
- [**RNF016**]: O sistema deve manter um log de auditoria imutável e seguro com todas as ações realizadas pelos usuários, incluindo horário e IP de acesso.
- [**RNF017**]: O sistema deve permitir backup automático da configuração e das permissões de usuários semanalmente, com recuperação simples.

## Desempenho
- [**RNF003**]: O sistema deve permitir a exportação completa dos prontuários dos pacientes em formato PDF, contendo dados clínicos e documentos anexados, com tempo de geração inferior a 5 segundos, desde que não ultrapasse 50MB. Para prontuários extensos, o sistema deve permitir a exportação em partes ou por seções (anamnese, PII, evolução, documentos).
- [**RNF006**]: O sistema deve registrar automaticamente a sessão, após realizada, no prontuário do paciente, incluindo horário, duração, e notas do terapeuta.
- [**RNF011**]: O sistema deve estar disponível 24 horas por dia, 7 dias por semana, 365 dias por ano. 
- [**RNF014**]: O sistema deve suportar conexões simultâneas de múltiplos usuários, sem degradação significativa no desempenho ou na disponibilidade. 
- [**RNF019**]: O painel administrativo deve ter tempo de resposta inferior a 2 segundos para cada operação, mesmo com base de dados contendo até 10 mil registros ativos.

## Suportabilidade
- [**RNF013**]: O sistema deve ser compatível com múltiplos navegadores e sistemas operacionais, garantindo o acesso irrestrito por diferentes tipos de usuários. 
- [**RNF015**]: O sistema deve ser desenvolvido de forma que possa ser executado em qualquer dispositivo com conexão offline, e com posterior sincronização dos dados com o servidor.
- [**RNF018**]: O sistema deve permitir login via autenticação em dois fatores (2FA) para usuários com acesso administrativo.

## Requisito de Design / Implementação / Interface / Físico
- [**RNF001**]: O sistema deve criptografar todos os dados sensíveis armazenados nos prontuários dos pacientes. Os dados sensíveis incluem: nome completo, CPF, endereço, anamnese, diagnóstico, evolução, vídeos e documentos clínicos.
- [**RNF002**]: O sistema deve permitir acesso ao prontuário apenas por usuários autenticados com permissão adequada (nesse caso, o terapeuta ocupacional ou assistente administrativo). (permissões podem ser configuradas no módulo de administração - fazer referência a RF do módulo 4 que fala sobre isso).


Criado em Junho de 2025 por _Joana Elise, Jonata Barbosa, Matheus Barbosa e Leidiana Nascimento_.