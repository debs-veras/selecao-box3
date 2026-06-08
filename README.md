# Seleção Box3 - CRUD de Contatos

Projeto desenvolvido como teste técnico para entrada na empresa Box3.

Esta versão foi feita com HTML, CSS e JavaScript puro, consumindo a API de contatos disponibilizada no desafio. Também existe uma outra versão em React, criada como evolução deste mesmo projeto.

## Sobre o desafio

O objetivo do teste era criar um CRUD de contatos com as seguintes funcionalidades:

- Listar contatos cadastrados
- Cadastrar um novo contato
- Editar dados de um contato existente
- Remover um contato
- Validar campos do formulário
- Consumir a API da Box3

O enunciado original está no arquivo `teste-estagiario.pdf`.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Fetch API
- API REST da Box3

## Estrutura do projeto

```text
.
|-- assets/
|   |-- css/
|   |-- img/
|   `-- js/
|-- controller/
|-- service/
|-- view/
|-- index.html
`-- teste-estagiario.pdf
```

## Principais arquivos

- `index.html`: tela inicial com a listagem de contatos.
- `service/contato-service.js`: centraliza as chamadas para a API da Box3.
- `controller/listaContatos-controller.js`: controla a renderização da lista e a exclusão de contatos.
- `controller/cadastraContato-controller.js`: controla o cadastro de novos contatos.
- `controller/atualizaContato-controller.js`: controla a edição de contatos existentes.
- `assets/js/validacao.js`: contém validações de formulário e máscara de telefone.

## Como executar

Este projeto não possui etapa de build nem instalação de dependências. Para executar, basta servir os arquivos com um servidor estático.

Opções comuns:

```bash
# Com a extensão Live Server do VS Code
# Abra o projeto e inicie o Live Server no arquivo index.html
```

ou:

```bash
# Com Node.js instalado
npx serve .
```

Depois, acesse a URL exibida pelo servidor no navegador.

## API

A aplicação consome a API da Box3 para realizar as operações de CRUD. As chamadas estão concentradas em `service/contato-service.js`.

Operações usadas no projeto:

- `GET`: listar contatos
- `POST`: cadastrar contato
- `GET`: buscar contato por ID
- `PUT`: atualizar contato
- `DELETE`: remover contato

## Versão em React

Este repositório representa a versão feita com HTML, CSS e JavaScript puro para o teste da Box3. Posteriormente, também foi criada uma versão em React, separada desta implementação, com a mesma proposta de CRUD de contatos.
