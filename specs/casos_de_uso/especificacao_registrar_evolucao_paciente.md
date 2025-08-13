## Casos de uso UC12 - Registrar evolução do paciente

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