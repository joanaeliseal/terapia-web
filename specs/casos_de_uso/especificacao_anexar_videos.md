## Casos de uso UC13 - Anexar vídeos

---

### Objetivo  
Anexar vídeos de avaliação funcional ou motora ao prontuário.

### Requisitos  
RF008, RF016

### Atores  
Terapeuta

### Condição de entrada  
O ator acessa a aba **Vídeos** no prontuário.

---

### Fluxo principal  

1. O ator seleciona **Anexar vídeo**.  
2. Escolhe um arquivo nos formatos MP4 ou AVI, até 50 MB. [E1]  
3. O ator confirma o envio.  
4. O sistema valida o formato e o tamanho.  
5. O sistema salva com segurança e confirma.

---

### Fluxos de exceção  

**E1 - Arquivo inválido**  
O sistema exibe mensagem e solicita novo envio.

**RNF001**, **RNF002**, **RNF016** aplicam-se integralmente.