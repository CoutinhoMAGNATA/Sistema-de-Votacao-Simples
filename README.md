Votação Turma
# Descrição
Votação Turma é um sistema simples e eficiente desenvolvido em Python com o framework Django, utilizando a interface administrativa do Django Admin para o gerenciamento. O objetivo principal é facilitar a eleição de representantes de turma de forma organizada e com validação de voto único.
O sistema é ideal para escolas, universidades ou qualquer ambiente que necessite de uma ferramenta rápida para conduzir votações internas.

# Funcionalidades
Gerenciamento de Eleições: Cadastro, edição e controle de eleições (título, descrição, período de início e fim).
Cadastro de Candidatos: Associação de candidatos a eleições específicas, incluindo nome e número.
Controle de Voto Único: Garante que cada usuário autenticado vote apenas uma vez por eleição.
Validação de Período: Permite votos apenas durante o período ativo da eleição.
Visualização de Resultados: Exibição da contagem de votos e percentual por candidato após o término da eleição.
Interface Administrativa Amigável: Utiliza o Django Admin para a administração completa do sistema.
Gerenciamento de Usuários: Utiliza o sistema de autenticação padrão do Django.

# Como Usar
Siga os passos abaixo para configurar e rodar o projeto localmente.
# Pré-requisitos
Python 3.x
pip (gerenciador de pacotes do Python)


1. Clonar o Repositório
Descompacte o arquivo do projeto e navegue até o diretório principal:
Bash
unzip VotacaoTurma.zip
cd VotacaoTurma


3. Configurar o Ambiente Virtual
É altamente recomendável usar um ambiente virtual para isolar as dependências do projeto:
Bash
# Cria o ambiente virtual
python3.11 -m venv venv

# Ativa o ambiente virtual
source venv/bin/activate


# Ativa o ambiente virtual
source venv/bin/activate

3. Instalar as Dependências
Instale todas as bibliotecas necessárias listadas no arquivo requirements.txt:
Bash
pip install -r requirements.txt

5. Rodar as Migrações
Aplique as migrações do banco de dados para criar as tabelas necessárias:
Bash
python manage.py migrate

7. Criar um Superusuário
Crie um usuário administrador para acessar a interface do Django Admin e gerenciar as eleições:
Bash
python manage.py createsuperuser

9. Iniciar o Servidor
Inicie o servidor de desenvolvimento do Django:
Bash
python manage.py runserver

11. Acessar o Sistema
O sistema estará acessível em http://127.0.0.1:8000/.
Interface Administrativa: Acesse http://127.0.0.1:8000/admin com o superusuário criado para cadastrar eleições e candidatos.
Interface de Votação: Acesse http://127.0.0.1:8000/votacao para que os usuários logados possam visualizar as eleições ativas e votar.
Licença: Projeto open source para fins educativos e comerciais.
