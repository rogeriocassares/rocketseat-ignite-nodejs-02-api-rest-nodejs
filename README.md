tsx only for develpo.

tsc to js for production


o comando time da o tempo de execucao!





Migrations sao controle de versao dentro do banco de dados.

O git eh muito mais para conseguirmos trabalhar na base de codigo com varias pessoas do que criar controles de versao



Supondo que duas pessoas podem alterar o banco de dados de funcionalidades diferentes. Quando duas pessoas forem colocar em produ~cao, elas precisariam enviar o sql para enviar os dados do banco atualizados.



O migraions sao um historico de todas as mudanças feitas no db e essas mudancas sao sempre anotados com data e horario com a data que foram criadas



O mais importante eh que tem com ela uma tabela acriada automaticamente chaada migrations.

Essa tabela mostra o historico de tabelas.

Se existir uma migrations que o db ainda nao conhece, basta atualizar o codigo.



As pessoas pdem adicionar e remover campos e temos a afacilidade de ter o db atualizado entre todos os desenvolvedores.

❯   npm run knex -- migrate:make create-transactions

❯   npm run knex -- migrate:rollback

❯ npm run knex -- migrate:latest



❯ npm run knex -- migrate:make add-session-id-to-transactions

// Make changes in the add-session-id-to-transactions migration

❯ npm run knex -- migrate:latest