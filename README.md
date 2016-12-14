#Músicas Brasileiras
Trabalho desenvolvido durante a disciplina de BD do Curso Técnico de Informática do Ifes/Serra.

#Sumário

###1	COMPONENTES<br>
Juliana Rangel Roque<br>

###2	INTRODUÇÃO E MOTIVAÇAO<br>
Música Brasileira foi o projeto escolhido, dentre as outras possibilidades apresentadas em sala de aula, devido a música ser uma das formas de artes que está presente no cotidiano de muitas pessoas. Além disso é algo que possui várias vertentes e combina vários sons e ritmos por consequÊncia tem a possibilidade de agradar a um público maior. A escolha ocorreu devido ao deficit existente no Brasil de um sistema online confiável pelo qual as pessoas possam ter acesso as informações confiáveis e corretas a respeito da composição das músicas brasileiras e dos intérpretes das mesmas.<br>

###3	MINI-MUNDO<br>

Música Brasileira é um sistema de dados online pelo qual será possível ter acesso às informações verídicas sobre as músicas escritas, produzidas e gravadas no Brasil. Este sistema será alimentado e retroalimentado pelos usuários, tendo que ter a aprovação dos administradores do sistema. 
Um usuário pode ter cadastro padrão, cantor, compositor ou de instrumentista. Uma música poderá ser escrita por um ou alguns compositores além de poder ser gravada por um ou vários cantores. Os usuários podem pesquisar compositores, cantores, músicas, gêneros e letras aos quais desejam ler, ouvir ou ser direcionados ao link da música escolhida no YouTube. Os usuários se cadastram no sistema e tem como atributo chave o cpf. Os usuários escolhem um gênero musical favorito/principal, podem marcar músicas como favoritas e podem enviar músicas para o sistema, alimentando o banco de dados. As músicas possuem compositores, cantores e gêneros. <br>
 
###4	RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
[Mockup - Música Brasileira - Em PDF] (https://github.com/julianar2/Trabalho01/blob/master/Mockup%20-%20MusicaBasileira.pdf)


###5	MODELO CONCEITUAL<br>
    5.1 NOTACAO ENTIDADE RELACIONAMENTO
[Conceitual - Música Brasileira - Em JPG](https://github.com/julianar2/Trabalho01/blob/master/Conceitual-Trab-BD.jpg)

####5.1 Validação do Modelo Conceitual
   Grupo01 - EstÊvão Segatto e Mathues Lopes <br>
   Grupo02 - Kelvin Kelvin Lehrback e Vinicius Martins <br>

####5.2 DECISÕES DE PROJETO
a) CPF: em nosso projeto optamos por um campo chave, pois cada usário possui um número diferente.<br>
b) Nome: em nosso projeto optamos por um campo comum, exceto na tabela usuário que é um campo multivalorado pois o usuái pode ter nome completo, artistíco e apelido.<br> 
C) Sexo: em nosso projeto optamos por um campo comum, pois pode haver o mesmo sexo para mais de um usuário.<br>
d) Login: em nosso projeto optamos por um campo comum, pois o campo código é de mais fácil filtragem.<br>
e) Senha: em nosso projeto optamos por um campo comum, pois pode haver a mesma senha pra mais de um login.<br>
f) Tipo de Usuário: em nosso projeto optamos por um campo comum, pois pode haver o mesmo tipo de usuário pra mais de um usuário.<br>
g) Código: em nosso projeto optamos por um campo chave, por ser único.<br>
h) Endereço: em nosso projeto optamos por um campo composto, pois o endereço é composto por vários atributos.<br>
i) Link Youtube: em nosso projeto optamos por um campo comum, pois foi preferível o campo código como chave. Pois o campo Link Youtube direciona apenas o caminho da música no Youtube.<br


####5.3 DESCRIÇÃO DOS DADOS 
  
NOME: Tabela que armazena as informações relativas aos nomes de identificação que o usuário pode utilizar.<br>
    COD_Nome: Tabela que armazena as informações relativas <br>

TIPO DE ID: Tabela que armazena as informações relativas ao tipo de identificação que o usuário pode utilizar. <br>
USUARIO: Tabela que armazena as informações relativas ao usuário.<br>
TIPO DE USUÁRIO: Tabela que armazena as informações relativas aos tipos de usuários. <br>
MÚSICA: Tabela que armazena as informações relativas as música. <br>
GÊNERO: Tabela que armazena as informações relativas aos gêneros. <br>
CANTOR: Tabela que armazena as informações relativas aos cantores. <br>
COMPOSITOR: Tabela que armazena as informações relativas aos compositores. <br>
CONTATO: Tabela que armazena as informações relativas aos contatos. <br>
TIPO DE CONTATO: Tabela que armazena as informações relativas aos tipos de contatos. <br>
ENDEREÇO: Tabela que armazena as informações relativas aos endereços. <br>
RUA: Tabela que armazena as informações relativas às ruas. <br>
CEP: Tabela que armazena as informações relativas aos ceps. <br>
BAIRRO: Tabela que armazena as informações relativas aos bairros. <br>
CIDADE: Tabela que armazena as informações relativas <br>
ESTADO: Tabela que armazena as informações relativas aos estados. <br>
PAÍS: Tabela que armazena as informações relativas aos países. <br>



