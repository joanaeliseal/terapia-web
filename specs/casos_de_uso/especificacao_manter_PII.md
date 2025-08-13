## Casos de uso UC05 - Manter PII

---

### Objetivo  
Criar e editar o Plano de Intervenção Individualizado (PII) com metas, objetivos e estratégias terapêuticas.

### Requisitos  
RF005, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário e seleciona **PII**.

---

### Fluxo principal  

1. O ator acessa a página de PII.  
2. O sistema exibe campos para:
   - metas  
   - objetivos  
   - estratégias terapêuticas  
   - prazos  
3. O ator preenche ou edita as informações.  
4. O ator seleciona **Salvar**.  
5. O sistema registra a nova versão do PII. [RN1]  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**RN1 - Histórico de versões**  
O sistema deve manter versões anteriores e permitir restauração.  

**RNF004**, **RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.