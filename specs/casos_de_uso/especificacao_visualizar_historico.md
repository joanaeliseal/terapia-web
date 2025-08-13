## Casos de uso UC06 - Visualizar histórico

---

### Objetivo  
Exibir painel com o histórico clínico do paciente, incluindo anamnese, PII, sessões realizadas e documentos anexados.

### Requisitos  
RF009, RF016

### Atores  
Terapeuta ocupacional, Assistente administrativo (quando autorizado)

### Condição de entrada  
O ator acessa o prontuário do paciente e seleciona **Histórico**.

---

### Fluxo principal  

1. O ator acessa a página de histórico clínico.  
2. O sistema exibe resumos das seções do prontuário.  
3. O ator pode navegar entre abas ou aplicar filtros de período.  
4. O sistema atualiza as informações exibidas.  
5. O ator encerra a visualização.

---

### Fluxos de exceção  

**RNF002** - Respeitar permissões de acesso.  
**RNF001** - Criptografia dos dados.  
**RNF016** - Registro em log.