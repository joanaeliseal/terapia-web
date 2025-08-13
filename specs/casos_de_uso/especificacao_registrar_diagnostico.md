## Casos de uso UC04 - Registrar diagnóstico

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