Docker e Django
Este guia fornece instruções para a instalação e utilização de um projeto Django utilizando Docker. Siga os passos abaixo para configurar seu ambiente de desenvolvimento.

Pré-requisitos
Certifique-se de ter as seguintes ferramentas instaladas em sua máquina:

Python
Docker
Passo a Passo
1. Configurar o Ambiente Virtual
1.1. Verifique a instalação do Python:

bash
Copiar código
python3 --version
1.2. Crie e ative um ambiente virtual:

bash
Copiar código
python3 -m venv venv
source venv/bin/activate
Isso criará uma pasta chamada venv para o ambiente virtual e ativará o mesmo.

2. Construir a Imagem Docker
2.1. No diretório do projeto, execute o seguinte comando para construir a imagem Docker:

bash
Copiar código
docker build -t NomeDaImagem .
Isso criará uma imagem baseada no Dockerfile presente no projeto.

3. Executar o Container Docker
3.1. Execute o container utilizando a imagem criada anteriormente:

bash
Copiar código
docker run -d -p 8000:8000 --name django NomeDaImagem
Isso iniciará um container Docker com a imagem criada e mapeará a porta 8000 do container para a porta 8000 da sua máquina.

4. Acessar a Aplicação
4.1. Após seguir os passos acima, você poderá acessar a aplicação em:

arduino
Copiar código
http://localhost:8000
Você deverá ver a mensagem configurada nas URLs do projeto Django.
