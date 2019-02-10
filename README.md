# ratts-server_docker-install: v1.0
Instalador da imagem docker (ratts-server)
instale as versões mais recentes do container docker ratts-server
mais informações: [ratts-server](https://hub.docker.com/r/ratts13/ratts-server)

Para ultilizar o sistema de automação do **ratts-server**, é nescessário ter o Docker instalado.
Caso não tenha baixado, segue abaixo os metodos de instalação do docker:

## Instalação Docker:
### metodo 01
no terminal, execute **curl -sSL https://raw.githubusercontent.com/victorratts13/ratts-server_docker-install/master/install.sh | sh** e dê um enter e aguarde a instalação do docker em sua maquina.
### metodo 02
execute **chmod +x install.sh** para tornar o arquivo executavel e depois execute-o com **./install.sh**

# Ultilizando o Ratts-server Start

## Requisitos
Ter git instalado em sua maquina (fisica ou virtual)
**sudo apt install git** ubuntu & debian

### função

instalar automaticamente todas as imagens e dependencias necessarias para instalar e rodar o docker ratts-server.
use **git clone** para clonar este repositorio. Após a clonagem, atualize as permições do arquivo **start** para executável com o comando **chmod +x start**. **(~$ sudo chmod+x ratts-server_docker-install/start)**

feito isso, entre na pasta **ratts-server_docker-install** e execute no terminal: **~$ratts-server_docker-install# sudo ./start**

agora ele vai baixar e executar a imagem.

* ao iniciar o container ratts-server, execute **/etc/init.d/apache2 start** para iniciar o servidor e depois, em sua maquina host (local) coloque o ip local ou ip publico da maquina anfitriã **(maquina host)** 192.188.0.1; 127.0.0.1; localhost...
* execute tambem o servidor mysql: **/etc/init.d/mysql start**


## Funções basicas

- Para sair da sua imagem e voltar para o host (desligando o server): **exit ou ctrl+d**
- para sair da sua imagem e voltar para o host (sem desligar o server) **ctrl + p + q**
- detalhes da imagem em execução: **sudo docker ps**
- voltar para a linha de comando do containner: **sudo docker attach id_da_imagem**
