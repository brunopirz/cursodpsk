# Cursos Flix - Plataforma de Streaming Educacional

![Cursos Flix Logo](https://via.placeholder.com/150x50?text=Cursos+Flix)

Plataforma de streaming de cursos online com interface similar à Netflix.

## Pré-requisitos

- Docker e Portainer instalados
- Acesso à VPS (47.90.228.205)
- Domínio configurado (cursosflix.zapchat.shop)

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/brunopirz/cursodpsk.git
cd cursodpsk
docker-compose build

No Portainer:

Crie um novo Stack

Cole o conteúdo do docker-compose.yaml

Adicione as variáveis de ambiente

Deploy

Configuração Pós-Instalação
Configure o DNS:

A record para cursosflix.zapchat.shop → 47.90.228.205

CNAME para api.cursosflix.zapchat.shop → cursosflix.zapchat.shop

SSL:
O Traefik já configurado irá gerar certificados automaticamente via Let's Encrypt

Estrutura do Projeto
frontend/: Aplicação React.js

backend/: API Node.js/Express

db/: Banco de dados PostgreSQL

Variáveis de Ambiente
Variável	Descrição
DB_USER	Usuário do PostgreSQL
DB_PASSWORD	Senha do PostgreSQL
DB_NAME	Nome do banco de dados
JWT_SECRET	Segredo para autenticação JWT
STRIPE_KEY	Chave da API Stripe
