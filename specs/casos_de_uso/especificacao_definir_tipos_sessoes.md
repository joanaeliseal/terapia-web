## Casos de uso UC38 - Definir tipos de sessões

---

### Objetivo  
Permitir que o administrador possa cadastrar, editar ou excluir os tipos de sessão disponíveis no sistema.

### Requisitos  
RF048

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona “Definir
tipos de sessões”.
3.O sistema abre a página “Definir tipos de sessões” com
título na aba e na página.
4.O ator visualiza a lista de tipos de sessão cadastrados.
5.O ator pode incluir novos tipos, editar existentes ou excluir
registros.
6.O sistema salva as alterações e atualiza a lista. [MSG01]
7.O ator confirma que a lista foi atualizada.

---

### Fluxo Alternativo 

A1 - Consulta sem alterações
- O ator acessa a página mas não realiza alterações.
- O sistema mantém a lista inalterada.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe mensagem de erro caso a operação não possa ser concluída.