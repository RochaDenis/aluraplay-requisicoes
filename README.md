**Documentação Resumida - Aplicação Web de Vídeos com JavaScript**

### Visão Geral:

Esta aplicação web permite aos usuários visualizar, criar e buscar vídeos por meio de uma interface simples. Ela utiliza JavaScript para interagir com uma API de vídeos, realizando operações como listar vídeos, criar novos vídeos e buscar vídeos com base em termos específicos.

### Estrutura do Projeto:

O projeto é dividido em módulos, cada um com uma responsabilidade específica:

1. **conectaApi.js:**
   - Contém funções assíncronas para interagir com a API de vídeos.
   - `listaVideos`: Obtém a lista de vídeos da API.
   - `criaVideo`: Cria um novo vídeo na API.
   - `buscaVideo`: Realiza uma busca na API com base em um termo.

2. **mostrarVideos.js:**
   - Exporta a função `constroiCard` que constrói cards de vídeo com base nos dados fornecidos.
   - Estes cards são utilizados para exibir os vídeos na interface da aplicação.

3. **scriptPrincipal.js:**
   - Utiliza as funções do módulo `conectaApi` para interagir com a API.
   - Gerencia eventos do DOM para criar vídeos, exibir listas e lidar com erros.

### Funcionalidades Principais:

1. **Listagem de Vídeos:**
   - A função `listaVideo` é responsável por obter a lista de vídeos da API e exibi-los na página.

2. **Criação de Vídeos:**
   - A função `criarVideo` é acionada quando o usuário envia o formulário de criação.
   - Os dados do formulário são coletados, e a função `criaVideo` da API é utilizada para adicionar um novo vídeo.
   - Em caso de sucesso, o usuário é redirecionado para uma página de confirmação.

3. **Busca de Vídeos:**
   - A função `buscarVideo` é acionada quando o usuário envia o formulário de busca.
   - O termo de busca é enviado para a API, e os resultados são exibidos na página.

### Estrutura dos Elementos na Página:

- **Formulário de Criação:**
  - Campos para título, descrição, URL e imagem do vídeo.
  - O botão de envio aciona a função `criarVideo`.

- **Lista de Vídeos:**
  - Elemento `<ul>` com a classe "videos__lista".
  - Cada vídeo é representado por um elemento `<li>` com a classe "videos__item".
  - Utiliza a função `constroiCard` para criar cards de vídeo.

- **Card de Vídeo:**
  - Contém um elemento `<iframe>` para exibir o vídeo.
  - Inclui um bloco com a imagem do canal, título e descrição do vídeo.

### Tratamento de Erros:

- Erros durante a interação com a API são capturados e tratados.
- Em caso de erro ao listar vídeos, uma mensagem é exibida na lista.
- Em caso de erro ao criar um vídeo, um alerta é exibido ao usuário.

### Conclusão:

Esta aplicação web proporciona uma experiência de usuário interativa, permitindo a criação, listagem e busca de vídeos por meio de uma integração eficiente com uma API dedicada. A estrutura modular e a manipulação de eventos em JavaScript garantem uma experiência fluida e responsiva para os usuários.



<p align="center"> <img src="https://imgur.com/J3hD21O.png" alt="Javascript: criando requisições"> </p>

<hr>

<p align="center"> <img src="https://github.com/MonicaHillman/aluraplay-requisicoes/blob/main/img/logo.png" alt="Logo da Alura"> </p>
<p align="center">Página inicial e formulário de cadastro de vídeos da AluraPlay, uma plataforma de compartilhamento de vídeos.</p>

## Tecnologias utilizadas durante o curso
* Javascript
* NodeJS
* Json-server

## Tecnologias utilizadas no projeto
* HTML
* CSS

## Screenshots
![Screenshot da tela inicial do AluraPlay](https://imgur.com/aymxEsh.png)
![Screenshot da tela do formulário do AluraPlay](https://imgur.com/ShNADf2.png)

