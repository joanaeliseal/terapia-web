## Casos de uso UC09 - Manter prontuário

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