# Kanban Board Interativo – Estilo Trello

Este é um projeto de Kanban Board Interativo que simula funcionalidades semelhantes às do Trello. A aplicação permite que você gerencie tarefas de forma visual e dinâmica, com suporte a operações de criação, edição, exclusão, arraste e soltura (drag & drop) entre as colunas "A Fazer", "Fazendo" e "Feito". Além disso, o estado do board é persistido no LocalStorage, garantindo que suas tarefas sejam mantidas mesmo após o recarregamento da página.

## Funcionalidades

- **Adicionar Tarefas:**  
  Cada coluna possui um formulário para adicionar novas tarefas.  
  - *A Fazer*: Tarefas a serem iniciadas.  
  - *Fazendo*: Tarefas em andamento.  
  - *Feito*: Tarefas concluídas.

- **Edição e Exclusão:**  
  As tarefas podem ser editadas via modal, permitindo atualizar seu conteúdo, e também podem ser excluídas individualmente com confirmação.

- **Marcar como Feito / Desfazer:**  
  Nas colunas "A Fazer" e "Fazendo", é possível marcar tarefas como concluídas (movendo-as para a coluna "Feito"). Já na coluna "Feito", há a opção de desfazer essa ação e retornar a tarefa para "A Fazer".

- **Drag & Drop:**  
  As tarefas (cards) são arrastáveis entre os contêineres das colunas graças à biblioteca SortableJS, permitindo reorganizar e mover tarefas conforme necessário.

- **Persistência Local:**  
  Toda a estrutura de dados é salva no LocalStorage, garantindo que o estado do board seja mantido entre sessões.

- **Visual Moderno e Responsivo:**  
  O projeto utiliza Bootstrap, Google Fonts (Poppins) e Font Awesome para criar uma interface bonita, limpa e adaptada a diferentes dispositivos.

- **Opção de Limpar o Quadro:**  
  Um botão no cabeçalho permite limpar todo o board, removendo todas as tarefas (com confirmação).

## Tecnologias Utilizadas

- **HTML5** – Estrutura da aplicação.
- **CSS3 & Google Fonts (Poppins)** – Estilização e tipografia moderna.
- **JavaScript (Vanilla)** – Lógica de funcionamento, manipulação do DOM e persistência com LocalStorage.
- **Bootstrap 5** – Layout responsivo, componentes e modais para edição.
- **Font Awesome** – Ícones para melhorar a interface.
- **SortableJS** – Funcionalidade de drag & drop para mover os cards entre as colunas.

## Como Executar

1. **Clone o Repositório ou Baixe os Arquivos:**

   ```bash
   git clone https://github.com/murilomm8/kanban-board-interativo.git
   cd kanban-board-interativo
Abra o Arquivo index.html:

Basta abrir o arquivo index.html em seu navegador favorito e você terá acesso à interface do Kanban Board. Como a aplicação é front-end puro e utiliza LocalStorage, nenhum server-side é necessário para testes.

Uso
Adição de Tarefas: Em cada coluna, utilize o campo de entrada para digitar uma nova tarefa e clique no botão "Adicionar". A tarefa será inserida no contêiner de cards correspondente.

Edição: Clique no ícone de lápis (botão de editar) para abrir o modal de edição da tarefa. Atualize o conteúdo e clique em "Salvar Alterações".

Exclusão: Clique no ícone de lixeira para remover uma tarefa. Um diálogo de confirmação aparecerá para evitar exclusões acidentais.

Marcar como Feito / Desfazer: Se a tarefa estiver em "A Fazer" ou "Fazendo", clique no botão com o ícone de check para movê-la para "Feito". Se estiver na coluna "Feito", clique no ícone de undo para voltar à coluna "A Fazer".

Reorganização via Drag & Drop: Você pode arrastar qualquer tarefa (card) entre os contêineres "A Fazer", "Fazendo" ou "Feito". A ordem e a posição serão salvas automaticamente no LocalStorage.

Limpar o Quadro: Utilize o botão "Limpar Quadro" no cabeçalho para remover todas as tarefas (apenas após confirmação).

Possíveis Melhorias Futuras
Filtragem e Priorização: Adicionar recursos para filtrar tarefas por data, prioridade ou etiquetas.

Colaboração Online: Implementar um backend com autenticação e compartilhamento em tempo real para múltiplos usuários.

Exportação/Importação: Permitir a exportação e importação do board para backup ou compartilhamento.

Conclusão
Este projeto demonstra habilidades em desenvolvimento web, manipulação do DOM, uso de bibliotecas modernas e persistência local. Ele é uma excelente base para evoluir para aplicações mais complexas e para mostrar seu portfólio de projetos interativos e bem estruturados.