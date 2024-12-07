
---

# **GitHub Fork Cleaner**

Uma ferramenta Python simples para ajudar a organizar sua conta do GitHub, removendo repositórios forkados e mantendo apenas os repositórios que você criou. Antes de excluir os forks, o script adiciona uma estrela (star) como forma de registrar que você utilizou ou apreciou o repositório.

---

## **Por que usar este script?**
Se sua conta do GitHub está cheia de repositórios forkados e você deseja mantê-la organizada, este script é uma solução automatizada para:
- Identificar repositórios forkados.
- Adicionar uma estrela (star) a eles.
- Excluir os repositórios forkados, mantendo apenas os criados por você.

---

## **Pré-requisitos**
1. Python 3.6 ou superior instalado.
2. Biblioteca `requests` instalada:
   ```bash
   pip install requests
   ```
3. Um token de acesso pessoal (PAT) do GitHub com as seguintes permissões:
   - `repo`: Acesso a repositórios públicos e privados.
   - `delete_repo`: Permissão para excluir repositórios.
   - `write:star`: Permissão para adicionar estrelas.

---

## **Como obter o token do GitHub?**
1. Acesse suas configurações no GitHub.
2. Vá até **Developer settings** > **Personal access tokens** > **Tokens (classic)**.
3. Clique em **Generate new token** e selecione as permissões mencionadas acima.
4. Salve o token gerado (ele será exibido apenas uma vez).

Para mais detalhes, veja o guia completo [aqui](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).

---

## **Configuração**
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/github-fork-cleaner.git
   ```
2. Edite o arquivo `fork_cleaner.py` e substitua:
   - `seu_usuario` pelo seu nome de usuário do GitHub.
   - `seu_token` pelo token gerado.

---

## **Uso**
1. Execute o script:
   ```bash
   python fork_cleaner.py
   ```
2. O script irá:
   - Listar todos os seus repositórios.
   - Identificar quais são forks.
   - Adicionar uma estrela aos forks.
   - Excluir os forks (após confirmação).

---

## **Exemplo de Execução**
```bash
Buscando repositórios...
Encontrados 50 repositórios.
Encontrados 10 forks para processar.
Tem certeza de que deseja adicionar uma estrela e excluir 10 forks? (sim/não): sim
Estrela adicionada ao repositório user/repo1.
Repositório user/repo1 excluído com sucesso.
...
Processo concluído.
```

---

## **Aviso**
- As exclusões são permanentes. Certifique-se de que não há informações importantes nos forks antes de executar o script.
- Use este script por sua conta e risco.

---

## **Contribuições**
Contribuições são bem-vindas! Se você encontrou um bug ou tem uma ideia para melhorar este script, fique à vontade para abrir uma issue ou enviar um pull request.

---

## **Licença**
Este projeto está licenciado sob a [MIT License](LICENSE).

---

## **Contato**
Se você tiver dúvidas ou precisar de ajuda, entre em contato:
- **Email**: dougdotcon@gmail.com
- **GitHub**: [dougdotcon](https://github.com/dougdotcon)

---

## **Inspirado por minha própria jornada**
Este projeto nasceu da minha necessidade de organizar meu próprio GitHub, que estava desorganizado por falta de prática. Espero que ele também possa ajudar você! 😄
