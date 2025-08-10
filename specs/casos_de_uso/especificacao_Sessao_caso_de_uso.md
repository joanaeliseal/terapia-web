**UC15 - Anexar vídeos**

---

### Objetivo  
Anexar vídeos de avaliação funcional ou motoras ao prontuário.

### Requisitos  
RF008, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa a aba **Vídeos** no prontuário.

---

### Fluxo principal  

1. O ator seleciona **Anexar vídeo**.  
2. Escolhe um arquivo nos formatos MP4 ou AVI, com limite de até 50MB. [E1]  
3. O ator confirma o envio.  
4. O sistema valida e salva o arquivo.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Arquivo inválido ou falha de envio**  
O sistema informa erro e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC16 - Visualizar histórico clínico**

---

### Objetivo  
Visualizar o histórico clínico completo do paciente.

### Requisitos  
RF009, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa o prontuário do paciente.

---

### Fluxo principal  

1. O sistema exibe painel (dashboard) com resumos de anamnese, PII, sessões realizadas e documentos anexados.

---

### Fluxos de exceção  
Não se aplica.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC17 - Registrar documento de alta**

---

### Objetivo  
Registrar o documento de alta do paciente.

### Requisitos  
RF010, RF016

### Atores  
Terapeuta

### Condição de entrada  
O ator acessa o prontuário do paciente.

---

### Fluxo principal  

1. O ator seleciona **Documento de alta**.  
2. Preenche resumo terapêutico, objetivos alcançados e encerramento do PII.  
3. Anexa assinatura digital ou digitalizada do paciente/responsável. [E1]  
4. O sistema gera documento em PDF.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Falha ao anexar assinatura**  
O sistema informa erro e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC18 - Anexar ou gerar relatórios**

---

### Objetivo  
Anexar ou gerar relatórios do prontuário.

### Requisitos  
RF011, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa a aba **Relatórios** no prontuário.

---

### Fluxo principal  

1. O ator escolhe **Anexar** ou **Gerar relatório**.  
2. Se anexar: escolhe arquivo PDF. [E1]  
3. Se gerar: escreve texto livre seguindo formato padrão.  
4. O sistema valida e salva.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Arquivo inválido ou falha de envio**  
O sistema informa erro e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC19 - Registrar dados do responsável legal**

---

### Objetivo  
Registrar os dados do responsável legal do paciente.

### Requisitos  
RF013, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa o cadastro do paciente.

---

### Fluxo principal  

1. O ator seleciona **Adicionar responsável legal**.  
2. Preenche nome, CPF, grau de parentesco e contatos. [E1]  
3. O sistema valida e salva.  
4. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Dados inválidos**  
O sistema informa erro e solicita correção.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC20 - Arquivar cadastro de paciente**

---

### Objetivo  
Arquivar o cadastro de pacientes inativos.

### Requisitos  
RF014, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa o cadastro do paciente.

---

### Fluxo principal  

1. O ator seleciona **Arquivar paciente**.  
2. O sistema solicita confirmação. [E1]  
3. O ator confirma.  
4. O sistema altera status para arquivado.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Operação cancelada pelo ator**  
O sistema mantém cadastro ativo.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC21 - Reativar prontuário arquivado**

---

### Objetivo  
Reativar prontuários arquivados.

### Requisitos  
RF015, RF016

### Atores  
Terapeuta, Assistente administrativo

### Condição de entrada  
O ator acessa lista de pacientes arquivados.

---

### Fluxo principal  

1. O ator seleciona prontuário arquivado.  
2. Solicita **Reativar**.  
3. O sistema solicita confirmação. [E1]  
4. O ator confirma.  
5. O sistema altera status para ativo.  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Operação cancelada pelo ator**  
O sistema mantém prontuário arquivado.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

---

**UC22 - Garantir confidencialidade dos prontuários**

---

### Objetivo  
Assegurar que todos os prontuários sejam confidenciais.

### Requisitos  
RF016

### Atores  
Sistema

### Condição de entrada  
O sistema está em operação.

---

### Fluxo principal  

1. O sistema restringe acesso a profissionais autorizados.  
2. Aplica criptografia e controle de permissões.

---

### Fluxos de exceção  
Não se aplica.

**RNF001**, **RNF002** aplicam-se integralmente.

---

**UC23 - Agendar sessão**

---

### Objetivo  
Agendar nova sessão para paciente cadastrado.

### Requisitos  
RF017, RF021, RF022, RF026, RF031, RNF007, RNF008, RNF009

### Atores  
Terapeuta

### Condição de entrada  
O ator acessa a agenda do sistema.

---

### Fluxo principal  

1. O ator seleciona paciente.  
2. Escolhe data, horário e duração. [E1]  
3. O sistema verifica disponibilidade.  
4. O sistema registra sessão na agenda.  
5. O sistema confirma agendamento.

---

### Fluxos de exceção  

**E1 - Horário indisponível**  
O sistema informa conflito e solicita nova escolha.

**RNF007**, **RNF008**, **RNF009** aplicam-se integralmente.
