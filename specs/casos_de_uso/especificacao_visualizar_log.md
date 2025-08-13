## Casos de uso UC45 - Visualizar log

---

### Objetivo  
Permitir que o administrador possa visualizar registros de log do sistema.

### Requisitos  
RF056

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona
“Visualizar log”.
3.O sistema abre a página correspondente com título na
aba e na página.
4.O ator visualiza a lista de registros, contendo data, hora,
ação executada e usuário responsável.
5.O ator pode filtrar registros por período, tipo de ação ou
usuário.


---

### Fluxo Alternativo 

A1 - Filtros não aplicados
- O ator visualiza todos os registros sem aplicar
filtros


### Fluxos de Exceção

MSG02 - Nenhum resultado encontrado
- O sistema exibe mensagem caso não haja registros
no período selecionado.