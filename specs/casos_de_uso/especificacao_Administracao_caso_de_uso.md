**UC35 - Manter terapeuta**

---

### Objetivo  
Permitir que o administrador possa gerenciar o cadastro de terapeutas, incluindo criação, edição e exclusão de registros.

### Requisitos  
RF046

### Atores  
Administrador

### Condição de entrada  
O ator acessa o menu **Administração** e seleciona **Manter terapeuta**.

---

### Fluxo principal  

1. O ator acessa a página inicial (home) do sistema.  
2. No menu principal, clica no item **Administração**.  
3. O sistema exibe um submenu com várias opções.  
4. O ator clica na opção **Manter terapeuta**.  
5. O sistema redireciona para a página **Manter terapeuta**, com título exibido na aba do navegador e na própria página.  
6. O ator visualiza a lista de terapeutas cadastrados.  
7. O ator pode escolher entre: adicionar um novo terapeuta, editar um terapeuta existente ou excluir um cadastro.  
8. O sistema processa a solicitação e atualiza a lista de terapeutas. [MSG01]  
9. O ator confirma que as informações estão corretas e finaliza a operação.

---

### Fluxos alternativos  

**A1 - Consultar sem alterar dados**  
O ator acessa a página, mas não realiza alterações.  
O sistema mantém os dados inalterados.

---

### Fluxos de exceção  

**MSG02 - Erro na operação**  
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.

---

**UC36 - Manter assistente**

---

### Objetivo  
Permitir que o administrador possa gerenciar o cadastro de assistentes administrativos, incluindo criação, edição e exclusão.

### Requisitos  
RF046

### Atores  
Administrador

### Condição de entrada  
O ator acessa o menu **Administração** e seleciona **Manter assistente**.

---

### Fluxo principal  

1. O ator acessa a página inicial (home) do sistema.  
2. No menu principal, clica em **Administração**.  
3. O sistema exibe um submenu.  
4. O ator clica na opção **Manter assistente**.  
5. O sistema redireciona para a página **Manter assistente**, com título exibido na aba do navegador e na própria página.  
6. O ator visualiza a lista de assistentes cadastrados.  
7. O ator pode adicionar, editar ou excluir registros de assistentes.  
8. O sistema processa a ação e atualiza a lista. [MSG01]  
9. O ator verifica que a atualização foi feita corretamente.

---

### Fluxos alternativos  

**A1 - Consultar sem alterar dados**  
O ator acessa a página, mas não realiza alterações.  
O sistema mantém os dados inalterados.

---

### Fluxos de exceção  

**MSG02 - Erro na operação**  
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.

---

**UC37 - Configurar horários de atendimento**

---

### Objetivo  
Permitir que o administrador possa definir e ajustar os horários padrão de atendimento dos profissionais.

### Requisitos  
RF047

### Atores  
Administrador

### Condição de entrada  
O ator acessa o menu **Administração** e seleciona **Configurar horários de atendimento**.

---

### Fluxo principal  

1. O ator acessa a página inicial (home) do sistema.  
2. No menu principal, clica em **Administração**.  
3. O sistema exibe um submenu.  
4. O ator seleciona **Configurar horários de atendimento**.  
5. O sistema exibe a página **Configurar horários de atendimento**, com título visível na aba do navegador e na própria página.  
6. O ator visualiza a grade de horários existente.  
7. O ator ajusta, adiciona ou remove horários disponíveis.  
8. O sistema salva as alterações e atualiza a agenda padrão. [MSG01]  
9. O ator confirma que as configurações foram aplicadas corretamente.

---

### Fluxos alternativos  

**A1 - Acesso sem alterações**  
O ator acessa a página, mas não modifica os horários.  
O sistema mantém as configurações atuais.

---

### Fluxos de exceção  

**MSG02 - Erro ao salvar alterações**  
O sistema exibe mensagem de erro caso não seja possível concluir a operação.

---

