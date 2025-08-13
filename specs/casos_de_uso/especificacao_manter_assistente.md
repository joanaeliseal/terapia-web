## Casos de uso UC36 - Manter assistente

---

### Objetivo  
Permitir que o administrador possa gerenciar o cadastro de
assistentes administrativos, incluindo criação, edição e
exclusão.


### Requisitos  
RF046

### Atores  
Administrador

---

### Fluxo principal  

1. O ator acessa a página inicial (home) do sistema. No
menu principal, clica em “Administração”.
2. O sistema exibe um submenu. O ator clica na opção
“Manter assistente”.
3. O sistema redireciona o ator para a página “Manter
assistente”, com título exibido na aba do navegador e na
própria página.
4. O ator visualiza a lista de assistentes cadastrados.
5. O ator pode adicionar, editar ou excluir registros de
assistentes.
6. O sistema processa a ação e atualiza a lista. [MSG01]
7. O ator verifica que a atualização foi feita corretamente.

---

### Fluxo Alternativo 

A1 - Consultar sem alterar dados
- O ator acessa a página, mas não realiza alterações.
- O sistema mantém os dados inalterados.


### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.