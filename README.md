# Curso-WEBIOM-2025

Repositório criado para detalhar os passos do curso prático de bioinformática que será ministrado no WEBIOM2025.


## Sinopse

O Sequenciamento de Nova Geração (NGS) tem possibilitado uma produção sem precedentes de dados genéticos. A análise subsequente desses dados, em busca de variantes genéticas que possam estar associadas a determinado fenótipo, é um importante passo para novas alternativas de diagnóstico e tratamento personalizado de pacientes. Este minicurso visa introduzir como é feito o tratamento dos dados de NGS advindos de DNA humano por meio de ferramentas de bioinformática, passando pelas etapas de análise de qualidade, alinhamento, chamada e anotação de variantes.

## Como instalar o git

```bash
sudo apt-get install git-all
```

> Para mais informações e outros sistemas operacionais, [clique aqui](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git)

## Como clonar esse repositório

1. Vá para uma pasta onde queira deixar este repositório;
2. Use o comando abaixo:

```bash
git clone https://github.com/Wilsonjsjunior/Curso-ONCOGEN-2022.git
```

## Como instalar conda

* [Link ensinando como instalar](https://conda.io/docs/user-guide/install/index.html)

## Como rodar o container Docker

Faça a instalação do Docker de acordo com o seu sistema operacional:

* [Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows) (Para usar o Docker no Windows, use o [Cmder](http://cmder.net/) para emular um terminal)
* [Ubuntu](https://store.docker.com/editions/community/docker-ce-server-ubuntu)
* [Mac](https://store.docker.com/editions/community/docker-ce-desktop-mac)

As instalações de outros sistemas operacionais podem ser encontradas [aqui](https://www.docker.com/community-edition).

Após a instalação, faça a build da imagem no seu computador:

```bash
dodocker build -t oncogene -f dockerfile .
```

Vá para o diretório do repositório do curso, e depois crie um container com a imagem baixada, utilizando o seguinte comando:

```bash
docker run -v ~/Curso-ONCOGEN-2022/curso:/curso -it oncogene
```

No final, será criado um container com todos os softwares necessários para a execução prática do curso já instalados.
