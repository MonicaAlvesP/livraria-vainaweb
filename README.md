# Livraria - Sistema de Doação de Livros

Este é um projeto fullstack de uma plataforma de doação de livros desenvolvido como projeto final do curso Vai na Web. O sistema permite que os usuários doem e vejam livros disponíveis para leitura.

## Estrutura do Projeto

O repositório está organizado em dois subprojetos principais:

- **front-livraria**: Frontend desenvolvido em React
- **api-livraria**: API desenvolvida em Flask (Python)

## Tecnologias Utilizadas

#### Frontend

- React com hooks
- React Router DOM para navegação
- Sass para estilização modular
- Vite como bundler e dev server

#### Backend

- Flask (Python)
- SQLite para armazenamento de dados

## Funcionalidades Principais

- Página inicial com informações sobre os benefícios de doar livros
- Cadastro de livros para doação
- Visualização de todos os livros doados
- Visualização detalhada de cada livro contendo sinopse
- Interface responsiva para diferentes dispositivos

## Rotas e Endpoints

#### Frontend

- `/`: Página inicial com informações sobre doação de livros
- `/livrosDoados`: Exibe todos os livros disponíveis no sistema
- `/queroDoar`: Formulário para doação de novos livros
- `/detalhesLivro/:id`: Visualização detalhada do livro selecionado

#### API Backend

- `GET /`: Página inicial da API
- `POST /doar`: Cadastra um novo livro
- `GET /livros-doados`: Retorna todos os livros cadastrados
- `GET /livros-doados/:id`: Retorna detalhes de um livro específico

## Como Executar

### Pré-requisitos

- Node.js e npm para o frontend
- Python para o backend

### Como Baixar o Projeto com Submódulo

1. Clone o repositório principal com o comando:

```bash
git clone --recurse-submodules https://github.com/MonicaAlvesP/livraria-vainaweb.git
```

2. Caso já tenha clonado o repositório sem os submódulos, inicialize-os com:

```bash
git submodule update --init --recursive
```

3. Navegue até os diretórios dos subprojetos para instalar as dependências e subir o servidor:

- **Frontend**:

  ```bash
  cd front-livraria
  npm install
  npm run dev
  ```

- **Backend**:
  ```bash
  cd api-livraria
  pip install -r requirements.txt
  python app.py
  ```

4. Execute os subprojetos conforme as instruções específicas de cada um.

## Desafios e Aprendizados

Durante o desenvolvimento deste projeto, foram aplicados conhecimentos em:

- Integração entre frontend React e backend Flask
- Implementação de rotas dinâmicas com React Router
- Estilização responsiva com Sass e módulos SCSS
- Gerenciamento de estados e ciclo de vida de componentes
- Consumo de API com Axios e tratamento de erros
- Estruturação do banco de dados SQLite

## Autora

Mônica Alves Pereira - [LinkedIn](https://www.linkedin.com/in/dev-alves/) | [GitHub](https://github.com/MonicaAlvesP)

---

Projeto desenvolvido como trabalho final do curso Vai na Web, sob orientação dos instrutores [Fernanda Corrêa](https://github.com/NandaCorreaa) e [João Pedro](https://github.com/silvajpedro).
