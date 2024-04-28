<h1 align="center"><font color="red">ML Project with Hydra and poetry</font></h1>

<font color="yellow">Data Scientist.: Dr. Eddy Giusepe Chirinos Isidro</font>

Neste pequeno projeto de `Machine Learning` usamos [Hydra](https://hydra.cc/docs/intro/), [poetry](https://python-poetry.org/) e `python`. Utilizamos `Hydra` para executar nosso pipeline de `Machine Learning`, já que oferece uma maneira flexível de configurar e gerenciar parâmetros (ou hiperparâmetros) nos programas de Python e porque o Hydra ajuda a separar a lógica do código da lógica de configuração. Ademais, usamos `poetry` porque é uma ferramenta para gerenciamento de dependências e empacotamento em Python. Ele permite que você declare as bibliotecas das quais seu projeto depende e irá gerenciá-las (instalá-las/atualizá-las) para você. Basicamente, `poetry` simplifica o processo de gerenciamento de dependências e criação de ambientes virtuais.  


Neste projeto focarei no uso do `poetry` em outro momento explicarei o uso de `Hydra`. Então, os passos para usar `poetry`, são:

## <font color="gree">Instalação do Poetry</font>

Você pode instalar o Poetry usando o pip, o gerenciador de pacotes do Python:
```
$ pip install poetry
```

## <font color="gree">Criando um Novo Projeto com Poetry</font>

* Para criar um novo projeto com `Poetry`, navegue até o diretório onde deseja criar o projeto e execute o seguinte comando:
```
$ poetry new nome_do_projeto
```

* Ou navegue até o diretório do projeto `clonado` no seu terminal. Dentro do diretório do projeto, execute o seguinte comando para iniciar um novo projeto Poetry:

```
$ poetry init
```
Isso criará um novo arquivo `pyproject.toml` e você será solicitado a fornecer informações sobre o projeto, como nome, versão, autor, etc.


## <font color="gree">Gerenciamento de Dependências</font>

* Adicionar uma nova dependência:
```
$ poetry add nome_do_pacote

Exemplos:

$ poetry add requests
$ poetry add pandas        ou      $ poetry add pandas==2.2.2
```

* Remover uma dependência:
```
$ poetry remove nome_do_pacote

Exemplos:

$ poetry remove pandas
$ poetry remove python-dotenv
```

* Atualizar dependências:
```
$ poetry update
```

## <font color="gree">Gerenciamento de Ambientes Virtuais</font>

* Criar um novo ambiente virtual:
```
$ poetry install
```
Isso criará um ambiente virtual isolado para o seu projeto e instalará as dependências listadas no arquivo `pyproject.toml`.

* Ativar o ambiente virtual:
```
$ poetry shell
```
Isso ativará o ambiente virtual, permitindo que você trabalhe no contexto do seu projeto.

* Sair do ambiente virtual:
```
$ exit
```

## <font color="gree">Outros Comandos Úteis</font>

* Para mostrar informações sobre o projeto e suas dependências:
```
$ poetry show
```

* Para executar um script Python no contexto do ambiente Poetry:
```
$ poetry run python meu_script.py      ou     $ python meu_script_python.py
```

Além disso, você pode verificar se o `ambiente virtual` está ativado verificando se o comando `python` aponta para o interpretador Python dentro do `ambiente virtual do Poetry`. Você pode fazer isso executando:
```
$ which python
```
Se o caminho retornado estiver dentro do diretório do ambiente virtual do Poetry, então o ambiente está ativado corretamente.




Thanks God 🤓!