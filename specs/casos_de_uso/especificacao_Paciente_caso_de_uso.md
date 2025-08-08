## Caso de uso  
**UC01 – Manter paciente**

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

**A1 – Buscar paciente**  
1. O ator deseja buscar um paciente na lista.  
2. Seleciona o campo específico de busca e digita o nome do paciente.  
3. Seleciona **Buscar**.  
4. O sistema exibe todos os pacientes que correspondem aos termos digitados.

**A2 – Editar paciente**  
1. O ator executa [A1].  
2. O ator seleciona o paciente na lista e clica no botão para editar.  
3. O sistema exibe a página de edição de pacientes, com os campos preenchidos com os dados do paciente.  
4. O ator altera os dados necessários e clica em **Salvar**.  
5. O sistema salva as alterações.  
6. O ator seleciona **Listar pacientes** no menu.  
7. O sistema exibe a lista de pacientes cadastrados.  
8. O ator verifica que as alterações foram aplicadas.

**A3 – Excluir paciente**  
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

**RN1 – Validação de campos**  
Todas as informações são obrigatórias, exceto quando explicitamente marcadas como opcionais.

**RNF001** – Criptografar dados sensíveis.  
**RNF002** – Acesso restrito a usuários autorizados.  
**RNF016** – Registro em log de todas as operações.
