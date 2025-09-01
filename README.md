# Pokédex App com Ionic e Angular

_Um Web App responsivo construído como projeto de estudo e avaliação, com foco em boas práticas, consumo de APIs e criação de uma interface reativa inspirada nos jogos clássicos de Pokémon._

<br>

![Pokédex App Demo](URL_DO_SEU_GIF_OU_IMAGEM_AQUI)

<p align="center">
  <img src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" alt="Angular">
  <img src="https://img.shields.io/badge/Ionic-3880FF?style=for-the-badge&logo=ionic&logoColor=white" alt="Ionic">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/SCSS-CC6699?style=for-the-badge&logo=sass&logoColor=white" alt="SCSS">
</p>

## 📜 Sobre o Projeto

Esta é uma aplicação de Pokédex que consome dados da [PokéAPI](https://pokeapi.co/) para exibir uma lista completa de Pokémon. O objetivo foi criar uma experiência de usuário fluida e nostálgica, com um design temático inspirado na Pokédex do jogo **Pokémon FireRed**. A aplicação foi desenvolvida utilizando as práticas mais modernas do ecossistema Angular e Ionic, como componentes Standalone e reatividade com RxJS.

## ✨ Funcionalidades

O aplicativo possui uma gama completa de funcionalidades que demonstram a manipulação de dados síncronos e assíncronos:

-   **Lista de Pokémon:** Visualização da lista completa com **Scroll Infinito** para uma navegação fluida e performática.
-   **Busca em Tempo Real:** Barra de busca que filtra a lista de Pokémon localmente, oferecendo resultados instantâneos.
-   **Filtros Avançados:** Menus para filtrar a Pokédex por **Tipo** e por **Região**, consumindo endpoints específicos da API.
-   **Sistema de Favoritos:** Funcionalidade para marcar e desmarcar Pokémon como favoritos, com os dados salvos localmente no navegador (`localStorage`) para **persistência de dados**.
-   **Página de Detalhes:** Tela detalhada para cada Pokémon com informações completas:
    -   Status Base (HP, Ataque, etc.) com barras visuais.
    -   Descrição oficial da Pokédex (Flavor Text).
    -   Habilidades (incluindo habilidades ocultas).
    -   Linha Evolutiva clicável para navegar entre as evoluções.
-   **Design Temático e Responsivo:** Interface inspirada no Pokémon FireRed, que se adapta a diferentes tamanhos e orientações de tela (retrato e paisagem).
-   **Testes Unitários:** O projeto inclui testes unitários para o `FavoritesService` utilizando Jasmine e Karma, garantindo a qualidade e a robustez da lógica de negócios.

## 🛠️ Tecnologias Utilizadas

-   **Angular (v17+)**: Framework principal para a construção da aplicação.
-   **Ionic (v7+)**: Utilizado para a criação da interface de usuário com componentes mobile-first.
-   **TypeScript**: Linguagem principal, garantindo um código mais seguro e escalável.
-   **SCSS**: Para estilização avançada e organização do CSS.
-   **RxJS**: Para o gerenciamento de operações assíncronas, como na lógica de *debounce* da busca que foi implementada anteriormente e no `forkJoin` para múltiplas chamadas na página de favoritos.
-   **Jasmine e Karma**: Para a escrita e execução dos testes unitários.

## 🧠 Arquitetura e Decisões Técnicas

-   **Componentes Standalone**: A aplicação foi construída utilizando a arquitetura de componentes standalone do Angular, que simplifica o gerenciamento de dependências e promove a modularidade.
-   **Serviços para Separação de Lógica**: A lógica de negócios foi separada em serviços para garantir um código limpo e organizado.
    -   `PokeapiService`: Responsável por todas as chamadas à API.
    -   `FavoritesService`: Responsável por toda a lógica de gerenciamento dos favoritos via `localStorage`.
-   **Persistência de Dados com `localStorage`**: A escolha do `localStorage` para o sistema de favoritos garante que as preferências do usuário sejam mantidas entre as sessões, de forma simples e eficaz para uma aplicação client-side.
-   **Otimização da Busca**: A busca por nome foi implementada para filtrar uma lista completa de mais de 1300 Pokémon de forma local e instantânea, melhorando a experiência do usuário.

## 🚀 Como Executar o Projeto

Para executar este projeto localmente, siga os passos abaixo:

```bash
# 1. Clone o repositório
git clone [https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git)

# 2. Navegue até a pasta do projeto
cd NOME_DO_SEU_REPOSITORIO

# 3. Instale as dependências
npm install

# 4. Inicie o servidor de desenvolvimento
ionic serve
```

## 🧪 Testes

Para rodar os testes unitários e verificar a integridade dos serviços, execute:

```bash
ng test
```

## 📫 Contato (43) 99619-7850

**Bruno Victorino Martins**

-   LinkedIn: [https://www.linkedin.com/in/SEU_LINKEDIN/](https://www.linkedin.com/in/SEU_LINKEDIN/)
-   Email: SEU_EMAIL@exemplo.com
