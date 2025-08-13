## Caso de uso UC29 - Visualizar Relatório de Procedimento


---
**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar relatórios que mostrem quais procedimentos são mais comuns.

**Requisitos**  
RF040

**Atores**  
Terapeuta
--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Procedimento”.
3. O sistema redireciona o ator para a página de procedimento. Ele verifica que o título da aba do navegador e da própria página é “Procedimento”
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● mês
● período
● ano
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● nome do terapeuta
● data do procedimento
● nome do procedimento
● quantidade de vezes realizado
8. O ator verifica as informações apresentadas e identifica o(s) procedimento(s) mais comum(s) com base nos dados exibidos.
---
### Fluxo Alternativo

A1 - Buscar todas as informações dos procedimentos sem
aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema retorna os relatórios de procedimentos de
todos os períodos disponíveis, organizados por ordem
cronológica decrescente.


---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.