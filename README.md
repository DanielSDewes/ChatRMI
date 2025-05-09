# ChatRMI

## Descrição
ChatRMI é uma aplicação de chat básica implementada usando Java RMI (Remote Method Invocation). Ela permite que múltiplos clientes enviem mensagens para um servidor remoto, que as exibe no console. Este projeto serve como uma introdução à computação distribuída e à comunicação remota em Java.

## Estrutura do Projeto
```
📂 ChatRMI/
┣ 📂 src/
┃ ┣ 📂 chat/
┃ ┃ ┣ 📂 model/ 
┃ ┃ ┃ ┣ 📜 ChatServidor.java  # Interface RMI para o servidor
┃ ┃ ┃ ┣ 📜 ChatCliente.java   # Interface RMI para o cliente
┃ ┃ ┣ 📂 service/ 
┃ ┃ ┃ ┣ 📜 ChatServidorImpl.java  # Implementação do servidor
┃ ┃ ┃ ┣ 📜 ChatMainServidor.java  # Classe principal para iniciar o servidor
┃ ┃ ┃ ┣ 📜 ChatMainCliente.java  # Classe principal para o cliente
```

## Funcionalidades
- Os clientes podem enviar mensagens para um servidor central.
- O servidor recebe e exibe as mensagens em tempo real.
- Utiliza Java RMI para comunicação remota.

## Instalação e Execução
### 1. Compile o projeto (vá para a pasta src)
```
javac chat/model/*.java chat/service/*.java
```

### 2. Execute o servidor
```
java chat.service.ChatMainServidor
```

### 3. Execute o cliente
```
java chat.service.ChatMainCliente
```

## Requisitos
- Java 8 ou superior

### Desenvolvido como parte de um exercício de sistemas distribuídos.