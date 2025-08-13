## Casos de uso UC39 - Manter convênio

---

### Objetivo  
Permitir que o administrador possa cadastrar, editar ou excluir convênios e planos de saúde aceitos pelo consultório.

### Requisitos  
RF049

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona “Manter
convênio”.
3.O sistema abre a página “Manter convênio” com título na
aba e na página.
4.O ator visualiza a lista de convênios cadastrados.
5.O ator pode incluir novos convênios, editar existentes ou
excluir registros.
6.O sistema salva as alterações e atualiza a lista. [MSG01]
7.O ator verifica que a lista está correta.

---

### Fluxo Alternativo 

A1 - Consultar sem alterar dados
- O ator acessa a página, mas não realiza alterações.
- O sistema mantém a lista inalterada.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.