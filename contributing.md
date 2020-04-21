# Executar um jupyter notebook

Depois de clonar esse repositório, execute dentro da pasta `docker build -t jupyter-tutorial .`

Com a imagem docker criada, execute `sh start-notebook.sh`

O servidor irá mostrar no terminal uma URL para você copiar no navegador. Pronto você deve ser capaz de ver seu Jupyter Notebook no navegador.

# Problemas encontrados

Usando Ubuntu, eu nao conseguia criar novos jupyter notebooks. A documentação da [imagem docker](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html) aponta para o uso das flags `--user <os-user-id> --group-add users`: https://jupyter-docker-stacks.readthedocs.io/en/latest/using/common.html 

Para descobrir <os-user-id>: https://www.howtogeek.com/438435/how-to-use-the-chown-command-on-linux/