## Casos de uso UC41 - Configurar mensagens e notificações

---

### Objetivo  
Permitir que o administrador possa configurar mensagens
automáticas e notificações enviadas aos pacientes.

### Requisitos  
RF053

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona
“Configurar mensagens e notificações”.
3.O sistema abre a página correspondente, exibindo o título
na aba e na página.
4.O ator visualiza as mensagens e notificações já
configuradas.
5.O ator pode criar novas mensagens, editar existentes ou
excluir configurações.
6.O sistema salva as alterações e atualiza as notificações
automáticas. [MSG01]
7.O ator confirma que as alterações foram aplicadas
corretamente.

---

### Fluxo Alternativo 

A1 - Consulta sem alterações
- O ator acessa a página mas não realiza mudanças.
- O sistema mantém as configurações vigentes.


### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.