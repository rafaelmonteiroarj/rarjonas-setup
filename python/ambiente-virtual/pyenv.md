### Passo a passo para usar o pyenv:

Instale o pyenv:

No Linux ou macOS, você pode instalar o pyenv seguindo estes comandos:

```shell
curl https://pyenv.run | bash
```

Após a instalação, adicione as seguintes linhas ao seu arquivo de configuração de

```shell
shell (~/.bashrc, ~/.zshrc, ou equivalente):
```

```shell
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```

Depois de fazer isso, execute:

```shell
source ~/.bashrc  # ou ~/.zshrc se estiver usando zsh
```

#### Instale uma versão do Python:

Para listar as versões disponíveis do Python para instalação, use o comando:

```sh
pyenv install --list
```

Para instalar uma versão específica (exemplo: Python 3.11):

```sh
pyenv install 3.11
```

Defina a versão global ou local do Python:

Você pode definir uma versão global (para ser usada em todo o sistema):

```sh
pyenv global 3.11
````

Ou definir uma versão específica apenas para o diretório atual:

```sh
pyenv local 3.9.10
````

#### Ative o ambiente virtual:

Para ativar o ambiente virtual criado, use:

```sh
pyenv activate myenv
````

Desative o ambiente virtual:

Para desativar o ambiente, use:

```sh
pyenv deactivate
````

Listar os ambientes virtuais criados:

Para ver os ambientes criados com o pyenv-virtualenv, use:

```sh
pyenv virtualenvs
````

#### Resumo:
O pyenv gerencia versões de Python.
O pyenv-virtualenv é um complemento para gerenciar ambientes virtuais.
Com ele, você pode criar ambientes virtuais específicos para cada versão de Python instalada.