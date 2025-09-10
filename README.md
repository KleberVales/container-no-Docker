# 🎯 Criando seu primeiro container no Docker

A ideia aqui é entender como rodar qualquer aplicação simples dentro de um container para começar a se familiarizar.

## 1. Verificando a instalação do Docker

Depois de instalar, veja se está funcionando:

```bash

docker --version
docker info

```

## 2. Rodando seu primeiro container (Hello World)

O Docker tem uma imagem oficial de teste:

```bash

docker run hello-world

```

👉 Isso baixa a imagem do Docker Hub (se ainda não existir localmente) e cria um container que apenas imprime uma mensagem.

## 3. Rodando um container interativo (Ubuntu)

Agora vamos rodar um container Linux interativo:

```bash

docker run -it ubuntu bash

```

- -it → interativo (teclado + terminal)
- ubuntu → nome da imagem
- bash → comando a executar no container

Você estará dentro de um Ubuntu isolado!\
Pode rodar comandos como ls, pwd, cat /etc/os-release.

Para sair:

```bash

exit

```

## 4. Rodando um container em background (Nginx)


