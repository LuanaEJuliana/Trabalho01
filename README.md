# TRABALHO 01
Trabalho desenvolvido durante a disciplina de BD

#Sumário

###1	COMPONENTES<br>
Luana Emiliano Ferreira e Juliana Rangel Roque<br>

###2	INTRODUÇÃO E MOTIVAÇAO<br>
Este projeto foi escolhido com o intuito de centralizar as músicas brasileiras e deixar acessível os nomes dos compositores de suas respectivas músicas. O projeto chama-se Músicas Brasileiras. Para ter acesso ao sistema os usuários se cadastram, e os dados solicitados são: cpf, e-mail, senha, contatos, endereço, gênero musical favorito/principal, data de nascimento, tipo de usuário, podendo ser usuário padrão, músico instrumentista, cantor ou compositor; e sexo.  <br>

###3	MINI-MUNDO<br>
No sistema Músicas Brasileiras os usuários podem pesquisar compositores, cantores, músicas, gêneros e letras aos quais desejam ler, ouvir ou serdirecionados ao link da música escolhida no YouTube. Os usuários se cadastram no sistema e tem como atributo chave o cpf. Os usuários escolhem um gênero musical favorito/principal, podem marcar músicas como favoritas e podem enviar músicas para o sistema, alimentando o banco de dados. As músicas possuem compositores, cantores e gêneros. <br>

###4	RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
neste ponto a codificação não e necessária, somente as ideias de telas devem ser criadas, o princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/1.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/2.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/3.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/4.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/5.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/6.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/7.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/8.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/9.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/10.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/11.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/12.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/13.png?raw=true "Title")
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/14.png?raw=true "Title")


###5	MODELO CONCEITUAL<br>
    5.1 NOTACAO ENTIDADE RELACIONAMENTO
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/conceitual%20imagem%203.jpg?raw=true "Modelo Conceitual")
    
    5.2 NOTACAO UML (Caso esteja fazendo a disciplina de analise)

####5.1 Validação do Modelo Conceitual
    [Grupo01]: Mathues Lopes e Estêvão Segatto
    [Grupo02]: Kelvin Lehrback e Vinicius Martins

####5.2 DECISÕES DE PROJETO   
    a) Campo endereço: em nosso projeto optamos por um campo multivalorado e composto, pois a empresa 
    pode possuir para cada departamento mais de uma localização... 
    b) justifique!
    a) CPF: em nosso projeto optamos por um campo chave, pois cada usário possui um número diferente.<br>
    b) Nome: em nosso projeto optamos por um campo comum, exceto na tabela usuário que é um campo multivalorado pois o usuái pode ter nome completo, artistíco e apelido.<br> 
    C) Sexo: em nosso projeto optamos por um campo comum, pois pode haver o mesmo sexo para mais de um usuário.<br>
    d) Login: em nosso projeto optamos por um campo comum, pois o campo código é de mais fácil filtragem.<br>
    e) Senha: em nosso projeto optamos por um campo comum, pois pode haver a mesma senha pra mais de um login.<br>
    f) Tipo de Usuário: em nosso projeto optamos por um campo comum, pois pode haver o mesmo tipo de usuário pra mais de um usuário.<br>
    g) Código: em nosso projeto optamos por um campo chave, por ser único.<br>
    h) Endereço: em nosso projeto optamos por um campo composto, pois o endereço é composto por vários atributos.<br>
    i) Link Youtube: em nosso projeto optamos por um campo comum, pois foi preferível o campo código como chave. Pois o campo Link Youtube direciona apenas o caminho da música no Youtube.<br>


####5.3 DESCRIÇÃO DOS DADOS     
    USUÁRIO: Tabela que armazena as informações relativas aos usuários.<br>
        CPF: campo que armazena o número de Cadastro de Pessoa Física para cada cliente da empresa.<br>
        Nome:campo que armazena o nome completo, nome artísitco e/ou apelido do usuário.<br>
        Contato:campo que armazena os contatos e os tipos de contatos de cada usuário.<br>
        Sexo:campo que armazena o sexo do usuário.<br>
        Login:campo que armazena o login do usuário.<br>
        Senha:campo que armazena a senha do usuário.<br>
        Tipo de Usuário:campo que armazena o tipo do usuário.<br>
        Código da Música:campo que armazena o código da música enviada pelo usuário.<br>
        Endereço:campo que armazena as informações completa do endereço do usuário.<br>
    MÚSICA: Tabela que armazena as informações relativas as músicas.<br>
        Código da Música:campo que armazena o código da música.<br>
        Nome da Música:campo que armazena o nome da música.<br>
        Link Youtube:campo que armazena o link do Youtube.<br>
    CANTOR:Tabela que armazena as informações relativas aos cantores.<br>
        Código do Cantor:campo que armazena o código do cantor.<br>
        Nome do Cantor:campo que armazena o nome do cantor.<br>
    COMPOSITOR:Tabela que armazena as informações relativas aos compositores.<br>
        Código do Compositor:campo que armazena o código do compositor.<br>
        Nome do Compositor:campo que armazena o nome do compositor.<br>
    GÊNERO:Tabela que armazena as informações relativas aos gêneros.<br>
        Código do gênero:campo que armazena o código do gênero.<br>
        Nome do Compositor:campo que armazena o nome do gênero.<br>



###6	MODELO LÓGICO<br>
![Alt text](https://github.com/LuanaEJuliana/Trabalho01/blob/master/l%C3%B3gico%202.jpg?raw=true "Modelo Lógico")

###7	MODELO FÍSICO<br>
###8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
####8.1 DETALHAMENTO DAS INFORMAÇÕES
        Detalhamento sobre as informações e processo de obtenção ou geração dos dados.
        Referenciar todas as fontes referentes a :
        a) obtenção dos dados
        b) obtenção de códigos reutilizados
        c) fontes de estudo para desenvolvimento do projeto
        
####8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) inclusão das instruções para criação das tabelas e estruturas de amazenamento do BD
        b) inclusão das instruções de inserção dos dados nas referidas tabelas
        c) inclusão das instruções para execução de outros procedimentos necessários

###9	TABELAS E PRINCIPAIS CONSULTAS<br>
####9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS<br>
####9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE<br>
####9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E CAMPOS RENOMEADOS<br>
####9.4	CONSULTAS QUE USAM OPERADORES LIKE<br>
####9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS<br>
####9.6	CONSULTAS COM JUNÇÃO<br>
####9.7	CONSULTAS COM GROUP BY<br>
####9.8	CONSULTAS COM LEFT E RIGHT JOIN<br>
####9.9	CONSULTAS COM SELF JOIN E VIEW<br>
####9.10	SUBCONSULTAS<br>
###10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES<br>
###11	DIFICULDADES ENCONTRADAS PELO GRUPO<br>
###12  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/