###6	MODELO LÓGICO<br>
[Lógico - Música Brasileira - Em JPG] (https://github.com/julianar2/Trabalho01/blob/master/Logico-Trab-BD.jpg)<br>

###7	MODELO FÍSICO<br>
[Física - Música Brasileira - Em SQL] (https://github.com/julianar2/Trabalho01/blob/master/Music.sql)<br>    
        
###8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
####8.1 DETALHAMENTO DAS INFORMAÇÕES
        Detalhamento sobre as informações e processo de obtenção ou geração dos dados.
        Referenciar todas as fontes referentes a :
        a) obtenção dos dados
        b) obtenção de códigos reutilizados
        c) fontes de estudo para desenvolvimento do projeto
        Materiais da Disciplina de Bando de Dados
        
####8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) inclusão das instruções para criação das tabelas e estruturas de amazenamento do BD
        b) inclusão das instruções de inserção dos dados nas referidas tabelas
        c) inclusão das instruções para execução de outros procedimentos necessários


        Entrega até este ponto em 01/11/2016
        
###9	TABELAS E PRINCIPAIS CONSULTAS<br>
OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>

####9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

/* Consulta de Dados presentes na Tabela Música */<br>
select * from MUSICA;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/01%20-%20Musica.png)<br>

/* Consulta de Dados presentes na Tabela Usuário */<br>
select * from USUARIO;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/02%20-%20Usuario.png)<br>

/* Consulta de Dados presentes na Tabela TipoDeUsuario */<br>
select * from TipoDeUsuario;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/03%20-%20Tipo%20de%20Usuario.png)<br>

/* Consulta de Dados presentes na Tabela Cantor */<br>
select * from CANTOR;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/04%20-%20Cantor.png)<br>

/* Consulta de Dados presentes na Tabela Compositor */<br>
select * from COMPOSITOR;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/05%20-%20Compositor.png)<br>

/* Consulta de Dados presentes na Tabela TipoContato */<br>
select * from TipoContato;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/06%20-%20Tipo%20de%20Contato.png)<br>

/* Consulta de Dados presentes na Tabela Contato */<br>
select * from Contato;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/07%20-%20Contato.png)<br>

/* Consulta de Dados presentes na Tabela Gênero */<br>
select * from GENERO;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/08%20-%20Genero.png)<br>

/* Consulta de Dados presentes na Tabela Estado */<br>
select * from ESTADO;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/09%20-%20Estado.png)<br>

/* Consulta de Dados presentes na Tabela País */<br>
select * from PAIS;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/10%20-%20Pais.png)<br>

/* Consulta de Dados presentes na Tabela CEP */<br>
select * from CEP;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/11%20-%20Cep.png)<br>

/* Consulta de Dados presentes na Tabela Bairro */<br>
select * from BAIRRO;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/12%20-%20Bairro.png)<br>

/* Consulta de Dados presentes na Tabela Cidade */<br>
select * from CIDADE;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/13%20-%20Cidade.png)<br>

/* Consulta de Dados presentes na Tabela Rua */<br>
select * from Rua;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/14%20-%20Rua.png)<br>

/* Consulta de Dados presentes na Tabela Endereço */<br>
select * from ENDERECO;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/15%20-%20Endereco.png)<br>

/* Consulta de Dados presentes na Tabela Nome */<br>
select * from Nome;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/16%20-%20Nome.png)<br>

/* Consulta de Dados presentes na Tabela Favorita */<br>
select * from FAVORITA;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/17%20-%20Favorita.png)<br>

/* Consulta de Dados presentes na Tabela Envia */<br>
select * from ENVIA;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/18%20-%20Envia.png)<br>

/* Consulta de Dados presentes na Tabela Possui */<br>
select * from POSSUI;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/19%20-%20Possui.png)<br>

/* Consulta de Dados presentes na Tabela Pertence */<br>
select * from PERTENCE;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/20%20-%20Pertence.png)<br>

/* Consulta de Dados presentes na Tabela Interpretada */<br>
select * from INTERPRETADA;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/21%20-%20Interpretada.png)<br>

/* Consulta de Dados presentes na Tabela COMPOSTA */<br>
select * from COMPOSTA;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/22%20-%20Composta.png)<br>

/* Consulta de Dados presentes na Tabela Contem */<br>
select * from CONTEM;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/23%20-%20Contem.png)<br>

####9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 3) <br>

/*CONSULTAS DAS TABELAS COM FILTROS WHERE*/<br>
select * from usuario where sexo = 'feminino';<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/24%20-%20Consulta%201.png)<br>
select * from nome where apelido is not null;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/24%20-%20Consulta%202.png)<br>
select * from contato where descricaocontato = 'facebook'; <br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/24%20-%20Consulta%203.png)<br>
select * from contato where cod_tipo = 4;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/24%20-%20Consulta%204.png)<br>
select * from envia where cod_usuario = 2;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/24%20-%20Consulta%205.png)<br>

