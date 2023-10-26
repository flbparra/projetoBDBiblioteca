# projeto de um Banco de Dados (Biblioteca)
Repositório voltado a crostução de um banco para uma biblioteca fictícia, fiquem avontade para darem suas dicas precisiosas para um iniciante!

Preciso saber o que acha dos diagramas de entidade relacionamento e modelo lógico que fiz, claro é para um trabalho de BD que tenho, porém, sinto que é algo que preciso melhorar então postarei aqui as partes do projeto depois que já entregar, para que os conselhos e dicas eu implemente no decorrer do projeto. Para torna melhor essa analise aqui em baixo vai ter as especificações do projeto.

# Especificações do Projeto

## Estrutura do Banco de Dados
O banco de dados do sistema deve ser projetado com as seguintes tabelas/entidades:
1. __Livros__:
- Título
- Autor
- ISBN (Chave primária)
- Descrição
- Categoria
- Data de Aquisição
- Estado de Conservação
- Localização Física
- URI da capa do livro
2. Materiais Didáticos:
- ID (Chave Primária)
- Descrição
- Categoria
- Número de Série
- Data de Aquisição
- Estado de Conservação
- Localização Física
- URI da foto do material
3. Usuários:
- ID (e.g., Chave Primária)
- Nome
- Sobrenome
- Função (e.g., Administrador, Membro)
- Login
- Senha (criptografada)
- URI da foto do usuário
4. Empréstimos:
- ID do Usuário (Chave Estrangeira)
- ID do Item (Chave Estrangeira)
- Data de Empréstimo
- Data de Devolução Prevista
- Status (Em andamento, Concluído)

## Requisitos funcionais:
O sistema deve ser capaz de realizar as seguintes funções:

1. __Cadastro de Livros e Materiais__:
- Os administradores e chefes de laboratório devem ser capazes de cadastrar
novos livros e materiais no sistema, fornecendo informações detalhadas sobre
cada um.
2. __Catalogação__:
- O sistema deve permitir a catalogação de informações detalhadas sobre cada
item, incluindo título, autor, ISBN (para livros), descrição, categoria, número de
série (para materiais), data de aquisição e estado de conservação.
3. __Armazenamento Físico__:
- O sistema deve registrar a localização física de cada livro e material, ou seja, em qual estante ou prateleira eles estão armazenados.
4. __Empréstimo e Devolução__:
- Os usuários devem poder solicitar empréstimos de livros e materiais através do
sistema computacional.
- O sistema deve controlar os prazos de empréstimo e permitir renovações (se
aplicável).
- Registrar a devolução e atualizar a disponibilidade.
5. __Pesquisa e Consulta__: 
- Os usuários devem ser capazes de pesquisar e consultar o catálogo de livros e
materiais por título, autor, categoria, etc.
- Exibir informações detalhadas sobre os itens disponíveis.
6. __Controle de Acesso__:
 - O sistema deve implementar controles de acesso para garantir que apenas usuários autorizados (administradores e chefes do laboratório) possam cadastrar, modificar e excluir registros.

## Considerações de Segurança
- Senhas de usuário devem ser armazenadas de forma segura e criptografadas (o
grupo pode implementar um algoritmo para cifrar a senha antes de salvá-la ou usar
um recurso disponível pelo SGBD escolhido).
- Apenas administradores têm permissão para realizar ações de cadastramento e
modificação dos usuários.
- Um sistema de controle de acesso baseado em funções deve ser implementado
para garantir que apenas usuários autorizados acessem recursos específicos.
- Chefes de laboratório podem gerenciar (inserir, remover, atualizar informações,
mudar o status do empréstimo, etc) os recursos (livros e materiais)

---

# Atualizações e comentários:
> No momento estou na parte de implmentação do SQL, logo mais atualizo vocês, peço apenas para dar uma olhada na pasta de _Diagrama do Banco_ onde vai conter os diagrama lógico e o DER, e falarem com suas esperiências o que posso melhorar. (__comentário: 26/10/2023 - Parra__).

Obrigado!