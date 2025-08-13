## Caso de uso UC32 - Visualizar Gráficos

---
**Objetivo**  
Permitir que o terapeuta possa visualizar gráficos financeiros
que representem a evolução das receitas, lucros e prejuízos ao
longo dos meses, possibilitando uma análise visual da
rentabilidade por período e por convênio.


**Requisitos**  
RF043

**Atores**  
Terapeuta

--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Gráfico”.
3. O sistema redireciona o ator para a página de gráfico. Ele
verifica que o título da aba do navegador e da própria página é “Gráfico”.
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● data
● período
● rentabilidade
● convênio
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● data ou período
● convênio
● valor do prejuízo
● lucro total
8. O ator analisa visualmente os gráficos e verifica as
informações correspondentes ao período selecionado,
identificando tendências e resultados financeiros.

---

### Fluxo Alternativo

A1 - Visualizar gráfico sem aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema exibe gráficos e dados dos períodos
disponíveis, organizados por ordem cronológica
decrescente.

---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.