####9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E CAMPOS RENOMEADOS (Mínimo 2)<br>

/*CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E CAMPOS RENOMEADOS*/<br>
select * from endereco where COD_pais = 2 and COD_estado = 7;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/25%20-%20Consulta%201.png)<br>
select * from interpretada where Gravacao > "01-02-2012";<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/25%20-%20Consulta%202.png)<br>
select * from endereco where cod_pais = 5 or COD_estado = 1;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/25%20-%20Consulta%203.png)<br>
select LinkYoutube from musica where Titulo ='Refém';<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/25%20-%20Consulta%204.png)<br>
select CPF from usuario where COD_Genero = 1;<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/25%20-%20Consulta%205.png)<br>

####9.4	CONSULTAS QUE USAM OPERADORES LIKE (Mínimo 3)  <br>
/*CONSULTAS QUE USAM OPERADORES LIKE*/<br>
select * from nome where nomecompleto like 'j%';<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/26%20-%20Consulta%201.png)<br>
select * from nome where nomecompleto like '%amaro%';<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/26%20-%20Consulta%202.png)<br>
select * from nome where nomecompleto like '%amaro%' and apelido = 'gringo';<br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/26%20-%20Consulta%203.png)<br>
select * from rua where cep like '29%';,br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/26%20-%20Consulta%204.png)<br>

####9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

/*ATUALIZAÇÃO E EXCLUSÃO DE DADOS*/<br>
update nome set apelido = 'Lu' where nome_pk = 1;<br>
update nome set NomeArtistico = 'Luemily' where apelido = 'Lu';<br>
update nome set NomeArtistico = 'Juliana Roque' where COD_Usuario_FK = 2;<br>
update nome set NomeArtistico = 'Luiz Picolé' where COD_Usuario_FK = 3;<br>
update nome set nomecompleto = 'Luiz Claudio Picolé' where COD_Usuario_FK = 3;<br>
select * from nome; ,br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/27%20-%20Consulta%201.png)<br>
delete from nome where nome_pk = 1;<br>
select * from nome; <br>
[Alt text](https://github.com/julianar2/Trabalho01/blob/master/27%20-%20Consulta%202.png)<br>


####9.6	CONSULTAS COM JUNÇÃO (Todas Junções)<br>
select NomeCompleto, nomeArtistico, COD_Usuario, COD_Usuario_FK from usuario inner join nome on (usuario.COD_Usuario = nome.COD_Usuario_FK);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select1.PNG)<br>

select cod_tipo as "cod_tipo_FK" from contato ;

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select2.PNG)<br>

select DescricaoContato, contato.COD_Tipo from contato inner join tipocontato on (contato.COD_Tipo = tipocontato.COD_Tipo);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select3.PNG)<br>

select Login, Titulo, musica.COD_Musica, usuario.COD_Usuario from favorita inner join usuario on(FAVORITA.COD_Usuario = usuario.COD_Usuario) inner join musica on(favorita.COD_Musica = musica.COD_Musica);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select4.PNG)<br>

select Login, dataDeEnvio, musica.COD_Musica, usuario.COD_Usuario from envia inner join usuario on(envia.COD_Usuario = usuario.COD_Usuario) inner join musica on(envia.COD_Musica = musica.COD_Musica);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select5.PNG)<br>

select Login, NomeDoGenero from usuario inner join genero on(usuario.COD_Genero = genero.COD_Genero); 

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select6.PNG)<br>

select Titulo, genero.COD_Genero, musica.COD_Musica from pertence inner join genero on(pertence.COD_Genero = genero.COD_Genero) inner join musica on(pertence.COD_Musica = musica.COD_Musica);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select7.PNG)<br>

select Titulo, NomeCantor, gravacao, musica.COD_Musica, cantor.COD_cantor from interpretada inner join cantor on(cantor.COD_cantor = interpretada.COD_Cantor) inner join musica on(interpretada.COD_Musica = musica.COD_Musica);

[Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/select8.PNG)<br>

####9.7	CONSULTAS COM GROUP BY (Mínimo 5)<br>


        Entrega até este ponto em 08/11/2016
        
####9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4) <br>
####9.9	CONSULTAS COM SELF JOIN (todas) E VIEW (mais importantes) <br>
####9.10	SUBCONSULTAS (Mínimo 3) <br>


###10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES<br>


###11	DIFICULDADES ENCONTRADAS PELO GRUPO<br>
A principal dificuldade é ter um entendimento total do modelo conceitual e ir caminhando com ele de acordo com as necessidade que vão surgindo no decorrer do processo.
Na utilização do MySql é que conseguir enxergar e acertar os erros cometidos (seja de digitação, lógica) <br> 

        Entrega final em 22/11/2016
###12  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
