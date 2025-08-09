Obs: Mensagem - MSG01 = “Nenhum resultado encontrado” 

---
## Casos de uso  
**UC24 - Forma de Pagamento**

---
**Objetivo**  
Permitir que o terapeuta e o assistente possam oferecer diferentes formas de pagamento para as consultas como: dinheiro, PIX, cartão crédito/débito, e boleto.

**Requisitos**  
RF031

**Atores**  
Terapeuta / Assistente
---

### Fluxo Principal

1. O ator acessa a página de pagamento. Ele verifica que o título da página da aba do navegador e na própria página é “Pagamento”. Ele observa que existe um campo para:  
   - nome do paciente  
   - cpf do paciente  
   - data da compra  
   - email do paciente  
   - valor da compra  
   - forma de pagamento (dinheiro, pix, cartão de crédito, cartão de débito e boleto)  
   - opções:  
     - confirmar  
     - cancelar  
2. O ator preenche os campos com os dados do paciente e da compra e seleciona o botão para confirmar o pagamento, [A1]  
3. O sistema verifica se as informações para o pagamento são válidas. [RN1]  
4. O sistema exibe uma página de confirmação do pagamento e mostra uma mensagem que o pagamento foi realizado com sucesso.

### Fluxo Alternativo

**A1 - Cancelar Pagamento**  
1. O ator decide cancelar o pagamento. Ele clica no botão cancelar.  
2. O sistema pergunta se o usuário deseja cancelar o pagamento.  
3. O ator confirma o cancelamento.  
4. O sistema cancela a compra.

### Fluxo de Exceção

**RN1 - Validação dos campos**  
Todas as informações são obrigatórias.

---

**UC25 - Receber Notificação de Pagamento**
---
**Objetivo**  
Permitir que o terapeuta e o paciente recebam uma mensagem de confirmação do pagamento da sessão.

**Requisitos**  
RF032

**Atores**  
Terapeuta / Paciente
---
### Fluxo Principal

1. O ator recebe uma mensagem por e-mail informando da compra realizada.

---

**UC26 - Acessar Informação de Inadimplência**
---

**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar informações de inadimplência dos pacientes, a fim de identificar pagamentos pendentes das sessões.

**Requisitos**  
RF034

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Paciente”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Inadimplência”.  
3. O sistema redireciona o ator para a página de inadimplência. Ele verifica que o título da aba do navegador e da própria página é “Inadimplência”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - nome do paciente  
   - CPF do paciente  
   - período (data inicial e final)  
   - status (inadimplente ou quitado)  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com os seguintes dados para cada paciente inadimplente:  
   - nome do paciente  
   - CPF  
   - data da cobrança  
   - valor pendente  
   - quantidade de dias de atraso  
   - status do pagamento  
8. O ator verifica quais pacientes estão na lista exibida.

### Fluxo Alternativo

**A1 - Buscar todos os inadimplentes sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna todos os pacientes inadimplentes cadastrados.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC27 - Acessar Relatório de Rentabilidade**
---

**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar relatórios que mostrem qual mês ou período foi o mais rentável.

**Requisitos**  
RF035

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Rentabilidade”.  
3. O sistema redireciona o ator para a página de rentabilidade. Ele verifica que o título da aba do navegador e da própria página é “Rentabilidade”  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - mês  
   - período  
   - ano  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - nome do terapeuta  
   - data  
   - receita total  
   - custos e despesas  
   - despesas gerais  
   - resultado final  
8. O ator verifica as informações apresentadas e identifica o(s) período(s) mais rentável(eis) com base nos dados exibidos.

### Fluxo Alternativo

**A1 - Buscar todas as informações de rentabilidade sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios de rentabilidade de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC28 - Acessar Relatório de Procedimento**
---

**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar relatórios que mostrem quais procedimentos são mais comuns.

**Requisitos**  
RF040

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Procedimento”.  
3. O sistema redireciona o ator para a página de procedimento. Ele verifica que o título da aba do navegador e da própria página é “Procedimento”  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - mês  
   - período  
   - ano  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - nome do terapeuta  
   - data do procedimento  
   - nome do procedimento  
   - quantidade de vezes realizado  
8. O ator verifica as informações apresentadas e identifica o(s) procedimento(s) mais comum(s) com base nos dados exibidos.

### Fluxo Alternativo

**A1 - Buscar todas as informações dos procedimentos sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios de procedimentos de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---
**UC29 - Acessar Relatório de Fluxo de Caixa**
---

**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar o fluxo de caixa da clínica/consultório, acompanhando entradas, saídas e saldo final de determinado período.

**Requisitos**  
RF041

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Fluxo de Caixa”.  
3. O sistema redireciona o ator para a página de fluxo de caixa. Ele verifica que o título da aba do navegador e da própria página é “Fluxo de Caixa”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - mês  
   - tipo (entrada, saída ou ambos)  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data da movimentação  
   - tipo (entrada/saída)  
   - descrição  
   - valor  
   - total de entradas  
   - total de saídas  
   - saldo total  
8. O ator verifica os valores e analisa a saúde financeira com base no saldo exibido.

### Fluxo Alternativo

**A1 - Buscar todas as informações do fluxo de caixa sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios do fluxo de caixa de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC30 - Filtrar Relatórios**
---

