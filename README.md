# TRABALHO 2 DE LABORATÓRIO DE REDES

Esse trabalho foi desenvolvido na disciplina de Laboratório de Redes ministrada pelo Professor Alexandre Pereira do Carmo. Tem como objetivo desenvolver uma
aplicação distribuída para troca de mensagens em Máquinas Virtuais:

**prog_cliente.py:** Aplicação de acesso ao usuário. 

**prog2_servidor.py:** Um servidor para realizar o gerenciamento e controle das mensagens.

## PRÉ-REQUISITOS

Certifique-se de ter o Docker instalado em sua máquina. Todas as bibliotecas utilizadas e o Python3, estão em container. 

>**NOTA:** Devido a conexão, a ordem de "abertura" dos programas devem ser respeitada. Sendo ela a ordem: **.py e logo em seguidas o .py, sendo o ultimo aberto 
quantas vezes for necessario**

### prog2_servidor.py

O servidor tem como objetivo realizar o fluxo de mensagens entre os diversos prog_cliente.py.

Só deve executar ele e deixar em aberto em quanto estiver realizando a troca de mensagens.

para rodar a aplicação, execute o comando

sudo docker run --rm -it  --network=host clauberar/cliente:cliente python3 prog_cliente.py 

### prog_cliente.py

Ao iniciar o cliente, vai ser pedido o IP do servidor, e em seguida o Nome do usuário.

Com esses primeiros passos feitos, basta somente digitar a mensagem que vai ser enviado para todos os clientes conectados ao servidor.

Para sair, basta somente digitar "sair"

para rodar a aplicação, execute o comando

sudo docker run --rm -it  --network=host clauberar/server:server python3 prog2_servidor.py 

## CONSIDERAÇÕES
Esse programa foi realizado com todos os conhecimentos adquiridos na disciplina de Redes e com instruções de programas recebidos ao longo de toda a formação acadêmica.
