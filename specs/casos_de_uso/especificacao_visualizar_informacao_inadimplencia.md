## Caso de uso UC26 - Visualizar Informação de Inadimplência

---
**Objetivo**  
Permitir que o terapeuta possa acessar e visualizar
informações de inadimplência dos pacientes, a fim de identificar pagamentos pendentes das sessões.


**Requisitos**  
RF034

**Atores**  
Terapeuta

--- 

### Fluxo Principal

1. O ator acessa a página inicial (home) do sistema. No menu
principal, ele clica no item “Paciente”.
2. O sistema exibe um submenu com várias opções. O ator
clica na opção “Inadimplência”.
3. O sistema redireciona o ator para a página de inadimplência. Ele verifica que o título da aba do navegador e da própria página é “Inadimplência”.
4. O ator observa que existe um campo de pesquisa com as
opções para filtrar por:
● nome do paciente
● CPF do paciente
● período (data inicial e final)
● status (inadimplente ou quitado)
5. O ator preenche os filtros desejados e clica no botão
"Buscar". [A1]
6. O sistema busca os registros com base nos filtros
informados. [MSG01]
7. O sistema exibe uma tabela com os seguintes dados para
cada paciente inadimplente:
● nome do paciente
● CPF
● data da cobrança
● valor pendente
● quantidade de dias de atraso
● status do pagamento
8. O ator verifica quais pacientes estão na lista exibida.
---
### Fluxo Alternativo

A1 - Buscar todos os inadimplentes sem aplicar filtros
● O ator não preenche nenhum filtro e clica em "Buscar".
● O sistema retorna todos os pacientes inadimplentes
cadastrados.


---
### Fluxo de Exceção

MSG01 - Nenhum resultado encontrado
O sistema exibe a mensagem MSG01.