## Casos de uso UC15 - Manter Sessão

---

### Objetivo  
Permitir que o terapeuta e o assistente efetuam as ações de agendar, editar, cancelar e confirmar a sessão, além de registrar a evolução do paciente.

### Requisitos  
RF017, RF018, RF019, RF020

### Atores  
Terapeuta/Assistente

### Condição de entrada  
O ator está logado no sistema.

---

### Fluxo principal  

1. O ator seleciona ‘Agendar Sessão’.
2. O sistema exibe a página de agendamento, com título ‘Agendar Sessão’ na aba do navegador e no topo da página.
3. O ator verifica que a página contém os campos:
- paciente (em formato de lista)
- data da sessão
- horário de início
- duração
- tipo de sessão (presencial, domiciliar, teleatendimento)
- observações
- campo opcional de motivo (em caso de reagendamento)
- opções: salvar e cancelar

4. O ator preenche os campos obrigatórios e seleciona Salvar.
5. O sistema valida os campos conforme [RN1 - Validação de campos obrigatórios].
6. O sistema salva a sessão e exibe mensagem de sucesso.


---

### Fluxos Alternativos  

A1 – Agendar sessão
1. O ator seleciona a opção ‘Agendar Sessão’.
2. O sistema solicita dados como paciente, data, horário e duração, respeitando os horários de trabalho configurados. [RF017]
3. O ator confirma o agendamento.
4. O sistema salva e exibe mensagem de sucesso.

A2 – Editar sessão agendada
1. O ator seleciona uma sessão não realizada.
2. O sistema exibe os dados atuais da sessão.
3. O ator altera os campos desejados (data, horário, duração, observações). [RF018]
4. O sistema salva as alterações e retorna à lista.

A3 – Cancelar sessão
1. O ator seleciona uma sessão agendada.
2. O sistema pergunta se deseja cancelar.
3. O ator confirma, opcionalmente informando um motivo. [RF020]
4. O sistema registra o status da sessão como ‘cancelada’ e mantém no histórico.

A4 – Confirmar realização de sessão
1. O ator seleciona uma sessão em andamento ou recém-encerrada.
2. O ator confirma manualmente a realização. [RF024]
3. O sistema atualiza o status e registra no prontuário.

A5 – Registrar evolução da sessão
1. O ator seleciona uma sessão já realizada.
2. O sistema permite inserir ou anexar documento de evolução. [RF019]
3. O sistema salva as informações.

### Fluxos de exceção

RN1 - Validação de campos
MSG01: Nenhum resultado encontrado. 
(Caso o ator tente acessar uma sessão que foi excluída ou não existe, o sistema exibe a mensagem MSG01.)
