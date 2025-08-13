## Casos de uso UC03 - Manter anamnese

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