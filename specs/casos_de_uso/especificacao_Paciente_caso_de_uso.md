## Casos de uso  
**UC01 - Manter paciente**

---

### Objetivo  
Permitir que o ator efetue o cadastro, alteração, exclusão e consulta de pacientes.

### Requisitos  
RF001, RF002, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo

### Condição de entrada  
O ator acessa o módulo **Pacientes e Prontuários** e seleciona **Manter paciente** no menu.

---

### Fluxo principal  

1. O ator acessa a página de cadastro de pacientes.  
   Ele verifica que o título da página na aba do navegador e na própria página é **Cadastro de pacientes**.  
   Ele observa que existem campos para:
   - nome completo  
   - CPF  
   - certidão (nascimento ou casamento)  
   - data de nascimento  
   - telefone  
   - e-mail  
   - endereço completo (rua/avenida, número, bairro, cidade, CEP, ponto de referência)  
   - opções:
     - cadastrar  
     - cancelar  

2. O ator preenche os campos com os dados do paciente e seleciona o botão para cadastrar o paciente. [A2], [A3]  
3. O sistema verifica se as informações para cadastro são válidas. [RN1]  
4. O sistema exibe a página de cadastro de pacientes novamente e mostra uma mensagem informando que o paciente foi cadastrado com sucesso.  
5. O ator seleciona **Listar pacientes** no menu.  
6. O sistema exibe uma lista de pacientes cadastrados.  
7. O ator verifica que o paciente cadastrado está na lista.

---

### Fluxos alternativos  

**A1 - Buscar paciente**  
1. O ator deseja buscar um paciente na lista.  
2. Seleciona o campo específico de busca e digita o nome do paciente.  
3. Seleciona **Buscar**.  
4. O sistema exibe todos os pacientes que correspondem aos termos digitados.

**A2 - Editar paciente**  
1. O ator executa [A1].  
2. O ator seleciona o paciente na lista e clica no botão para editar.  
3. O sistema exibe a página de edição de pacientes, com os campos preenchidos com os dados do paciente.  
4. O ator altera os dados necessários e clica em **Salvar**.  
5. O sistema salva as alterações.  
6. O ator seleciona **Listar pacientes** no menu.  
7. O sistema exibe a lista de pacientes cadastrados.  
8. O ator verifica que as alterações foram aplicadas.

**A3 - Excluir paciente**  
1. O ator decide excluir um paciente e executa [A1].  
2. Ele visualiza o paciente e seleciona a opção **Excluir**.  
3. O sistema pergunta se o ator deseja confirmar a exclusão.  
4. O ator confirma a exclusão.  
5. O sistema exclui o paciente.  
6. O ator seleciona **Listar pacientes** no menu.  
7. O sistema exibe a lista de pacientes cadastrados.  
8. O ator verifica que o paciente não está mais na lista.

---

### Fluxos de exceção  

**RN1 - Validação de campos**  
Todas as informações são obrigatórias, exceto quando explicitamente marcadas como opcionais.

**RNF001** - Criptografar dados sensíveis.  
**RNF002** - Acesso restrito a usuários autorizados.  
**RNF016** - Registro em log de todas as operações.


**UC02 - Cadastrar dados do responsável legal**

---

### Objetivo  
Permitir o registro e a atualização dos dados do responsável legal do paciente.

### Requisitos  
RF013, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo

### Condição de entrada  
O ator acessa o cadastro do paciente e seleciona **Responsável legal** no menu.

---

### Fluxo principal  

1. O ator acessa a página de cadastro de responsável legal.  
2. O sistema exibe campos para:
   - nome completo  
   - CPF  
   - grau de parentesco  
   - contatos (telefone, e-mail)  
3. O ator preenche ou edita as informações.  
4. O ator seleciona **Salvar**.  
5. O sistema valida as informações. [RN1]  
6. O sistema confirma a operação e registra em log.

---

### Fluxos alternativos  

**A1 - Cancelar cadastro**  
1. O ator clica em **Cancelar**.  
2. O sistema retorna à tela anterior sem salvar as informações.

---

### Fluxos de exceção  

**RN1 - Validação de campos**  
Todos os campos são obrigatórios.  

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.


**UC03 - Manter anamnese**

---

### Objetivo  
Registrar e atualizar a anamnese clínica do paciente.

