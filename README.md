# library-api
Caso de Uso: Sistema de Empréstimo de Livros em uma Biblioteca
1. Introdução
   Este caso de uso descreve as funcionalidades básicas de um sistema simples de empréstimo de livros em uma biblioteca. O sistema visa automatizar o processo de empréstimo, devolução e gerenciamento de livros e usuários.

2. Atores
   Bibliotecário: Responsável por cadastrar livros, usuários, realizar empréstimos e devoluções, e gerar relatórios.
   Usuário: Pessoa que deseja realizar empréstimos e devoluções de livros.
3. Pré-condições
   O sistema está instalado e configurado corretamente.
   O bibliotecário possui acesso ao sistema.
   O usuário está cadastrado no sistema.
4. Pós-condições
   As informações sobre livros, usuários, empréstimos e devoluções são armazenadas no sistema.
   O status dos livros e usuários é atualizado após cada operação.
   Relatórios podem ser gerados a qualquer momento.
5. Fluxo Principal
   Cadastrar Livro:
   O bibliotecário informa o título, autor, ISBN, quantidade disponível e outras informações relevantes sobre o livro.
   O sistema armazena as informações do livro no banco de dados.
   Cadastrar Usuário:
   O bibliotecário informa o nome, endereço, telefone e outras informações relevantes sobre o usuário.
   O sistema armazena as informações do usuário no banco de dados.
   Realizar Empréstimo:
   O biblioteário informa o código do livro e o código do usuário.
   O sistema verifica a disponibilidade do livro e se o usuário possui algum empréstimo em atraso.
   Se o livro estiver disponível e o usuário estiver em dia, o sistema registra o empréstimo e atualiza a quantidade disponível do livro.
   Realizar Devolução:
   O biblioteário informa o código do livro e o código do usuário.
   O sistema verifica se o livro está cadastrado e se o empréstimo está ativo.
   Se o empréstimo estiver ativo, o sistema registra a devolução e atualiza a quantidade disponível do livro.
   Gerar Relatórios:
   O bibliotecário seleciona o tipo de relatório desejado (livros mais emprestados, usuários com mais atrasos, etc.).
   O sistema gera o relatório com base nos dados armazenados.
6. Fluxos Alternativos
   Livro Indisponível: Se o livro solicitado estiver emprestado, o sistema informa o usuário sobre a indisponibilidade.
   Usuário com Empréstimo em Atraso: Se o usuário possuir algum empréstimo em atraso, o sistema não permite realizar um novo empréstimo até que o atraso seja regularizado.
   Livro não Cadastrado: Se o livro informado não estiver cadastrado no sistema, o bibliotecário deve cadastrar o livro antes de realizar o empréstimo.
   Usuário não Cadastrado: Se o usuário informado não estiver cadastrado no sistema, o bibliotecário deve cadastrar o usuário antes de realizar o empréstimo.

7. Exceções
   Erro ao conectar ao banco de dados: O sistema informa o erro e interrompe a operação.
   Falha ao salvar dados: O sistema informa o erro e permite que o bibliotecário tente novamente.
   Observações:
