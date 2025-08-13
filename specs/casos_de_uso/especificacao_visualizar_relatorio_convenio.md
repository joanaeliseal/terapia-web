## Caso de uso UC28 - Visualizar Relatório de Convênio

---
**Objetivo**  
Permitir que o terapeuta possa filtrar os relatórios financeiros de convênios e/ou pacientes em determinado período. Esses relatórios devem oferecer comparativos entre atendimentos particulares e por convênio, bem como demonstrar o desempenho mensal e a distribuição do atendimento.


**Requisitos**  
RF037, RF038, RF039, RF042

**Atores**  
Terapeuta

--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Relatório”.
3. O sistema redireciona o ator para a página de relatório. Ele
verifica que o título da aba do navegador e da própria página é
“Relatório”
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● data
● período
● convênio
● paciente
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● data/ período
● convênio
● total por convênio
● valor total no período
8.O ator verifica os dados e identifica quais convênios foram
mais utilizados no período selecionado.
---
### Fluxo Alternativo

A1 - Buscar todas as informações do relatório de convênio sem
aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema retorna os relatórios de convênio todos os
períodos disponíveis, organizados por ordem cronológica decrescente.


---
### Fluxo de Exceção

EMSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.