### Requisitos  
RF003, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário do paciente e seleciona **Anamnese**.

---

### Fluxo principal  

1. O ator acessa a página de anamnese.  
2. O sistema exibe campos para registro de histórico de saúde e condições atuais.  
3. O ator preenche ou edita as informações.  
4. O ator seleciona **Salvar**.  
5. O sistema valida as informações e registra a nova versão da anamnese. [RN1]  
6. O sistema confirma a operação.

---

### Fluxos alternativos  

**A1 - Cancelar edição**  
1. O ator clica **Cancelar**.  
2. O sistema descarta alterações e retorna à tela anterior.

---

### Fluxos de exceção  

**RN1 - Validação de campos**  
Todos os campos são obrigatórios.  

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.


**UC04 - Registrar diagnóstico**

---

### Objetivo  
Registrar diagnóstico clínico (texto e/ou documento anexo) no prontuário.

### Requisitos  
RF004, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário do paciente e seleciona **Diagnóstico**.

---

### Fluxo principal  

1. O ator acessa a página de diagnóstico.  
2. O sistema exibe campo de texto e opção de anexar laudo (PDF ou imagem).  
3. O ator preenche o diagnóstico e/ou anexa o documento. [E1]  
4. O ator seleciona **Salvar**.  
5. O sistema valida o formato/tamanho do arquivo. [RN1]  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Formato ou tamanho inválido**  
O sistema exibe mensagem de erro e solicita um novo envio.

**RN1 - Validação de campos**  
O diagnóstico em texto ou documento é obrigatório.  

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.


**UC05 - Manter PII**

---

### Objetivo  
Criar e editar o Plano de Intervenção Individualizado (PII) com metas, objetivos e estratégias terapêuticas.

### Requisitos  
RF005, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário e seleciona **PII**.

---

### Fluxo principal  

1. O ator acessa a página de PII.  
2. O sistema exibe campos para:
   - metas  
   - objetivos  
   - estratégias terapêuticas  
   - prazos  
3. O ator preenche ou edita as informações.  
4. O ator seleciona **Salvar**.  
5. O sistema registra a nova versão do PII. [RN1]  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**RN1 - Histórico de versões**  
O sistema deve manter versões anteriores e permitir restauração.  

**RNF004**, **RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

 
**UC06 - Visualizar histórico**

---

### Objetivo  
Exibir painel com o histórico clínico do paciente, incluindo anamnese, PII, sessões realizadas e documentos anexados.

### Requisitos  
RF009, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo (quando autorizado)

### Condição de entrada  
O ator acessa o prontuário do paciente e seleciona **Histórico**.

---

### Fluxo principal  

1. O ator acessa a página de histórico clínico.  
2. O sistema exibe resumos das seções do prontuário.  
3. O ator pode navegar entre abas ou aplicar filtros de período.  
4. O sistema atualiza as informações exibidas.  
5. O ator encerra a visualização.

---

### Fluxos de exceção  

**RNF002** - Respeitar permissões de acesso.  
**RNF001** - Criptografia dos dados.  
**RNF016** - Registro em log.


**UC07 - Registrar alta**

---

### Objetivo  
Gerar documento de alta com resumo terapêutico, objetivos alcançados e encerramento do PII, incluindo assinatura do paciente ou responsável.

### Requisitos  
RF010, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário e seleciona **Alta**.

---

### Fluxo principal  

1. O ator acessa a página de alta.  
2. O sistema exibe campos para resumo terapêutico e encerramento do PII.  
3. O ator preenche os campos e insere a assinatura (digitalizada ou eletrônica). [E1]  
4. O ator solicita **Gerar PDF**.  
5. O sistema valida, gera o documento e o registra no prontuário.  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Falha na geração ou assinatura**  
O sistema exibe mensagem de erro e mantém o documento em edição.

**RNF003**, **RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

 
**UC08 - Gerar relatório de procedimento**

---

### Objetivo  
Gerar ou anexar relatórios clínicos em PDF para compartilhamento com outros profissionais.

### Requisitos  
RF011, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário e seleciona **Relatórios**.

---

### Fluxo principal  

1. O ator escolhe entre:
   - **Gerar relatório**: preencher campos de texto livre e dados do paciente.  
   - **Anexar relatório**: selecionar um arquivo PDF existente.  
