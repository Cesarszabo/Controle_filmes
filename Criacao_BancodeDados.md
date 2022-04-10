#Esses foram os comandos usados para criação do Banco de Dados


create database movies_control;


create table movies(
id INT Primary Key IDENTITY(1,1),
type INT NOT NULL,
nome VARCHAR(30) NOT NULL,
total_ep INT,
atual_ep INT,
last_view DATE DEFAULT getdate()
)

tipo > 0- series e 1-filmes

INSERT INTO movies (type, nome, total_ep, atual_ep) VALUES (0, 'Lupin', 20,2), (1,'Spider Man',NULL,NULL)

INSERT INTO movies (type, nome, total_ep, atual_ep) VALUES (0, 'Brooklyn 99', 20,2), (1,'Sonic',NULL,NULL), (1,'The Davinci code',null,null),(0,'Friends',30,5)  

Update movies set last_view ='2022-02-09' WHERE id=1



SELECT * FROM movies