# ratts-server_docker-install
Instalador da imagem docker (ratts-server)
instale as versões mais recentes do container docker ratts-server
mais informações: [ratts-server](https://hub.docker.com/r/ratts13/ratts-server)

## Requisitos
Ter git instalado em sua maquina (fisica ou virtual)
**sudo apt install git** ubuntu & debian

#função

instalar automaticamente todas as imagens e dependencias necessarias para instalar e rodar o docker ratts-server
use **git clone** para clonar este repositorio. Após a clonagem, atualize as permições do arquivo **start** para executável com o comando **chmod +x start**.

feito isso, execute no terminal: **~$ratts-server_docker-install# sudo ./start**

agora ele vai baixar e executar a imagem.

## Funções basicas

Para sair da sua imagem e voltar para o host (desligando o server): **exit ou ctrl+d**
para sair da sua imagem e voltar para o host (sem desligar o server) **ctrl + p + q**
detalhes da imagem em execução: **sudo docker ps**
voltar para a linha de comando do containner: **sudo docker attach [[id da imagem]]**
