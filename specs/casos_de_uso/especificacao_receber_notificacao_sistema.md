## Casos de uso UC48 - Receber notificação do sistema

---

### Objetivo  
Permitir que o administrador visualize notificações
administrativas geradas pelo sistema.

### Requisitos  
RF055

### Atores  
Administrador

---

### Fluxo principal  

1.O sistema envia automaticamente notificações relevantes.
2.O administrador acessa a área de notificações no
sistema.
3.O administrador visualiza as mensagens e pode marcálas como lidas.

---

### Fluxo Alternativo 

A1 - Nenhuma notificação disponível
- O sistema exibe mensagem informando que não
há novas notificações.

### Fluxos de Exceção

MSG02 - Falha no carregamento
O sistema exibe mensagem de erro caso não seja
possível carregar as notificações.