create database academia;
create table cadastro(
cd_matricula int auto_increment,
nome varchar (11),
rg varchar (11),
nascimento date,
dt_matricula date,
primary key (cd_matricula)
);


create table atividade( 
cd_atividade int auto_increment,
qntd_alunos decimal,
h_aula time,
d_aula date,
d_inicial date,
d_final date,
t_atividade varchar (11),
primary key (cd_atividade));


create table contato ( 
cd_contato int auto_increment,
telefone_fixo varchar (10),
celular varchar (11),
 PRIMARY KEY (cd_contato));

create table titulo ( 
id_titulo int auto_increment,
primary key (id_titulo));

create table instrutor (
cd_instrutor int auto_increment,
primary key (cd_instrutor));

alter table instrutor add column cd_matr_intrutor int,
add constraint fk_cd_matr_intrutor
foreign key (cd_matr_intrutor)
references cadastro (cd_matricula);

create table monitor (
cd_monitor int auto_increment,
primary key (cd_monitor));

create table endereco (
logradouro varchar (15),
num varchar (10),
cep varchar (6),
cidade varchar (11),
complemente varchar (15),
cd_endereco int auto_increment,
primary key (cd_endereco));

create table turma(
ausencia varchar (11));

alter table turma add column cd_turma int auto_increment,
add primary key (cd_turma);


alter table turma add column cd_tur_ativ int,
add constraint fk_cd_tur_ativ
foreign key (cd_matricula)
references cadastro (cd_matricula);


alter table contato add column cd_matricula int,
add constraint fk_cd_matricula
foreign key (cd_matricula)
references cadastro (cd_matricula);
