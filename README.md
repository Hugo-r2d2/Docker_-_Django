# Docker_-_Django

Para instalação e utilização do Projeto faça os seguintes passos:
 
 1. Verifique a instalação do python na sua máquina;
 2. Utilizando seu  terminal digite:
    - python3 -m venv venv

    - source venv/bin/activate
 
    - Isso criará uma pasta para utilização de um ambiente virtual no seu python e também ativará o mesmo
 
 4. Verifique a instalação do Docker na sua máquina;
 5. Digite o seguinte comando no terminal do diretório do projeto:
    - docker build -t NomeDaImagem .
      
    - Isso criará uma imagem com base no Dockerfile já encontrado no projeto
    
    - docker run -d -p 8000:8000 --name django NomeDaImagem
    
    - Isso criará um container no docker que utilizará a imagem feita anteriormente e também usará a porta 8000
    
  6. Feito tudo isso você poderá acessar "http://localhost:8000" e verá a mensagem que colocamos nas urls 
  
  
  