2. O ator confirma a ação. [E1]  
3. O sistema valida o conteúdo ou formato do arquivo.  
4. O sistema salva o relatório no prontuário.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Formato ou conteúdo inválido**  
O sistema informa o erro e solicita correção.

**RNF003**, **RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

 
**UC09 - Manter prontuário**

---

### Objetivo  
Administrar o prontuário do paciente, organizando documentos, evoluções e mídias.

### Requisitos  
RF006, RF007, RF008, RF014, RF015, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo (quando autorizado)

### Condição de entrada  
O ator acessa o prontuário do paciente.

---

### Fluxo principal  

1. O sistema exibe todas as seções do prontuário.  
2. O ator executa as ações necessárias:  
   - **UC14 – Anexar documentos** (<<include>>)  
   - **UC13 – Anexar vídeos** (<<include>>)  
   - **UC12 – Registrar evolução do paciente** (<<include>>)  
   - **UC10 – Arquivar prontuário** (<<include>>)  
   - **UC11 – Reaver prontuário arquivado** (<<include>>)  
3. O sistema aplica as permissões de acesso.  
4. O sistema registra as operações no log.

---

### Fluxos de exceção  

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

 
**UC10 - Arquivar prontuário**

---

### Objetivo  
Arquivar o prontuário de pacientes inativos, preservando o histórico.

### Requisitos  
RF014, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo (quando autorizado)

### Condição de entrada  
O ator abre o prontuário e seleciona **Arquivar**.

---

### Fluxo principal  

1. O sistema exibe mensagem de confirmação e efeitos da ação.  
2. O ator confirma a operação.  
3. O sistema altera o status para **Arquivado**.  
4. O sistema registra a operação no log e confirma.

---

### Fluxos de exceção  

**RNF002**, **RNF016**, **RNF001** aplicam-se integralmente.


**UC11 - Reaver prontuário arquivado**

---

### Objetivo  
Reativar o prontuário de um paciente arquivado.

### Requisitos  
RF015, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo (quando autorizado)

### Condição de entrada  
O ator pesquisa um paciente arquivado e acessa seu prontuário.

---

### Fluxo principal  

1. O sistema exibe opção para **Reativar prontuário**.  
2. O ator confirma a operação.  
3. O sistema altera o status para **Ativo**.  
4. O sistema registra no log e confirma.

---

### Fluxos de exceção  

**RNF002**, **RNF016**, **RNF001** aplicam-se integralmente.


**UC12 - Registrar evolução do paciente**

---

### Objetivo  
Registrar a evolução clínica do paciente, vinculada a uma sessão realizada.

### Requisitos  
RF007, RF016

### Atores  
Terapeuta

### Condição de entrada  
O ator acessa a aba **Evolução** no prontuário.

---

### Fluxo principal  

1. O sistema exibe campos para:
   - data da evolução  
   - sessão vinculada  
   - observações clínicas  
2. O ator preenche as informações.  
3. O ator seleciona **Salvar**.  
4. O sistema valida e salva a evolução.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.  
Relaciona-se ao **RNF006** quando a evolução é registrada automaticamente após a sessão.


**UC13 - Anexar vídeos**

---

### Objetivo  
Anexar vídeos de avaliação funcional ou motora ao prontuário.

### Requisitos  
RF008, RF016

### Atores  
Terapeuta

### Condição de entrada  
O ator acessa a aba **Vídeos** no prontuário.

---

### Fluxo principal  

1. O ator seleciona **Anexar vídeo**.  
2. Escolhe um arquivo nos formatos MP4 ou AVI, até 50 MB. [E1]  
3. O ator confirma o envio.  
4. O sistema valida o formato e o tamanho.  
5. O sistema salva com segurança e confirma.

---

### Fluxos de exceção  

**E1 - Arquivo inválido**  
O sistema exibe mensagem e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.

 
**UC14 - Anexar documentos**

---

### Objetivo  
Anexar documentos ao prontuário do paciente.

### Requisitos  
RF006, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo

### Condição de entrada  
O ator acessa a aba **Documentos** no prontuário.

---

### Fluxo principal  

1. O ator seleciona **Anexar documento**.  
2. Escolhe um arquivo nos formatos JPG, PNG ou PDF. [E1]  
3. O ator confirma o envio.  
4. O sistema valida e salva o arquivo.  
5. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Arquivo inválido ou falha de envio**  
O sistema informa erro e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.
