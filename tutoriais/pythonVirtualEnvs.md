# Ambientes Virtuais Python

![pythonVirtualEnv](../readme_imgs/pythonVirtualEnv.webp)

Esse tutorial tem como objetivo a implemetação de um abiente virtual para desenvolvimento com a linguagem python.

Ambientes virtuais surgiram com o objetivo de isolar a instalação python padrão do seu sistema operacional das usadas para desenvolvimento, posibilitando assim utilizar versões complementamente distintas da linguagem em cada projeto sem que uma interfira na outra.

Sendo assim com a utilização de tais ambientes o desenvolvedor fica livre para criar um ambiente para cada projeto se assim desejar e distribuir as configurações desse ambientes que conterão apenas os pacotes relevantes para o projeto em questão.

Aqui serão apresetadas três opções para a criação de tais ambientes:

* [Venv](https://docs.python.org/3/library/venv.html)
* [Anaconda](https://www.anaconda.com)
* [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

O primeiro sendo a ferrenta distribuida junto com as distribuições da linguagem python sendo um tanto mais complicada de configurar não tendo privilégios de super usuário na maquina em questão. Já Ananconda e Miniconda te daram acesso a um novo gerenciador de pacotes python o **conda**, que lhe dá acesso a ainda mais opções de versões de módulos python a diferença entre eles se da principalmente no uso do disco, Anaconda consumirá **muito** espaço no entanto instalará automaticamente muitos pacotes que podem ser úteis, já o Miniconda terá uma pegada menor no seu disco contudo exigirá um conhecimento maior dos pacotes a serem instalados.

Leitura adicional sobre a diferença entre as opções [aqui](http://deeplearning.lipingyang.org/2018/12/23/anaconda-vs-miniconda-vs-virtualenv/), mitos e equívocos sobre conda [aqui](https://jakevdp.github.io/blog/2016/08/25/conda-myths-and-misconceptions/).

## Venv

A criação de um ambiente se dá de maneira muito simples pois o utilitário a ser utilizado é distribuido juntamente com a maioria das distribuições python. Sendo assim abra o terminal, crie um diretório para armazenamento de seus ambientes e inicie seu ambiente tal terefa pode ser realizada seguindo os seguintes comandos ( **substituindo <nome_do_ambiente>** pelo nome que deseja dar a seu ambiente):

```console
user@computer:~$ mkdir myEnvs
user@computer:~$ cd myEnvs
user@computer:~/myEnvs $ python3 -m venv <nome_do_ambiente>
```

Para ativar o seu ambinete faça:

```console
user@computer:~$ source ~/myEnvs/<nome_do_ambiente>/bin/activate
```

Com seu ambinete ativado, para instalar um pacote faça:

```console
(<nome_do_ambiente>) user@computer:~$ pip install <nome_do_pacote>
```

## Anaconda e Miniconda

Considere a diverença entre as opções descritas na primeira seção deste tutorial, então siga os passos para instalação de uma das opções em sua máquina:

* [Anaconda](https://www.anaconda.com/distribution/)
* [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

Com uma das opções intalada abra o terminal e siga os comandos para criar o ambiente (**substituindo <nome_do_ambiente>** pelo nome que deseja dar a seu ambiente):

```console
user@computer:~$ conda create -n <nome_do_ambiente> python=3
```

Para ativar o seu ambinete faça:

```console
user@computer:~$ conda activate <nome_do_ambiente>
```

ou

```console
user@computer:~$ source activate <nome_do_ambiente>
```

Com seu ambinete ativado, para instalar um pacote faça:

```console
(<nome_do_ambiente>) user@computer:~$ conda install <nome_do_pacote>
```

## Dúvidas, comentários e sugestões

Entrar em contato com [Richardson Santiago](https://github.com/vanluwin)