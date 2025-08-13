## Caso de uso UC33 - Visualizar Relatórios dos Clientes

---
**Objetivo**  
Permitir que o administrador do sistema ter acesso a relatórios
com o total de clientes (terapeutas) e empresas cadastrados,
incluindo mensalidades.
.

**Requisitos**  
RF045

**Atores**  
Administrador
--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Cliente”.
3. O sistema redireciona o ator para a página de clientes. Ele
verifica que o título da aba do navegador e da própria página é “Cliente”
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● data
● período
● cliente
● clínica
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● data ou período
● total de clientes
● total de clínicas
● valor da mensalidade
● total da mensalidade dos clientes
● total da mensalidade das clínicas
8. O ator verifica os dados e identifica o quantitativo de clientes e clínicas no período selecionado.

---
### Fluxo Alternativo

A1 - Buscar todas as informações do relatório de cliente sem
aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema exibe todos os relatórios dos clientes dos
períodos disponíveis, organizados por ordem
cronológica decrescente.

---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.