## CatalogoAPI

Projeto criado durante a realização do curso - Curso Web API ASP .NET Core Essencial, ministrado por Macoratti na Udemy.

Foram utilizadas as seguintes tecnologias: 
- ASP .NET Core Web API
- C#

O objetivo desse projeto era criar uma Web API usando uma arquitetura limpa.

Arquitetura limpa ou Clean Architecture - Robert C. Martin (Uncle Bob):

- Definir uma arquitetura desacoplada e robusta;
- Criar projetos distintos separados conforme a sua responsabilidade;
- Usar a inversão de controle e injeção de dependência.
      Tornar o projeto fácil de manter, testar e estender.

Características desejadas:
- Independente de Frameworks
- Testável 
- Independente da Camada de Apresentação (UI)
- Independente do Banco de dados.
- Independente de fatores externos.

Regra de dependência 
- As camadas internas não devem ter qualquer dependência das externas, nem indiretas, como nomes de variáveis e funções.

CatalogoAPI foi desenvolvida com uma solução (ASP .NET Core Web API) e com 5 projetos distintos (Class Library (.NET 5.0)):

- Catalogo.Domain → Modelo de domínio, Interfaces, regras de negócio.
- Catalogo.Application → Regras da aplicação, serviços, mapeamento, DTOs.
- Catalogo.Infrastructure → Lógica Acesso a dados, Contexto, Configurações, ORM.
- Catalogo.CrossCutting → IoC, Registro dos Serviços e recursos, DI.
- Catalogo.API → Controladores, endpoints, filtros.




