## Casos de uso UC40 - Configurar regras de cobrança e repasse

---

### Objetivo  
Permitir que o administrador possa definir as regras de
cobrança e repasse financeiro por profissional.

### Requisitos  
RF050

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona
“Configurar regras de cobrança e repasse”.
3.O sistema abre a página com título correspondente na
aba e na página.
4.O ator visualiza as regras vigentes.
5.O ator ajusta, adiciona ou remove regras de cobrança e
repasse.
6.O sistema salva as alterações e atualiza os cálculos
financeiros. [MSG01]
7.O ator confirma que as regras foram aplicadas
corretamente.

---

### Fluxo Alternativo 

A1 - Acesso sem alterações
- O ator acessa a página mas não realiza mudanças.
- O sistema mantém as regras vigentes.

### Fluxos de Exceção

MSG02 - Erro na operação
O sistema exibe uma mensagem de erro caso a operação não possa ser concluída.