## Casos de uso UC37 - Configurar horários de atendimento

---

### Objetivo  
Permitir que o administrador possa definir e ajustar os horários padrão de atendimento dos profissionais.

### Requisitos  
RF047

### Atores  
Administrador

---

### Fluxo principal  

1. O ator acessa a página inicial (home) do sistema e clica
em “Administração”.
2. O sistema exibe um submenu. O ator seleciona
“Configurar horários de atendimento”.
3. O sistema exibe a página “Configurar horários de
atendimento”, com título visível na aba do navegador e na
própria página.
4. O ator visualiza a grade de horários existente.
5. O ator ajusta, adiciona ou remove horários disponíveis.
6. O sistema salva as alterações e atualiza a agenda
padrão. [MSG01]
7. O ator confirma que as configurações foram aplicadas
corretamente.

---

### Fluxo Alternativo 

A1 - Acesso sem alterações
- O ator acessa a página mas não modifica os
horários.
- O sistema mantém as configurações atuais.

### Fluxos de Exceção

MSG02 - Erro ao salvar alterações
O sistema exibe mensagem de erro caso não seja possível concluir a operação.