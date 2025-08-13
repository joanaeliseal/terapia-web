## Casos de uso UC08 - Gerar relatório de procedimento

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