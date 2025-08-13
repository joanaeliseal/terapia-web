## Casos de uso UC10 - Arquivar prontuário

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