**Objetivo**  
Permitir que o terapeuta possa filtrar os relatórios financeiros por convênio e/ou paciente(s) em determinado período.

**Requisitos**  
RF042

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Relatório”.  
3. O sistema redireciona o ator para a página de relatório. Ele verifica que o título da aba do navegador e da própria página é “Relatório”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - data  
   - período  
   - convênio  
   - paciente  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data/ período  
   - convênio  
   - paciente  
   - quantidade por convênio  
   - valor total no período  
8. O ator verifica os dados e identifica as informações financeiras referente aos convênios e pacientes no período selecionado.

### Fluxo Alternativo

**A1 - Buscar todas as informações dos relatórios dos convênios sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios da forma de pagamento de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC31 - Acessar Relatório de Forma de Pagamento**
---

**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar a(s) forma(s) de pagamento(s) dos pacientes em determinado período.

**Requisitos**  
RF033

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Forma de Pagamento”.  
3. O sistema redireciona o ator para a página de forma de pagamento. Ele verifica que o título da aba do navegador e da própria página é “Forma de Pagamento”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - data  
   - período  
   - tipo (dinheiro, pix, cartão crédito/débito, boleto, todas as formas)  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data do pagamento  
   - tipo (dinheiro, pix, cartão crédito/débito, boleto)  
   - quantidade de cada tipo  
   - total por forma de pagamento  
   - valor total no período  
8. O ator verifica os dados e identifica quais formas de pagamento foram mais utilizadas no período selecionado.

### Fluxo Alternativo

**A1 - Buscar todas as informações da forma de pagamento sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios da forma de pagamento de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC32 - Filtrar Relatório de Convênio**
---

**Objetivo**  
Permitir que o terapeuta possa filtrar os relatórios financeiros de convênios e/ou pacientes em determinado período. Esses relatórios devem oferecer comparativos entre atendimentos particulares e por convênio, bem como demonstrar o desempenho mensal e a distribuição do atendimento.

**Requisitos**  
RF037, RF038, RF039, RF042

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Relatório”.  
3. O sistema redireciona o ator para a página de relatório. Ele verifica que o título da aba do navegador e da própria página é “Relatório”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - data  
   - período  
   - convênio  
   - paciente  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data/ período  
   - convênio  
   - total por convênio  
   - valor total no período  
8. O ator verifica os dados e identifica quais convênios foram mais utilizados no período selecionado.

### Fluxo Alternativo

**A1 - Buscar todas as informações do relatório de convênio sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema retorna os relatórios de convênio de todos os períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC33 - Visualizar Gráficos**
---

**Objetivo**  
Permitir que o terapeuta possa visualizar gráficos financeiros que representem a evolução das receitas, lucros e prejuízos ao longo dos meses, possibilitando uma análise visual da rentabilidade por período e por convênio.

**Requisitos**  
RF043

**Atores**  
Terapeuta
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Gráfico”.  
3. O sistema redireciona o ator para a página de gráfico. Ele verifica que o título da aba do navegador e da própria página é “Gráfico”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - data  
   - período  
   - rentabilidade  
   - convênio  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data ou período  
   - convênio  
   - valor do prejuízo  
   - lucro total  
8. O ator analisa visualmente os gráficos e verifica as informações correspondentes ao período selecionado, identificando tendências e resultados financeiros.

### Fluxo Alternativo

**A1 - Visualizar gráfico sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema exibe gráficos e dados dos períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção

**MSG01 - Nenhum resultado encontrado**  
O sistema exibe a mensagem MSG01.

---

**UC34 - Acessar Relatórios dos Clientes**
---

**Objetivo**  
Permitir que o administrador do sistema tenha acesso a relatórios com o total de clientes (terapeutas) e empresas cadastrados, incluindo mensalidades.

**Requisitos**  
RF045

**Atores**  
Administrador
---

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu principal, ele clica no item “Financeiro”.  
2. O sistema exibe um submenu com várias opções. O ator clica na opção “Cliente”.  
3. O sistema redireciona o ator para a página de clientes. Ele verifica que o título da aba do navegador e da própria página é “Cliente”.  
4. O ator observa que existe um campo de pesquisa com as opções para filtrar por:  
   - data  
   - período  
   - cliente  
   - clínica  
5. O ator preenche os filtros desejados e clica no botão "Buscar". [A1]  
6. O sistema busca os registros com base nos filtros informados. [MSG01]  
7. O sistema exibe uma tabela com as seguintes informações:  
   - data ou período  
   - total de clientes  
   - total de clínicas  
   - valor da mensalidade  
   - total da mensalidade dos clientes  
   - total da mensalidade das clínicas  
8. O ator verifica os dados e identifica o quantitativo de clientes e clínicas no período selecionado.

### Fluxo Alternativo

**A1 - Buscar todas as informações do relatório de cliente sem aplicar filtros**  
- O ator não preenche nenhum filtro e clica em "Buscar".  
- O sistema exibe todos os relatórios dos clientes dos períodos disponíveis, organizados por ordem cronológica decrescente.

### Fluxo de Exceção
MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.

## Caso de uso UC35 - Emitir Nota Fiscal

---
**Objetivo**  
Permitir a emissão de nota fiscal.

**Requisitos**  
RF044

**Atores**  
SEFAZ
--- 

### Fluxo Principal

1. O ator realiza a emissão da nota fiscal.
