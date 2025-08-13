## Casos de uso UC46 - Definir tempo de upload

---

### Objetivo  
Permitir que o administrador possa definir o tempo máximo
permitido para upload de arquivos.

### Requisitos  
RF059

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona “Definir
tempo de upload”.
3.O sistema abre a página correspondente.
4.O ator visualiza o tempo atual configurado.
5.O ator define um novo tempo máximo.
6.O sistema salva a alteração e aplica aos envios de
arquivos. [MSG01]

---

### Fluxo Alternativo 

A1 - Sem alterações
- O ator acessa a página mas não muda a
configuração.

### Fluxos de Exceção

MSG02 - Erro na operação
- O sistema exibe mensagem de erro caso não seja
possível concluir a alteração.