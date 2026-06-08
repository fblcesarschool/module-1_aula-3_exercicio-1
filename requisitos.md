# Documento de Requisitos do Projeto: API de Séries e Filmes

A tabela abaixo apresenta os requisitos funcionais detalhados para uma **API de gerenciamento de listas de séries e filmes**.

| ID do Requisito | Descrição | História do Usuário | Comportamento/Resultado Esperado |
|----------------|-----------|----------------------|-----------------------------------|
| RF01 | Criar uma nova lista | Como consumidor da API, quero criar uma nova lista vazia para começar a adicionar séries ou filmes. | A API deve disponibilizar um endpoint para criação de uma nova lista vazia. |
| RF02 | Adicionar séries/filmes à lista | Como consumidor da API, quero adicionar séries ou filmes informando seus nomes ou IDs para organizar minha lista. | A API deve permitir inserir itens (séries/filmes) em uma lista existente. |
| RF03 | Consultar itens da lista | Como consumidor da API, quero listar todas as séries ou filmes de uma lista para visualizar seu conteúdo. | A API deve retornar todos os itens associados a uma lista. |
| RF04 | Atualizar item da lista | Como consumidor da API, quero editar informações de uma série ou filme na lista caso haja erro ou atualização. | A API deve permitir a atualização de um item existente na lista. |
| RF05 | Remover item da lista | Como consumidor da API, quero remover uma série ou filme da lista quando não desejar mais mantê-lo. | A API deve permitir a exclusão de itens individuais da lista. |
| RF06 | Publicar lista | Como consumidor da API, quero publicar uma lista para torná-la acessível publicamente. | A API deve alterar o status da lista para pública e gerar um link de acesso compartilhável. |
| RF07 | Compartilhar lista | Como consumidor da API, quero obter um link de compartilhamento da lista para uso externo. | A API deve retornar uma URL pública da lista com possibilidade de acesso externo. |
| RF08 | Acessar lista pública | Como usuário externo, quero acessar uma lista publicada para visualizar seus conteúdos. | A API deve permitir a leitura de listas públicas via endpoint sem necessidade de autenticação. |
| RF09 | Listar todas as listas do usuário | Como consumidor da API, quero recuperar todas as listas que criei para gerenciamento. | A API deve retornar todas as listas associadas a um usuário autenticado. |
| RF10 | Excluir lista | Como consumidor da API, quero excluir uma lista inteira quando não precisar mais dela. | A API deve remover a lista e todos os seus itens associados permanentemente. |
| RF11 | Listar todos os filmes | Como consumidor da API, quero visualizar o catálogo completo de filmes disponíveis no sistema. | A API deve retornar uma listagem completa de todos os filmes cadastrados com paginação. |
| RF12 | Listar filmes disponíveis para aluguel | Como consumidor da API, quero visualizar apenas os filmes que estão disponíveis para aluguel. | A API deve retornar filmes com status de disponibilidade ativa. |
| RF13 | Listar filmes indisponíveis | Como consumidor da API, quero visualizar os filmes que estão indisponíveis para aluguel. | A API deve retornar filmes com status de indisponibilidade. |
| RF14 | Consultar detalhes de um filme | Como consumidor da API, quero obter informações completas de um filme específico. | A API deve retornar dados detalhados do filme (título, sinopse, gênero, ano, duração, etc). |
| RF15 | Buscar filmes por nome | Como consumidor da API, quero buscar filmes pelo título para encontrar conteúdos específicos. | A API deve retornar filmes que correspondam ao critério de busca por nome. |
| RF16 | Buscar filmes por gênero | Como consumidor da API, quero filtrar filmes por categoria/gênero. | A API deve retornar todos os filmes que pertencem ao gênero solicitado. |
| RF17 | Buscar filmes por ano de lançamento | Como consumidor da API, quero filtrar filmes por ano de lançamento. | A API deve retornar filmes lançados no ano especificado. |
| RF18 | Listar filmes mais alugados | Como consumidor da API, quero visualizar os filmes com maior quantidade de aluguéis. | A API deve retornar filmes ordenados por número de aluguéis (ranking). |
| RF19 | Listar lançamentos | Como consumidor da API, quero visualizar os filmes lançados recentemente. | A API deve retornar filmes ordenados por data de lançamento (mais recentes primeiro). |
| RF20 | Alugar um filme | Como consumidor da API, quero alugar um filme disponível. | A API deve criar um registro de aluguel associando o filme ao usuário e definir data de devolução. |
| RF21 | Devolver um filme alugado | Como consumidor da API, quero registrar a devolução de um filme alugado. | A API deve atualizar o status do aluguel para concluído e marcar o filme como disponível novamente. |
| RF22 | Renovar aluguel | Como consumidor da API, quero estender o período de um aluguel ativo. | A API deve permitir a renovação de aluguéis, estendendo a data de devolução. |
| RF23 | Consultar histórico de aluguéis do cliente | Como consumidor da API, quero visualizar todos os aluguéis que realizei (ativos e concluídos). | A API deve retornar o histórico completo de aluguéis do usuário autenticado. |
| RF24 | Consultar aluguéis ativos do cliente | Como consumidor da API, quero visualizar apenas os aluguéis vigentes que ainda não foram devolvidos. | A API deve retornar apenas aluguéis com status ativo do usuário. |
| RF25 | Adicionar filme à lista de favoritos | Como consumidor da API, quero marcar filmes como favoritos para acesso rápido posterior. | A API deve permitir adicionar/remover filmes da lista de favoritos do usuário. |
| RF26 | Receber notificação quando um filme voltar ao estoque | Como consumidor da API, quero ser notificado quando um filme indisponível voltar a estar disponível. | A API deve registrar a preferência de notificação e enviar alerta quando o filme ficar disponível. |
