## Caso de uso UC31 - Visualizar Relatório de Forma de Pagamento


---
**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar a(s)
forma(s) de pagamento(s) dos pacientes em determinado
período.


**Requisitos**  
RF033

**Atores**  
Terapeuta
--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Forma de Pagamento”.
3. O sistema redireciona o ator para a página de forma de
pagamento. Ele verifica que o título da aba do navegador e da
própria página é “Forma de Pagamento”
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● data
● período
● tipo (dinheiro, pix, cartão crédito/débito, boleto,
todas as formas )
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● data do pagamento
● tipo (dinheiro, pix, cartão crédito/débito, boleto )
● quantidade de cada tipo
● total por forma de pagamento
● valor total no período
8.O ator verifica os dados e identifica quais formas de
pagamento foram mais utilizadas no período selecionado. 
---
### Fluxo Alternativo

A1 - Buscar todas as informações da forma de pagamento sem
aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema retorna os relatórios da forma de pagamento
de todos os períodos disponíveis, organizados por
ordem cronológica decrescente.


---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.