## Casos de uso UC49 - Definir nível de acesso

---

### Objetivo  
Permitir que o administrador possa configurar permissões e
níveis de acesso para usuários do sistema.

### Requisitos  
RF060

### Atores  
Administrador

---

### Fluxo principal  

1.O ator acessa a página inicial e clica em “Administração”.
2.O sistema exibe um submenu. O ator seleciona “Definir
nível de acesso”.
3.O sistema abre a página com a lista de usuários e suas
permissões.
4.O ator ajusta as permissões conforme necessário.
5.O sistema salva as alterações e aplica imediatamente.
[MSG01]

---

### Fluxo Alternativo 

A1 - Sem alterações
- O ator acessa a página mas não modifica
permissões.

### Fluxos de Exceção

MSG02 - Erro na operação
- O sistema exibe mensagem de erro caso a alteração
não possa ser concluída.