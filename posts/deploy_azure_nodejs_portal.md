## Introdução

O Azure serviço de cloud da Microsoft, disponibiliza um catálogo enorme de produtos para computação em nuvem, o Azure App Service Web Apps é um destes, que tem como premissa facilitar o processo de build e deploy de uma aplicação web, podendo essa ser uma aplicação web tradicional ou uma web api, nas mais variadas teconologias como .NET Core, ASP.NET, Java, Node.js, PHP, Python ou Ruby.

Neste artigo vamos aprender como realizar o deploy de uma aplicação Node.js da forma mais prática através do Portal do Azure.

## Requisitos

Para prosseguir é necessário que você já tenha criado uma conta no Azure, um processo simples que necessita apenas que você tenha uma e-mail da Microsoft (hotmail ou outlook) e um cartão internacional, a solicitação do cartão no momento do cadastro é somente para fins de segurança, podendo gerar um custo que será estornado no momento seguinte.

## Acessando o Portal

Depois de termos acesso a conta do Azure, logo após a realização do cadastro ou do login, nós teremos acesso ao Portal do Azure, que a princípio pode ser assutador, mas logo depois de entendermos como as coisas são organizadas tudo vai ficando mais claro.

Essa á a tela inicial que pode estar um pouco diferente da sua, pois o Portal do Azure é personalizavel, podendo realizar algumas pequenas modificação na sua aparência, como a paleta de cores por exemplo.

![Home](../images/001_deploy_azure_nodejs_portal.png)

## Criando um Resource Group

O primeiro passo para a configuração de um Azure App Service Web App é a criação de um Resource Group, para isso nós vamos fazer uma busca pelo termo "Resource groups" na barra de pesquisa e selecionar a opção "Resource groups".

![Home](../images/002_deploy_azure_nodejs_portal.png)

Depois de selecionarmos a opção veremos uma listagem contendo todos os Resource Groups já criados em nossa conta, para criarmos um novo nós podemos selecionar a opção "Add" para irmos para o formulário de criação. Esses passos são semelhantes para a maioria dos serviços no Azure, normalmente fazemos uma busca, vemos uma listagem e selecionamos a opção para adicionar um novo.

![Home](../images/003_deploy_azure_nodejs_portal.png)

Nesta etapa nós devemos informar nossas preferências a respeito do Resource group a ser criado, selecionando uma Subscription (normalmente é criado uma no momento de cadastro no Azure mas nós podemos adicionar outras posteriormente), informando um nome e selecionando uma região. Depois disso podemos selecionar a opção "Review + create", e por fim a opção "Create". No exemplo selecionei a minha Subscription padrão, nomeei o Resource Group como "tempflaviogfresourcegroup" e selecionei a região como East US.

![Home](../images/004_deploy_azure_nodejs_portal.png)

![Home](../images/005_deploy_azure_nodejs_portal.png)

## Criando um App Service Plan

Avançando vamos criar um outro recurso necessário, que é a criação de um App Service Plan como dito anteriormente é muito semelhante. Para isso nós vamos fazer uma busca pelo termo "App Service Plans" na barra de pesquisa e selecionar a opção "App Service plans" 

![Home](../images/006_deploy_azure_nodejs_portal.png)

Depois de selecionarmos a opção veremos uma listagem agora contendo todos os App Service Plans já criados em nossa conta, para criarmos um novo nós podemos selecionar a opção "Add" para irmos para o formulário de criação.

![Home](../images/007_deploy_azure_nodejs_portal.png)

Agora iremos informar as opções a respeito do nosso App Service Plan a ser criado, selecionando uma Subscription, um Resource Group, informando um nome, selecionando um sistema opercional, uma região e uma camada de preço. Logo após isso podemos selecionar a opção "Review + create", e por fim a opção "Create". No exemplo selecionei minha Subscription padrão, o Resource Group criado na etapa anterior, nomeei o serviço como "tempflaviogfappserviceplan", selecionei o Windows como sistema operacional, a região como East US, e por fim a camada Free F1 disponível somente no Windows.

![Home](../images/008_deploy_azure_nodejs_portal.png)

![Home](../images/009_deploy_azure_nodejs_portal.png)

![Home](../images/010_deploy_azure_nodejs_portal.png)

![Home](../images/011_deploy_azure_nodejs_portal.png)

## Criando um App Service Web App

Por fim criaremos o último recurso necessário e também o tema principal deste artigo, o App Service Web App, para enfim podermos hospedar nossa aplicação, novamente faremos uma busca pelo recurso agora digitando na barra de pesquisa o termo "App services" e selecionando a opção encontrada.

![Home](../images/012_deploy_azure_nodejs_portal.png)

Veremos novamente uma listagem com nossos recursos já contratados e a opção "Add" que é o nosso interesse principal então selecionaremos ela. 

![Home](../images/013_deploy_azure_nodejs_portal.png)

Agora para prosseguirmos selecionaremos uma Subscription, um Resource Group, informaremos um nome, escolheremos um tipo de publicação, selecionaremos um Runtime, escolheremos um sistema operacional, selecionaremos uma região e um App Service Plan. Enfim podemos selecionar a opção "Review + create", e depois a opção "Create". No exemplo selecionei minha Subscription padrão, o Resource Group criado na primeiro etapa, nomeei o App Service Web App como "tempflaviogfwebapp", escolhi o tipo de publicação Code, selecione o runtime Node 12 LTS, escolhi o sistema operacional Windows, selecionei a região East US e o App Service plan criado na etapa anterior, que esta disponível para seleção por possuir o mesmo sistema operacional deste que estamos criando.

![Home](../images/014_deploy_azure_nodejs_portal.png)

![Home](../images/015_deploy_azure_nodejs_portal.png)

![Home](../images/016_deploy_azure_nodejs_portal.png)

## Configurando o Git

## Realizando o deploy

## Descartando todos os recursos (Opcional)
