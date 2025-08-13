## Caso de uso UC30 - Acompanhar Fluxo de Caixa

---
**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar o fluxo de
caixa da clínica/consultório, acompanhando entradas, saídas e
saldo final de determinado período.


**Requisitos**  
RF041

**Atores**  
Terapeuta

--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Financeiro”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Fluxo de Caixa”.
3. O sistema redireciona o ator para a página de fluxo de caixa.
Ele verifica que o título da aba do navegador e da própria
página é “Fluxo de Caixa”
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● mês
● tipo (entrada, saída ou ambos)
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com as seguintes informações:
● data da movimentação
● tipo (entrada/saída)
● descrição
● valor
● total de entradas
● total de saídas
● saldo total
8.O ator verifica os valores e analisa a saúde financeira com
base no saldo exibido.

---
### Fluxo Alternativo

A1 - Buscar todas as informações do fluxo de caixa sem aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema retorna os relatórios do fluxo de caixa todos
os períodos disponíveis, organizados por ordem
cronológica decrescente.
---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.