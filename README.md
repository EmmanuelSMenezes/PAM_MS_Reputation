# PAM_MS_Reputation

<div align="center">

[![.NET](https://img.shields.io/badge/.NET-6.0-512BD4?style=for-the-badge&logo=dotnet)](https://dotnet.microsoft.com/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker)](https://www.docker.com/)
[![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=for-the-badge&logo=swagger)](https://swagger.io/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

**Microservico de alta performance para a Plataforma PAM**

[Demo](#demo) â€¢ [Documentacao](#documentacao) â€¢ [Instalacao](#instalacao) â€¢ [Contribuicao](#contribuicao)

</div>

---

## Sobre o Projeto

Microservico para sistema de avaliacoes e reputacao. Gerencia ratings, reviews detalhados, comentarios, sistema de pontuacao de parceiros e servicos, moderacao de conteudo, analise de sentimento e ranking de qualidade.

### Principais Funcionalidades

- **Avaliacoes**: Sistema de rating 1-5 estrelas
- **Reviews**: Comentarios detalhados
- **Rankings**: Classificacao de parceiros
- **Moderacao**: Filtro de conteudo
- **Analytics**: Analise de sentimento
- **Recomendacoes**: Sugestoes baseadas em rating
- **Tendencias**: Evolucao da reputacao
- **Denuncias**: Sistema de reports

## Tecnologias

### Core Framework
- **[.NET 6.0](https://dotnet.microsoft.com/)** - Framework principal
- **[ASP.NET Core](https://docs.microsoft.com/aspnet/core/)** - Web API framework
- **[Entity Framework Core](https://docs.microsoft.com/ef/core/)** - ORM para acesso a dados

### Documentacao e Testes
- **[Swagger/OpenAPI](https://swagger.io/)** - Documentacao interativa da API
- **[FluentValidation](https://fluentvalidation.net/)** - Validacao de dados
- **[AutoMapper](https://automapper.org/)** - Mapeamento de objetos
- **[xUnit](https://xunit.net/)** - Framework de testes

## Pre-requisitos

- **[.NET 6.0 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)** (versao 6.0 ou superior)
- **[Docker Desktop](https://www.docker.com/products/docker-desktop)** (opcional)
- **[SQL Server](https://www.microsoft.com/sql-server)** (banco de dados)
- **[Visual Studio 2022](https://visualstudio.microsoft.com/)** (IDE recomendada)

## Instalacao

### 1. Clone o Repositorio

`ash
git clone https://github.com/EmmanuelSMenezes/PAM_MS_Reputation.git
cd PAM_MS_Reputation
`

### 2. Configuracao do Ambiente

`ash
cp WebApi/appsettings.example.json WebApi/appsettings.Development.json
`

### 3. Restaurar Dependencias

`ash
dotnet restore
`

### 4. Executar Migracoes

`ash
cd WebApi
dotnet ef database update
cd ..
`

### 5. Executar o Projeto

`ash
cd WebApi
dotnet run
`

### 6. Verificar Instalacao

- **API**: http://localhost:5011
- **Swagger UI**: http://localhost:5011/swagger
- **Health Check**: http://localhost:5011/health

## Docker

`ash
# Build
docker build -t pam_ms_reputation .

# Run
docker run -p 5011:5011 pam_ms_reputation
`

## Testes

`ash
dotnet test
`

## Contribuicao

1. Fork o projeto
2. Crie uma branch (git checkout -b feature/nova-funcionalidade)
3. Commit suas mudancas (git commit -m 'feat: nova funcionalidade')
4. Push para a branch (git push origin feature/nova-funcionalidade)
5. Abra um Pull Request

## Licenca

Este projeto esta sob a licenca **MIT**. Veja [LICENSE](LICENSE) para mais detalhes.

## Suporte

- **Email**: suporte@pam.com
- **Issues**: [GitHub Issues](https://github.com/EmmanuelSMenezes/PAM_MS_Reputation/issues)

---

<div align="center">

**PAM - Plataforma de Agendamento de Manutencao**  
*Desenvolvido com amor pela equipe PAM*

</div>