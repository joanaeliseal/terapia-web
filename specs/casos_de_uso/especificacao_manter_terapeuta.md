## Casos de uso UC35 - Manter terapeuta

---

### Objetivo  
Permitir que o administrador possa gerenciar o cadastro de
terapeutas, incluindo criação, edição e exclusão de registros

### Requisitos  
RF046

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial (home) do sistema. No
menu principal, clica no item “Administração”.
2.O sistema exibe um submenu com várias opções. O ator
clica na opção “Manter terapeuta”.
3.O sistema redireciona o ator para a página “Manter
terapeuta”, com título exibido na aba do navegador e na
própria página.
4.O ator visualiza a lista de terapeutas cadastrados.
5.O ator pode escolher entre: adicionar um novo terapeuta,
editar um terapeuta existente ou excluir um cadastro.
6.O sistema processa a solicitação e atualiza a lista de
terapeutas. [MSG01]
7.O ator confirma que as informações estão corretas e
finaliza a operação.


---

### Fluxo Alternativo 

A1 - Consultar sem alterar dados
- O ator acessa a página, mas não realiza alterações.
- O sistema mantém os dados inalterados.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.