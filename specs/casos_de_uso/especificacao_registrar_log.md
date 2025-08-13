## Casos de uso UC44 - Registrar log

---

### Objetivo  
Permitir que o administrador possa registrar atividades do
sistema para auditoria.

### Requisitos  
RF056

### Atores  
Administrador

---

### Fluxo principal  

1.O sistema registra automaticamente todas as ações
relevantes no log.
2.O administrador acessa a função “Registrar log” apenas
para verificar se o recurso está ativo e configurado.
3.O sistema confirma que o registro automático está
funcionando.

---

### Fluxo Alternativo 

A1 - Falha no registro automático
- O sistema detecta falha no log e alerta o
administrador.

### Fluxos de Exceção

MSG02 - Erro no registro
O sistema exibe mensagem de erro caso não seja
possível registrar as ações.