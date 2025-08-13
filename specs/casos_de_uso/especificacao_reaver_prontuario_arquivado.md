## Casos de uso UC11 - Reaver prontuário arquivado

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