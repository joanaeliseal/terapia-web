## Casos de uso UC07 - Registrar alta

---

### Objetivo  
Gerar documento de alta com resumo terapêutico, objetivos alcançados e encerramento do PII, incluindo assinatura do paciente ou responsável.

### Requisitos  
RF010, RF016

### Atores  
Terapeuta 

### Condição de entrada  
O ator acessa o prontuário e seleciona **Alta**.

---

### Fluxo principal  

1. O ator acessa a página de alta.  
2. O sistema exibe campos para resumo terapêutico e encerramento do PII.  
3. O ator preenche os campos e insere a assinatura (digitalizada ou eletrônica). [E1]  
4. O ator solicita **Gerar PDF**.  
5. O sistema valida, gera o documento e o registra no prontuário.  
6. O sistema confirma a operação.

---

### Fluxos de exceção  

**E1 - Falha na geração ou assinatura**  
O sistema exibe mensagem de erro e mantém o documento em edição.

**RNF003**, **RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.