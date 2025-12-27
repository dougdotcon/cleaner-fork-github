# GitHub Fork Cleaner

Uma ferramenta completa projetada para gerenciar e limpar eficientemente seus repositórios fork do GitHub, utilizando uma interface gráfica moderna e intuitiva.

## Funcionalidades

- **Interface Gráfica Moderna:** Interface intuitiva construída com Python para facilitar o uso.
- **Visualização de Repositórios:** Visualize todos os seus forks em um painel centralizado.
- **Exclusão Inteligente:** Adiciona automaticamente uma estrela ao repositório antes de remover o fork, preservando o histórico.
- **Gerenciamento Seguro de Credenciais:** Manipulação segura de credenciais do GitHub usando variáveis de ambiente.
- **Acompanhamento de Progresso:** Feedback visual em tempo real sobre o status das operações.

## Pré-requisitos

- Python 3.7 ou superior
- Um Token de Acesso Pessoal do GitHub com as seguintes permissões:
  - `repo` (Controle total de repositórios privados)
  - `delete_repo` (Para deletar repositórios)

## Instalação

### 1. Clone o Repositório

bash
git clone https://github.com/seu-usuario/github_fork_cleaner.git
cd github_fork_cleaner


### 2. Instale as Dependências

É altamente recomendável usar um ambiente virtual:

bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
pip install -r requirements.txt


### 3. Configure as Credenciais

Renomeie o arquivo de ambiente de exemplo:

bash
mv .env.example .env


Edite o `.env` e adicione seus detalhes do GitHub:

ini
GITHUB_USERNAME=seu_usuario_github
GITHUB_TOKEN=seu_token_de_acesso_pessoal


## Uso

### Recomendado: Interface Gráfica (GUI)

Execute a aplicação principal para abrir a interface gráfica:

bash
python app_gui.py


**A interface gráfica permite que você:**
- Configure credenciais de forma segura.
- Busque e liste todos os seus forks.
- Selecione forks específicos para remover.
- Monitore o progresso das tarefas de exclusão.

### Alternativa: Linha de Comando (CLI)

Se preferir o terminal, execute a versão CLI:

bash
python app.py


## Melhores Práticas de Segurança

- **Nunca commit o arquivo `.env`** ou o envie para o controle de versão.
- **Limite as Permissões do Token:** Certifique-se de que seu token do GitHub tenha apenas os escopos necessários (`repo`, `delete_repo`).
- **Mantenha as Credenciais Seguras:** Não compartilhe seu token ou usuário publicamente.

## Contribuição

Contribuições são o que tornam a comunidade open-source um lugar incrível para aprender, inspirar e criar. Quaisquer contribuições que você fizer são **muito apreciadas**.

1. Fork o Projeto
2. Crie sua Branch de Funcionalidade (`git checkout -b feature/NovaFuncionalidade`)
3. Commite suas Alterações (`git commit -m 'Adiciona uma NovaFuncionalidade'`)
4. Envie para a Branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

## Licença

Distribuído sob a Licença MIT. Veja o arquivo `LICENSE` para mais informações.
