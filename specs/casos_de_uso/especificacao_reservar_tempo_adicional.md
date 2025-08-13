## Casos de uso UC17 - Reservar tempo adicional

---

### Objetivo  
Permitir que o terapeuta reserve tempo extra antes ou depois de sessões domiciliares para deslocamento, bloqueando esse período na agenda.

### Requisitos  
RF021

### Atores  
Terapeuta 

---

### Fluxo principal  

1. O ator seleciona uma sessão domiciliar na agenda.
2. O ator visualiza as opções de ‘Tempo adicional’ antes e/ou depois da sessão.
3. O ator informa a quantidade de tempo extra desejada (em minutos).
4. O sistema ajusta o agendamento para incluir o tempo adicional como bloqueio na agenda.
5. O ator confirma a alteração.
6. O sistema salva o agendamento com o bloqueio registrado.

---

### Fluxos Alternativos 

A1 – Remover tempo adicional: O ator edita uma sessão e zera os campos de tempo extra, removendo o bloqueio.

A2 – Definir tempo padrão: O ator configura um tempo adicional padrão nas preferências do sistema; este valor é aplicado automaticamente em novas sessões domiciliares.

### Fluxos de Exceção

Conflito de horário: Se o tempo adicional conflitar com outra sessão ou bloqueio existente, o sistema alerta e não permite salvar.