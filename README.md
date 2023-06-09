# API CORES
A API serve para gerenciar um banco de dados de cores, que pode ser fácilmente acessado e alterado, por meio da interface implementada na pasta ***Frontend***.

## Instalação

Para rodar esse projeto você vai precisar ter o Node JS, MySQL e o MySQL Workbench instalados.

Use os seguintes comando no MySQL Workbench:

`create database dbApiColors;`
`use dbApiColors;`
`create table colors(
	pKey int primary key auto_increment,
    hexCode varchar(6),
    colorName varchar(30)
);`
`insert into colors(hexCode, colorName) values ('000000', 'Preto');`
`insert into colors(hexCode, colorName) values ('18BBF7', 'Azul Zima');`
`insert into colors(hexCode, colorName) values ('9b59b6', 'Ametista');`
`insert into colors(hexCode, colorName) values ('e67e22', 'Cenoura');`

Depois disso você vai ter o banco de dados `dbApiColors` criado e populado com quatro cores.

Agora abra a pasta ***Backend*** no prompt, digite `npm i`, depois que a instalação for concluída, digite `npm start`, isso vai fazer com que o Backend comece a rodar e se conecte com o banco de dados.

O último passo é abrir o arquivo `index.html` na pasta Frontend, depois disso você vai poder utilizar livremente.

## Como usar
- Para criar uma nova cor você deve inserir o Nome da cor, e o código HEX, sem # no início, depois é só clicar no botão *Nova cor*. 

- Se quiser alterar alguma cor que já foi criada, você precisa inserir a chave primaria da mesma, que vai estar visível no canto superior esquerdo do quadrado da cor em questão e clicar no botão *Alterar cor*.

- Quando precisar apagar uma cor existente, você só precisa preencher o campo *Chave Primária* e clicar no boão *Deletar cor*.

- Também é possível copiar o código HEX de uma cor existente, clicando sobre o quadrado que representa a mesma.