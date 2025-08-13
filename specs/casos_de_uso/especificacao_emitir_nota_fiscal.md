## Caso de uso UC34 - Emitir Nota Fiscal

---
**Objetivo**  
Permitir a emissão de nota fiscal.

**Requisitos**  
RF044

**Atores**  
SEFAZ
--- 

### Fluxo Principal

1. O sistema recebe solicitação de acesso ao serviço de emissão
de nota fiscal. [E1], [MSG01].
2. O sistema valida os dados obrigatórios para emissão [A1], [E2],
[MSG02]:
● identificação do prestador
● CPF/CNPJ do tomador
● descrição do serviço
● valor
● data
3. O ator recebe os dados fiscais enviados pelo serviço de
integração. [E3], [MSG03]
4. O ator processa e valida as informações recebidas. [E4],
[MSG04]
5. O ator retorna a resposta ao serviço de integração (autorização,
rejeição, protocolo ou pendência).
6. O ator grava a resposta no histórico de emissão e atualiza o
status da nota fiscal.
7. Se autorizado, o sistema disponibiliza o documento eletrônico
(PDF/XML) para download/impressão.
8. O fluxo é encerrado.
---
### Fluxo Alternativo

A1 – Emissão a partir de atendimento já cadastrado
● O sistema preenche automaticamente os dados da nota
fiscal a partir do atendimento selecionado.
● O fluxo segue a partir do passo 3 do Fluxo Principal.

---
### Fluxo de Exceção

E1 – Solicitação de acesso inválida ou não autorizada
● O sistema exibe a mensagem MSG01 ( Solicitação inválida
ou não autorizada) e encerra o processo sem tentar
emissão.
E2 – Dados inválidos
● O sistema exibe a mensagem MSG02 (Dados inválidos) e
destaca os campos que precisam ser corrigidos.
E3 – Falha na transmissão para o SEFAZ
● O sistema exibe a mensagem MSG03 (Falha de
comunicação com o SEFAZ) e registra a tentativa para
reenvio automático.
E4 – Rejeição pelo SEFAZ
● O sistema exibe a mensagem MSG04 (Rejeição de
emissão) com a justificativa retornada.