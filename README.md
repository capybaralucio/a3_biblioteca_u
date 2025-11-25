#sistema de biblioteca universitaria aplicada em Python, estruturada padrão arquitetura MVC, orientacao a objetos com banco de dados PostgreSQL

estrutura do pgadmin:
create table autor(
id serial primary key,
nome varchar(100) not null,
nacionalidade varchar(50)
);

create table livro(
id serial primary key,
titulo varchar(200) not null,
ano_publicacao int,
id_autor integer not null,
id_autor int references autor(id)
);