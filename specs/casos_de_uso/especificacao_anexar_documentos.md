## Casos de uso UC14 - Anexar documentos

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
