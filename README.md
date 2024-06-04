ServeRest - Usuários

 Descrição

Este repositório contém uma coleção de testes para a API de Usuários do ServeRest, utilizando o Postman. A coleção inclui testes para operações CRUD (Create, Read, Update, Delete) nos endpoints de usuários, garantindo que a API funcione conforme o esperado.

Estrutura da Coleção

A coleção é composta pelos seguintes endpoints e testes:

1. GET /usuarios
   - Verifica se a resposta tem status 200.
   - Confirma que a resposta contém um array de usuários e que a quantidade de usuários é maior que zero.

2. GET /usuarios/{id} - válido
   - Verifica se a resposta tem status 200.
   - Confirma que a resposta contém os dados do usuário especificado pelo ID.

3. GET /usuarios/{id} - inválido
   - Verifica se a resposta tem status 400.
   - Confirma que a resposta contém a mensagem de erro "Usuário não encontrado" para um ID inválido.

4. POST /usuarios - válido
   - Verifica se a resposta tem status 201.
   - Confirma que a resposta contém a mensagem "Cadastro realizado com sucesso".

5. POST /usuarios - inválido (email repetido)
   - Verifica se a resposta tem status 400.
   - Confirma que a resposta contém a mensagem de erro "Este email já está sendo usado".

6. PUT /usuarios/{id}
   - Verifica se a resposta tem status 200.
   - Confirma que a resposta contém a mensagem "Registro alterado com sucesso" após a atualização dos dados do usuário.

7. DELETE /usuarios/{id}
   - Verifica se a resposta tem status 200.
   - Confirma que a resposta contém a mensagem "Registro excluído com sucesso" após a exclusão do usuário.

Como Usar

Pré-requisitos

- [Postman](https://www.postman.com/downloads/)
- API ServeRest rodando localmente em `http://localhost:3000`

Importando a Coleção

1. Abra o Postman.
2. Clique em `Import` no canto superior esquerdo.
3. Selecione `File` e importe o arquivo `ServeRest - Usuários.postman_collection.json` do repositório.

Executando os Testes

1. Certifique-se de que a API ServeRest está rodando em `http://localhost:3000`.
2. No Postman, vá até a aba `Collections` e selecione `ServeRest - Usuários`.
3. Clique em `Run` para executar todos os testes da coleção.

Contribuindo

1. Faça um fork deste repositório.
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`).
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`).
4. Push para a branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

Licença

Este projeto está licenciado sob os termos da licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

Contato

Para mais informações, entre em contato com [Ivaneide Nascimento](mailto:ivaneideqa@ebac.com.br).
