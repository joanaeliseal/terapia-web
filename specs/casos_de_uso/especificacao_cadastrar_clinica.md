## Casos de uso UC42 - Cadastrar clínica

---

### Objetivo  
Permitir que o administrador possa cadastrar novas clínicas ou
locais de atendimento.

### Requisitos  
RF052

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona
“Cadastrar clínica”.
3.O sistema abre a página “Cadastrar clínica”, com título na
aba e na página.
4.O ator visualiza a lista de clínicas cadastradas.
5.O ator pode adicionar uma nova clínica informando nome,
endereço e dados de contato.
6.O sistema salva as informações e atualiza a lista de
clínicas. [MSG01]
7.O ator confirma que a nova clínica foi cadastrada com
sucesso.

---

### Fluxo Alternativo 

A1 - Consulta sem alterações
- O ator acessa a página, mas não realiza alterações.
- O sistema mantém a lista inalterada.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.