# SSI Solid Server

<img src="https://raw.githubusercontent.com/CommunitySolidServer/CommunitySolidServer/main/templates/images/solid.svg"
 alt="[Solid logo]" height="150" align="right"/>

[![MIT license](https://img.shields.io/npm/l/@solid/community-server)](https://github.com/CommunitySolidServer/CommunitySolidServer/blob/main/LICENSE.md)
[![npm version](https://img.shields.io/npm/v/@solid/community-server)](https://www.npmjs.com/package/@solid/community-server)
[![Node.js version](https://img.shields.io/node/v/@solid/community-server)](https://www.npmjs.com/package/@solid/community-server)
[![Build Status](https://github.com/CommunitySolidServer/CommunitySolidServer/workflows/CI/badge.svg)](https://github.com/CommunitySolidServer/CommunitySolidServer/actions)
[![Coverage Status](https://coveralls.io/repos/github/CommunitySolidServer/CommunitySolidServer/badge.svg)](https://coveralls.io/github/CommunitySolidServer/CommunitySolidServer)
[![DOI](https://zenodo.org/badge/265197208.svg)](https://zenodo.org/badge/latestdoi/265197208)
[![GitHub discussions](https://img.shields.io/github/discussions/CommunitySolidServer/CommunitySolidServer)](https://github.com/CommunitySolidServer/CommunitySolidServer/discussions)
[![Chat on Gitter](https://badges.gitter.im/CommunitySolidServer/community.svg)](https://gitter.im/CommunitySolidServer/community)

- **SSI significa Identidade Auto Soberana -> [*Self Sovereign Identity*](https://www.manning.com/books/self-sovereign-identity) -> SSI**
- **SSI Solid Server, SSS, é baseado no [Community Solid Server, CSS,](https://github.com/CommunitySolidServer/CommunitySolidServer)**
- **Este é um projeto da Universidade de Brasília, UnB, para ajudar a alcançar a SSI por meio do protocolo [Solid](https://solidproject.org/)**
- **Todo o *software* é código aberto e pensado na sua segurança, privacidade e autonomia! 🙏​**

O SSS provê hospedagem de Pods Solid e Identidade Web (WebID). Esses Pods atuam como seu próprio espaço de armazenamento pessoal para que você possa compartilhar dados com pessoas e aplicativos Solid. O projeto foi pensado para:

- 👨🏿‍💻 **Desenvolvedores** dispostos a utilizarem e melhorarem o *software*.
- 👨🏽‍🎓​ **Estudantes** principalmente no contexto da UnB, com o projeto [SmartUnB.ECOS](https://sol.sbc.org.br/index.php/weihc/article/view/22854).
- 👩🏻‍🔬 **Pesquisadores** que gostariam de desenvolver novas funcionalidades.
- 🧑🏽 **Qualquer pessoa** interessada em ter autonomia dos seus próprios dados.

O projeto ainda está em fase de desenvolvimento e adaptação, contribuições são bem-vindas para melhorar a experiência do usuário, tanto do experiente quanto do usuário normal da Web.

## ⚡ Executando o SSI Solid Server

Certifique-se de possuir o [Node.js](https://nodejs.org/en/), versão 18.0 ou maior, instalado na sua máquina. Clone o repositório, acesse a pasta e instale as dependências.

```shell
npm i
```

Inicie o servidor.

```shell
npx .
```

Agora visite o seu servidor local, através de um navegador, em [http://localhost:3000/](http://localhost:3000/).

Para persistir o conteúdo do seu pod entre reinicializações, use:

```shell
npx . @solid/community-server -c @css:config/file.json -f data/
```

Caso prefira usar o Docker, você pode encontrar instruções para este e outros métodos na [documentação](https://communitysolidserver.github.io/CommunitySolidServer/latest/usage/starting-server/).

## 🔧 Configurando o servidor

Mudanças substanciais no comportamento do servidor podem ser alcançadas por meio de arquivos de configuração JSON, utilizando o [Components.js](https://componentsjs.readthedocs.io/en/latest/), para especificar como módulos e componentes precisam ser interligados em tempo de execução. o SSS também adiciona funcionalidades por meio desse módulos, permitindo que todas as opções de configurações possam ser habilitadas e selecionadas.

Receitas para configurar o servidor podem ser encontradas em [CommunitySolidServer/recipes](https://github.com/CommunitySolidServer/recipes).

Exemplos e orientações sobre configurações personalizadas estão disponíveis na pasta `config` e no [tutorial de configurações](https://github.com/CommunitySolidServer/tutorials/blob/main/custom-configurations.md). Há também um [gerador de configurações](https://communitysolidserver.github.io/configuration-generator/).

## 👩🏽‍💻 Desenvolvendo código de servidor

O servidor permite escrever e conectar módulos personalizados sem alterar seu código-fonte base.

A [📗 documentação da API](https://communitysolidserver.github.io/CommunitySolidServer/5.x/docs) e a [📓 documentação do usuário](https://communitysolidserver.github.io/CommunitySolidServer/) estão disponpiveis para consulta. Há também um repositório de [📚 tutoriais abrangentes](https://github.com/CommunitySolidServer/tutorials/)

## 📜 Licença

O código do Community Solid Server é protegido por direitos autorais da [Inrupt Inc.](https://inrupt.com/) e da [imec](https://www.imec-int.com/) e está disponível sob a [Licença MIT](https://github.com/CommunitySolidServer/CommunitySolidServer/blob/main/LICENSE.md).
