## Caso de uso UC24 - Forma de Pagamento

---
**Objetivo**  
Permitir que o terapeuta e o assistente possam oferecer
diferentes formas de pagamento para as consultas como:
dinheiro, PIX, cartão crédito/débito, e boleto.


**Requisitos**  
RF031

**Atores**  
Terapeuta/Assistente

--- 

### Fluxo Principal

1. O ator acessa a página de pagamento. Ele verifica que o
título da página da aba do navegador e na própria página é
“Pagamento”. Ele observa que existe um campo para:
● nome do paciente
● cpf do paciente
● data da compra
● email do paciente
● valor da compra
● forma de pagamento(dinheiro, pix, cartão de crédito,
cartão de débito e boleto)
● opções:
❖ confirmar
❖ cancelar
2. O ator preenche os campos com os dados do paciente e da
compra e seleciona o botão para confirmar o pagamento, [A1]
3. O sistema verifica se as informações para o pagamento são
válidas. [RN1]
4. O sistema exibe uma página de confirmação do pagamento
e mostra uma mensagem que o pagamento foi realizado com
sucesso.

---
### Fluxo Alternativo

A1 - Cancelar Pagamento
1. O ator decide cancelar o pagamento. Ele clica no botão
cancelar.
2. O sistema pergunta se o usuário deseja cancelar o
pagamento.
3. O ator confirma o cancelamento.
4. O sistema cancela a compra.
---
### Fluxo de Exceção

RN1- Validação dos campos
Todas as informações são obrigatórias.