                        Enriquecedor de planilhas

                            Descrição do projeto.

-> Automação que irá ler arquivos excel com CNPJs de empresas e irá buscar na API receita ws os dados faltantes da empresa. 


                        Pré-requisitos e instalação

Instalação da biblioteca openpyxl: Insira no seu terminal o comando pip install openpyxl.

                        Ferramentas e Bibliotecas Utilizadas

python 3.12.10: Linguagem que irá construir o script de automação.

receita ws: API que busca informações sobre empresas através de CNPJs.

link da documentação da API: https://developers.receitaws.com.br/?_gl=1*lngslr*_gcl_aw*R0NMLjE3ODI0MTM2NDEuQ2owS0NRandvX1BSQmhETkFSSXNBRWNWQUxWblNDN01oYTltSVBOSUhFTVZnT1pDSXpEUXF6ZndRQmdrQ1lVRlJmTGZKRHNNbTU5T2MwSWFBaERtRUFMd193Y0I.*_gcl_au*NDg1MzMwNjUuMTc4MjQxMzYzOQ..*_up*MQ..*_gs*MQ..&gclid=Cj0KCQjwo_PRBhDNARIsAEcVALVnSC7Mha9mIPNIHEMVgOZCIzDQqzfwQBgkCYUFRfLfJDsMm59Oc0IaAhDmEALw_wcB&gbraid=0AAAAADf89S9MqVKfYeVaqUoqi5AzUjvYZ#/operations/queryRFFree

openpyxl: Biblioteca do python que acessa e manipula planilhas. Vamos
utiliza-la para atualizar a planilha com as informaçoes faltantes. 

os: Biblioteca nativa do python que irá acessar as pastas e criar arquivos

requests: Biblioteca nativa que irá realizar as requisições a API

                            Funcionalidades do sistema

-> O sistema deverá receber o caminho da pasta que contém as planilhas.
Dessa forma, a automação não se limitara a apenas um arquivo, já que
o sistema ira percorrer uma pasta especifica.

-> O sistema devera avisar ao usuário caso algum cnpj não seja encontrado

-> Para garantir que o sistema não percorra arquivos de extensões diferentes, ele irá verificar a extensão antes de realizar a busca
na API.

-> Ele devera criar colunas com as informações que estão faltando.

-> O sistema deverá criar uma pasta que irá conter todas as planilhas
atualizadas.

-> A cada execução do sistema, ele devera criar um arquivo txt com uma
lista com os cnpjs nao encontrados.

                                Considerações sobre o sistema                              
-> O link de requisições da API é do tipo GET que realiza a consulta de dados.

-> Nesse projeto iremos utilizar a versão gratuita da API que aceita 3
consultas por minuto.

-> A versão pública não necessita de autenticação, ou seja, não é necessária a criação de uma chave de API.

-> No plano gratuito, só temos acesso a CNPJs já existentes no banco de dados, ou seja, diferente da conta comercial, a API não irá realizar
consultas em tempo real (busca em outras fontes até onde entendi).


                                Como utilizar o sistema
-> 1: Crie 2 pastas em seu gerenciador de arquivos: uma para planilhas que contém os CNPJs e outra para salvar as planilhas que foram atualizadas
com as informações encontradas

-> 2: Cole o caminho da pasta que contém as planilhas que SERÃO atualizadas
no campo de entrada de pastas que contém planilhas

-> 3: Cole o caminho da pasta que ira conter as planilhas ATUALIZADAS com
as informações no campo de entrada que contém a pasta de planilhas atualizadas.




