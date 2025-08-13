## Casos de uso UC02 - Cadastrar dados do responsável legal

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