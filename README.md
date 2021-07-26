# Desafio - Desenvolvedor Python

Parabens por ter chegado na etapa de teste técnico!

Estamos felizes com o seu interesse em fazer parte da qflash.

O teste técnico a seguir tem um prazo máximo de 7 dias pra ser concluído.

Ele precisa ser feito em Python e entregue num repositório Git, porém sinta-se livre pra usar as demais tecnologias e bibliotecas que você quiser.


## Teste

O teste é dividido em 3 partes, com graus de dificuldade variados.

Não tem problema se não conseguir fazer o teste todo, ainda nos mande o que conseguiu fazer para avaliarmos :).

##### Introdução 
Um pet shop possui um hotel para cachorros e gostaria de automatizar o seu processo de cadastro. 

Você foi contratado para fazer uma API para eles, e te deram o arquivo **"pets.csv"** com a tabela dos cachorros já cadastrados. 

(uma cópia da mesma tabela também está presente no arquivo **"database.db"** caso queira usar sqlite)

##### Parte 1
A primeira etapa é desenvolver algo semelhante a um CRUD, que permite ler, adicionar, modificar e deletar a tabela de pets.

Aqui vai uma sugestão de organização da API:
- PUT /pet
- POST /pet
- GET /pet/{petId}
- DELETE /pet/{petId}

##### Parte 2
Para identificar melhor os cachorros, o pet shop achou uma boa ideia adicionar uma opção para mandar a foto do pet no cadastro.

A segunda etapa consiste em desenvolver endpoints para armazenar e ler fotos com base no id do cachorro.

Sugestões de armazenamento: S3, arquivos na máquina local, tabela com blobs

Aqui vai uma sugestão de organização da API:


- POST /picture/{petId}
- GET /picture/{petId}.png

##### Parte 3
Para manter a permanência desses dados e facilitar futuras migrações, o pet shop resolveu implementar um endpoint que faz o dump desses dados.

A terceira etapa consiste em desenvolver um **ou mais** endpoints para fazer o dump de todos os dados do banco, incluindo as fotos.

Sugestão: envio de arquivos grandes com http streaming

Aqui vai uma sugestão de organização da API:
- POST /dump.sql

##### Bônus
Achariamos muito legal se você fizer alguma dessas coisas na sua solução:
- utilizar recursos da AWS (EC2,S3,RDS, etc)
- containerizar o projeto e providenciar dockerfile
- fazer testes unitários pras funções do código

---

Se tiver alguma dúvida por favor fale com a gente no email do processo seletivo.

Boa sorte!
