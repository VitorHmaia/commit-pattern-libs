# Importância do padrão de commit e suas ferramentas 

Diferentes bibliotecas para implementar o padrão de commit [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/#summary): [Husky](https://typicode.github.io/husky/), [Commitlint](https://commitlint.js.org/#/), e [Commitizen](https://commitizen-tools.github.io/commitizen/)


## Requisitos Funcionais

- Python versão 3.8 ou superior
- Node.js na versão v18.18.2 ou superior
- Git versão 1.8.5.2 ou superior

### Ambiente de Desenvolvimento Integrado (IDE)
- Recomendamos o uso do VSCode ou PyCharm, na versão mais recente.

### Sistema Operacional (SO)
- O projeto foi testado e é compatível com Windows e Linux.

### Terminais

- Recomendo os seguintes terminais para executar os comandos: Git Bash, Zsh, PowerShell, Bash, Cmd.  

## Requisitos Não Funcionais

### Conhecimentos Necessários
- Python: Conhecimento básico é recomendado.
- Node.js: Conhecimento básico é suficiente.
- Git: Conhecimento básico é necessário.


## Tecnologias Utilizadas

### Python

Python é uma linguagem de programação interpretada, de alto nível e de propósito geral. Ela é amplamente utilizada para desenvolvimento web, automação, análise de dados, entre outros.

Certifique-se de ter o Python instalado e, em seguida, instale as dependências Python necessárias:

```bash
pip install -r requirements.txt
```

### Node.js

O Node.js é uma plataforma construída sobre o motor JavaScript V8 do Google Chrome para desenvolver aplicações de rede escaláveis. Ele facilita a construção de aplicações JavaScript do lado do servidor.

Para instalar as dependências do Node.js, utilize o seguinte comando:

```bash
npm install
```

### Husky

Husky é uma ferramenta que permite automatizar tarefas antes de commits e pushes no Git (por via dos hooks). No atual projeto, estamos utilizando o Husky para integrar o Commitlint e garantir que os commits sigam a convenção de commits convencionais.


### Commitlint

Commitlint é uma ferramenta de verificação de mensagens de commit. Ele ajuda a garantir que as mensagens de commit sigam uma convenção predefinida, como a Conventional Commits.

Na imagem abaixo é possível ver um caso onde o commitlint atua, visto que o commit não está seguindo o padrão, ele impede a realização do mesmo e indica o que deve ser alterado:

![Alt text](./images/commitlint-exemplo.png)


### Commitizen

Commitizen é uma ferramenta para facilitar a criação de mensagens de commit seguindo a convenção predefinida. Ele fornece uma interface interativa para gerar mensagens de commit no formato correto.

#### Como utilizar:

Visto que o Commitizen gera um cli, não devemos utilizar mais o comando ```git commit -m``` para esta finalidade, utilizamos a seguinte ordem:

1. Após feita as alterações no código-fonte, devemos designar as mesmas para o ambiente de staged, com o comando:
```git add```

2. Agora é o momento que chamamos a interface do Commitizen, com o comando realizado preferencialmente no terminal do Git Bash:
```git cz```

3. A imagem abaixo corresponde a CLI, que de forma interativa (com as setas do teclado) podemos navegar e escolher o tipo do commit:
![Alt text](./images/cli-commitizen.png)

4. Dessa forma, será realizada uma série de perguntas que nos auxiliam na construção do commit, seguindo a convenção:
![Alt text](./images/commit.png)


Espero que estas sugestões e a conversão atendam às suas expectativas! Se precisar de mais alguma coisa, estou à disposição.


