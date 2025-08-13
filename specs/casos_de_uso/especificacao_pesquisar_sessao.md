## Casos de uso UC16 - Pesquisar Sessão

---

### Objetivo  
Permitir que o terapeuta ou assistente encontre sessões agendadas ou passadas filtrando por nome do paciente, data, status, tipo ou palavra-chave.

### Requisitos  
RF022, RF023

### Atores  
Terapeuta/Assistente

### Condição de entrada  
O ator acessa a página de agenda/lista de sessões.

---

### Fluxo principal  

1. O ator visualiza o campo de busca e os filtros disponíveis:
- nome do paciente
- data ou intervalo de datas
- status da sessão (realizada, agendada, cancelada)
- tipo (presencial, domiciliar, teleatendimento)
- palavras-chave

2. O ator informa os critérios de pesquisa.
3. O ator aciona a opção ‘Pesquisar’.
4. O sistema filtra as sessões de acordo com os critérios e exibe os resultados em formato de lista ou calendário.
5. O ator localiza a sessão desejada.

---

### Fluxos Alternativos  

A1 – Limpar filtros: O ator seleciona a opção "Limpar filtros" para restaurar a lista completa de sessões.


A2 – Acesso rápido: O ator utiliza a barra de busca no topo da página para digitar parte do nome do paciente; o sistema atualiza a lista em tempo real.

### Fluxos de exceção

MSG01: Nenhum resultado encontrado. 
(Caso não existam sessões, o sistema exibe  a mensagem MSG01.)

