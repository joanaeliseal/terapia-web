## Casos de uso UC43 - Definir documentos e anexos necessários

---

### Objetivo  
Permitir que o administrador possa definir documentos obrigatórios para o prontuário de pacientes.

### Requisitos  
RF054

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona “Definir
documentos e anexos necessários”.
3.O sistema abre a página correspondente com título na
aba e na página.
4.O ator visualiza a lista de documentos obrigatórios
definidos.
5.O ator pode adicionar, editar ou remover documentos e
anexos exigidos.
6.O sistema salva as alterações e aplica as regras de
obrigatoriedade. [MSG01]
7.O ator confirma que as alterações foram aplicadas.
---

### Fluxo Alternativo 

A1 - Consulta sem alterações
- O ator acessa a página, mas não realiza mudanças.
- O sistema mantém as configurações atuais.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.