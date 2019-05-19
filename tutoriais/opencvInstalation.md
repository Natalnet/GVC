# Instalação do OpenCV para python

![opencvLogo](../readme_imgs/opencv.jpg)

Esse tutorial tem como objetivo a instalação da bibloteca OpenCV em um ambiente python sendo assim se faz necessário a posse de um ambiente virtual funcional, caso não o possua siga [esse tutorial](./pythonVirtualEnvs.md).

OpenCV (Open Source Computer Vision) é uma biblioteca de programação, de código aberto e inicialmente desenvolvida pela Intel com o objetivo de tornar a visão computacional mais acessível a desenvolvedores e hobistas.

## Instalação

Com seu ambiente virtual ativado siga os comandos relativos a seu tipo de ambinete para a instalação da bilioteca.

### Venv

Para os usuários do venv alguns pacotes estão disponíveis e podem ser verificados através do comando:

```console
(<nome_do_ambiente>) user@computer:~$ pip search opencv | grep python | grep opencv-

opencv-python (4.1.0.25)                   - Wrapper package for OpenCV python bindings.
opencv-python-armv7l (3.2.0)               - opencv-python on armv7l.
opencv-python-aarch64 (3.3.0.1)            - Wrapper package for OpenCV python bindings.
opencv-python-headless (4.1.0.25)          - Wrapper package for OpenCV python bindings.
opencv-contrib-python (4.1.0.25)           - Wrapper package for OpenCV python bindings.
opencv-contrib-python-headless (4.1.0.25)  - Wrapper package for OpenCV python bindings.
opencv-python-inference-engine (4.1.1.1)   - Wrapper package for OpenCV 4 #e28e3c9 with Inference Engine 2019_R1.0.1 python bindings
```

Escolha a opção mais relevante para suas necessidades e instale-a seguindo o seguinte comando (**recomenda-se a opencv-contrib-python**):

```console
(<nome_do_ambiente>) user@computer:~$ pip install <nome_do_pacote>
```

Estejam cientes de que em alguns testes realizados utilizando os pacotes disponíveis nos repositórios PyPi **não foi possível exibir imagens** devido a inconsistências de compatibilidade dos arquivos pré compilados dos módulos com o GTK e Qt na máquinas utilizadas para os testes, ainda não foi encontrado uma solução simples sendo a única disponível complilar manualmente a biblioteca e apontar a utilização de interpretador python do seu ambiente.

## Anaconda ou Miniconda

Para os usuários de ambientes com a ferramenta conda estão disponíveis ainda mais opções para está biblioteca, presente em diversos canais tento atender todas as possíveis necessidades do projeto.

Para verificar as opções disponíveis execute o comando:

```console
(<nome_do_ambiente>) user@computer:~$ conda search opencv

opencv                         2.4.2      np17py27_1  pkgs/free
opencv                         2.4.6      np18py27_0  pkgs/free
opencv                         2.4.9      np18py27_0  pkgs/free
opencv                        2.4.10     np110py27_1  pkgs/free
opencv                         3.1.0     np112py36_1  pkgs/free
opencv                         3.3.1  py36h9248ab4_2  pkgs/main
opencv                         3.4.2  py27h40b0b35_1  pkgs/main
```

Escolha a opção mais relevante para suas necessidades e instale-a seguindo o seguinte comando (**recomenda-se a versão mais recente**):

```console
(<nome_do_ambiente>) user@computer:~$ conda install opencv==<versao>
```

Estejam cientes de que em alguns testes realizados utilizando os pacotes disponíveis nos repositórios conda foram encontrados problemas para exibir imagens, para resolver o excute o seguinte comando:

```console
(<nome_do_ambiente>) user@computer:~$ conda install -c loopbio -c conda-forge -c pkgw-forge ffmpeg gtk2
```

## Dúvidas, comentários e sugestões

Entrar em contato com [Richardson Santiago](https://github.com/vanluwin).