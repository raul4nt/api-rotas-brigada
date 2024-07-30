# Sistema de Otimização de Rotas da Brigada Militar para Patrulha Maria da Penha

## Descrição do Projeto

Este projeto foi desenvolvido como parte da disciplina de **Gestão Ágil de Projetos**, no quarto semestre da faculdade. O objetivo é criar um sistema que otimize as rotas da Brigada Militar para a Patrulha Maria da Penha, facilitando o registro e a gestão de visitas de proteção. Nosso grupo ficou com a parte de backend e frontend, onde a linguagem escolhida foi Python, e o framework utilizado para construção da API foi o Django.

## Funcionalidades: visão geral

- **Registro de Usuários e Autenticação**: Permite que novos usuários se registrem e façam login no sistema.
- **Painel de Navegação**: Interface principal para navegação entre as funcionalidades do sistema.
- **Exibição de Mapas com Direções**: Mostra direções e rotas otimizadas para as patrulhas.
- **Cadastro de Pessoas**: Formulário para cadastrar novas pessoas(agressores ou vítimas) no sistema.
- **Registro de Visitas e Priorização**: Registro detalhado das visitas e priorização baseada em critérios específicos(incluindo o formulário frida).
- **Registro de Medidas Protetivas**: Registro detalhado das medidas protetivas, com ênfase na gestão das mesmas.

## Detalhes da Implementação

### Registro de Medidas Protetivas(minha parte)

Esta funcionalidade foi feita por mim, criada para registrar medidas protetivas no sistema. Inclui a coleta de dados como número do processo, nome da vítima e do agressor, data e hora de registro, status da medida, e mais. A validação de campos obrigatórios e o envio dos dados para a API externa são realizados de forma segura e eficiente.

### Registro de Usuários e Autenticação

Implementado para permitir que novos usuários se registrem no sistema e façam login de forma segura. O sistema valida os dados de entrada e fornece mensagens de erro ou sucesso conforme necessário.

### Painel de Navegação

Um painel que serve como ponto central de navegação para acessar as diversas funcionalidades do sistema, como registrar visitas, ver mapas e gerenciar medidas protetivas.

### Exibição de Mapas com Direções

Integração com APIs de mapas para mostrar direções e rotas otimizadas para as patrulhas, facilitando a logística das operações.

### Registro e Priorização de Visitas

As visitas são registradas e priorizadas com base em critérios como a urgência e a criticidade da situação. A priorização ajuda a determinar quais visitas devem ser realizadas primeiro.

## Como Executar o Projeto

1. **Clone o repositório**:
    ```bash
    git clone https://github.com/usuario/projeto.git
    cd projeto
    ```

2. **Instale as dependências**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Execute as migrações do banco de dados**:
    ```bash
    python manage.py migrate
    ```

4. **Inicie o servidor**:
    ```bash
    python manage.py runserver
    ```

5. **Acesse o sistema** via [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Banco de Dados

O banco de dados utilizado no projeto foi criado por outro grupo e está hospedado no Vercel em [https://api-eproc-senac.vercel.app/](https://api-eproc-senac.vercel.app/). Nossa API se comunica com este banco para obter e registrar dados.

## Contribuidores

- **Raul(eu)**: Registro de medidas protetivas.
- **Jonas**: Implementação do registro de usuários e autenticação.
- **Cleiton**: Desenvolvimento do painel de navegação.
- **Lucas**: Implementação dos mapas e cadastro de pessoas.
- **Jonathan**: Registro e priorização de visitas.

