## Casos de uso UC18 - Receber notificação

---

### Objetivo  
Permitir que o terapeuta e o paciente recebam notificações sobre mudanças, confirmações ou cancelamentos de sessões.

### Requisitos  
RF024, RF030

### Atores  
Terapeuta / Assistente / Paciente

---

### Fluxo principal  

1. Um evento relevante ocorre no sistema (ex.: sessão agendada, cancelada, reagendada).
2. O sistema identifica o público-alvo da notificação (terapeuta, paciente, assistente). 
3. O sistema envia a notificação pelo(s) canal(is) configurados (app, e-mail, SMS).
4. O ator visualiza a notificação com as informações essenciais:
- data e hora da sessão
- tipo (confirmação, cancelamento, lembrete)
- informações adicionais, se houver
