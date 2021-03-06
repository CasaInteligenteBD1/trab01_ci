# TRABALHO 01:  JARVIS - CASA INTELIGENTE
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1 COMPONENTES <br>

<b> Integrantes do grupo (Casa Inteligente -> Estaciona): </b> <br>

Andreângelo Patuzzo: andreangelo.pp@gmail.com <br>
Anne Caroline Silva: carolinesilva4@gmail.com <br>
Caicke Carvalho de Pinheiro: caicke@gmail.com <br>
Emanuel Rampinelli: emanuel_rampinelli@hotmail.com <br>

<b> Integrantes do grupo 2 (EasyMarket -> Casa Inteligente): </b> <br>

Rafaela Amorim Pessin: rafaelapessin@outlook.com <br>

### 2 INTRODUÇÃO E MOTIVAÇÃO <br>

<p align = "justify"> Com a evolução dos computadores e das conexões de rede sem fio foi possível o advento da Internet das Coisas (IoT - Internet of Things), possibilitando a comunicação de equipamentos eletrônicos com a internet e entre si. O IoT é base para o desenvolvimento de casas inteligentes, onde as pessoas podem, por exemplo, gerenciar equipamentos que estão em suas casas através da internet e reconhecer padrões, trazendo então, formas de facilitar e agilizar suas vidas. </p>

<p align = "justify"> Imaginando dois irmãos gêmeos idênticos, mesmo sendo iguais em aparência, eles passam por experiências diferentes durante a vida, o que influencia, por exemplo, que tenham uma visão de mundo distinta devido às diferentes informações que guardaram. Pode-se fazer uma analogia a isso quando se pensa em casas inteligentes, na qual casas idênticas e com o mesmo sistema de IoT, mas com pessoas diferentes habitando nelas, guardam informações particulares a elas devido às diferentes rotinas e hábitos de seus moradores. Logo, a partir dos bancos de dados que armazenam a usabilidade de cada uma das casas, extrai-se informações e padrões diferentes. </p>

<p align = "justify"> Um ambiente automatizado, mais conhecido como Casa Inteligente, necessita de uma tecnologia de apoio. JARVIS é um sistema mobile que auxilia no controle de alguns eletroeletrônicos, equipamentos e outros itens disponíveis em ambientes (familiares e/ou empresariais) que dispõem de projetos de automação residencial. O sistema irá atuar diretamente no dia a dia do usuário, proporcionando a ele praticidade, conforto e até mesmo segurança. </p>

### 3 MINI-MUNDO

<p align = "justify"> O cliente deseja um sistema para controle de ambientes residenciais e/ou empresariais, com projetos de automatização. Para um projeto inicial, o sistema JARVIS está disponível para os seguintes eletroeletrônicos: ar-condicionado, computador, lâmpadas, televisão, geladeira, máquina de lavar roupas, microondas, fogão, chuveiro, forno elétrico e ventilador. O sistema JARVIS está restrito a controlar apenas as funções “liga e desliga” desses equipamentos, permitindo às pessoas que, através de um botão, consigam ligá-los e desligá-los. Dos eletroeletrônicos (equipamentos) é desejável saber o nome, a potencia, o status (ligado ou desligado), a hora e o dia que foi ligado e a hora e o dia que foi desligado. </p>

<p align = "justify"> JARVIS oferece uma tecnologia de sistema integrado capaz de controlar remotamente todos os cômodos de um ambiente utilizando um dispositivo mobile. O aplicativo pode ser utilizado em qualquer local que possua projetos de automatização e que contenha equipamentos os quais o aplicativo atende. Para o funcionamento dos eletroeletrônicos junto ao aplicativo é necessário conexão Wi-Fi, para que os sensores dos eletrônicos sejam pareados com o aplicativo. </p>

<p align = "justify"> Para obter o aplicativo é necessário comprá-lo pelo site de publicidade do JARVIS.  Através do site é possível realizar um cadastro e contratar o sistema. Ao realizar o cadastro, é necessário optar por pagar via boleto bancário, cartão de crédito ou débito. Ao final do seu cadastro, o comprador poderá acessar o sistema sem que haja necessidade de realizar um novo cadastro via aplicativo. O comprador se tornará o Titular pois será o usuário principal do sistema e será responsável por cadastrar locais (casas, empresas, escritórios, lojas, entre outros) no aplicativo, e gerenciá-los. </p>

<p align = "justify"> O Titular pode ser, por exemplo, um morador de uma residência ou um gerente de uma empresa que é responsável por cadastrar, respectivamente, outros moradores da casa ou os funcionários da empresa como pessoas que não podem gerenciar o local, mas podem ou não controlar os eletroeletrônicos de acordo com as permissões dadas a eles, e também podem fazer o monitoramento do consumo de energia (damos a eles o nome de Dependentes). O Titular possui o controle sobre todos os locais cadastrados e todos os elementos do local. Ele pode cadastrar no máximo seis locais no aplicativo. Além de poder cadastrar locais e usuários referentes a eles, ele também pode adicionar os cômodos para cada local cadastrado, adicionar os eletroeletrônicos e equipamentos dos cômodos,  e monitorar o consumo de energia de cada local por período selecionado obtendo uma estimativa de valor para aquele período. </p>

<p align = "justify"> A pessoa que possui a conta de Titular dispõe da possibilidade de colocar restrições em relação à utilização dos eletroeletrônicos pelas outras pessoas que utilizam o aplicativo. O Titular possui controle total sobre o(s) ambiente(s). Logo, ele possui controle sobre todos os equipamentos de todos os locais cadastrados, podendo ligá-los e desligá-los a qualquer momento. Porém, ele pode querer colocar algumas restrições de acesso para as outras pessoas, escolhendo qual tipo de acesso cada pessoa pode ter para cada equipamento de cada cômodo. Dessa forma, uma criança, por exemplo, pode ter acesso a uma lâmpada ou ao computador de um cômodo,mas pode não ter acesso para controlar um fogão. </p>

<p align = "justify"> Da pessoa (Titular ou Dependente) é desejável saber o nome, a data de nascimento, o email e o endereço. Do local é desejável saber o nome. Do cômodo é desejável saber o nome. Do eletroeletrônico é desejável saber o nome, a potência, o status, a hora e o dia que foi ligado e a hora e o dia que foi desligado. Do nível de permissão é necessário saber uma descrição sobre o que é permitido em cada nível. </p>

<p align = "justify"> O aplicativo deve notificar os usuários quando algum eletroeletrônico estiver inacessível e os equipamentos devem possuir uma forma de desligamento manual a fim de garantir uma maior segurança. A cobrança será mensal e o valor da cota de cobrança será proporcional ao número de usuários cadastrados em cada conta, pelo tempo que o cliente estiver utilizando o  aplicativo. </p>

<p align = "justify"> <b> REGRAS DE NEGÓCIO: </b> </p>

<br align = "justify"> <b> RN01: </b> A cobrança pela utilização do aplicativo será realizada mensalmente.
<br align = "justify"> <b> RN02: </b> O valor da cota de cobrança será proporcional ao número de usuários do aplicativo em cada conta. O cálculo mensal será com base na seguinte expressão: Valor Mensal = Número de Usuários x Valor por Usuário.
<br align = "justify"> <b> RN03: </b> O sistema deve ter um único Usuário Titular.
<br align = "justify"> <b> RN04: </b> Todo eletroeletrônico atendido pelo aplicativo precisa ser cadastrado para que seja controlado.
<br align = "justify"> <b> RN05: </b> O Titular pode adicionar restrições quanto à utilização dos eletroeletrônicos por parte dos Dependentes. Isso é feito da seguinte forma: para cada Dependente, é alocada uma permissão diferente a cada eletroeletrônico.
<br align = "justify"> <b> RN06: </b> O relatório de consumo de energia deve gerar uma estimativa de consumo de acordo com o período selecionado pelo usuário.
<br align = "justify"> <b> RN07: </b> A estimativa de consumo gerada no relatório de consumo de energia refere-se à três informações: ao gasto de energia por eletroeletrônico dentre todos presentes no local em KWh, ao gasto total de energia em KWh (soma dos gastos de cada equipamento) e à estimativa de valor gasto naquele período.
<br align = "justify"> <b> RN08: </b> Deve ser possível cadastrar no máximo seis locais/ambientes.
<br align = "justify"> <b> RN09: </b> Apenas pessoas com idade maior ou igual a 18 anos podem contratar o sistema.
<br align = "justify"> <b> RN10: </b> Para contratar o sistema é necessário realizar um cadastro pelo site do JARVIS, a partir do qual é possível acessá-lo sem a necessidade de um novo cadastro pelo aplicativo.
<br align = "justify"> <b> RN11: </b> Após realizar o cadastro no site de publicidade do JARVIS, o aplicativo somente será liberado para uso após confirmação do pagamento.
<br align = "justify"> <b> RN12: </b> Para adquirir o sistema é preciso realizar um cadastro no site de publididade do JARVIS, sendo necessário selecionar a forma de pagamento. O pagamento mensal pelo contrato do sistema pode ser realizado por boleto bancário, cartão de crédito ou débito.
<br align = "justify"> <b> RN13: </b> Clientes em atraso têm até 15 dias para realizar o pagamento. Após esse período, o aplicativo será desativado para uso.
<br align = "justify"> <b> RN14: </b> Somente é possível cadastrar cômodos se um local já estiver cadastrado. Da mesma forma, somente é possível cadastrar moradores e eletroeletrônicos se os cômodos estiverem cadastrados.
<br align = "justify"> <b> RN15: </b> O sistema deve manter o histórico de consumo de energia. Portanto, é possível selecionar um período passado.
<br align = "justify"> <b> RN16: </b> O acesso à funções de cadastro deve ser gerenciado pelo nível de permissão.
<br align = "justify"> <b> RN17: </b> O sistema deve controlar o acesso às funcionalidades. Funcionalidades de cadastro de locais, moradores, cômodos e eletroeletrônicos, estão restritas à pessoa com conta Titular. A pessoa com conta comum possui restrições.

### 4 RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)

[Propótipos - JARVIS - Casa Inteligente](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Proto%CC%81tipos%20JARVIS.pdf)

#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    
<p align = "justify"> O sistema JARVIS precisa inicialmente dos seguintes relatórios: </p>

<p align = "justify"> - Relatório dos locais cadastrados em cada conta de Usuário Master, incluindo as seguintes informações: nome do local, nome do Usuário Master, país, estado, município, bairro, logradouro, número e CEP. </p>

<p align = "justify"> - Relatório que informe os dados relacionados às pessoas de cada local e sua relação de acesso aos eletroeletrônicos, incluindo as seguintes informações: nome da pessoa, idade, e-mail, nome do eletroeletrônico, tipo do eletroeletrônico, cômodo em que está o eletroeletrônico e nível de acesso por eletroeletrônico. </p>

<p align = "justify"> - Relatório que informe os eletroetrônicos de um local, incluindo as seguintes informações: nome do eletroeletrônico, local onde está o eletroeletrônico, cômodo em que está o eletroeletrônico, tipo de eletroeletrônico. </p>

<p align = "justify">  - Relatório que informe o periodo do mês de maior utilização de eletroeletrônicos: nome do eletroeletrônico, status do eletroeletrônico, datas de interval, horas de intervalo. </p>

<p align = "justify"> - Relatório do consumo de energia dos locais/ambientes cadastrados, incluindo as seguintes informações: nome do local, nome do eletroeletrônico, potência do eletroeletrônico, consumo em KWh por eletroeletrônico, consumo total em KWh, consumo total em reais (R$) e datas de intervalo. </p>
    
#### 4.2 TABELA DE DADOS DO SISTEMA:
    
[Tabela de Atributos e Registros - Casa Inteligente - JARVIS](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Tabela%20de%20Atributos%20e%20Registros%20-%20Casa%20Inteligente%20-%20Jarvis%20(Junta).xlsx)
    
>## Marco de Entrega 01 em: (02/04/2018)<br>

### 5. MODELO CONCEITUAL<br>

    Modelo Conceitual

![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Modelo%20Conceitual%20-%20JARVIS.png "Modelo Conceitual - Casa Inteligente - JARVIS")

    Notação UML

![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Diagrama%20de%20Classes.png "Notação UML - Casa Inteligente - JARVIS")

#### 5.1 Validação do Modelo Conceitual
    
    Estaciona: Andreângelo, Emanuel, Caicke e Anne Caroline
    Super Market: Antônio, Jennifer, Joel e Larissa

#### 5.2 DECISÕES DE PROJETO
    
•	Foi normalizado o endereço para padronizar os dados, evitando o armazenamento de vários dados  que representem a mesma coisa. <br>
•	Optou-se por não criar uma entidade sensor já que, para o projeto inicial, existe apenas um tipo de sensor para todos os eletroeletrônicos. <br>
•	Foi criada a entidade DATA_USO para que estabelecesse uma relação de utilização do eletroeletrônico em uma determinada data sem que houvesse o armazenamento de muitas datas repetidas. Sem essa tabela, o número de dados redundantes seria muito grande. Se um eletroeletrônico fosse ligado e desligado dez vezes em um mesmo dia, iria armazenar a mesma data dez vezes. <br>
•	Apesar de existirem apenas dois níveis de acesso aos eletroeletrônicos no projeto inicial, optou-se por criar a entidade NIVEL_ACESSO, pensando na possibilidade de existirem mais níveis de permissão com o desenvolvimento do projeto. <br>

<b> Em relação aos tipos dos atributos de cada tabela: </b> <br>

<b> ENTIDADE PESSOA: </b> É uma entidade forte, pois não necessita de outra entidade para existir. <br>

•	id_pessoa: É um atributo chave que irá identificar de forma única a entidade PESSOA, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É um atributo simples (atômico) pois recebe um único valor, já que um morador só possui um único nome. <br>
•	data_nasc: É um atributo simples (atômico) pois recebe um único valor, já que um morador possui apenas uma data de nascimento. <br>
•	login: É um atributo simples (atômico) pois recebe um único valor, ou seja, é possível que a pessoa tenha apenas um login para acesso ao sistema. <br>
•	senha: É um atributo simples (atômico) pois recebe um único valor, ou seja, é possível que a pessoa tenha apenas uma senha para acessar o sistema. <br>
•	email: É um atributo simples (atômico) pois recebe um único valor, já que optamos pelo cadastro de apenas uma conta de e-mail por usuário. <br>

<b> ENTIDADE LOCAL: </b> É uma entidade forte, pois não necessita de outra entidade para existir. <br>

•	id_local: É um atributo chave que irá identificar de forma única a entidade LOCAL, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É um atributo simples (atômico) pois recebe um único valor, já que um local cadastrado recebe apenas um único nome. <br>

<b> ENTIDADE ENDERECO: </b> <br>

•	id_endereco: É um atributo chave que irá identificar de forma única a entidade ENDERECO, e por esse motivo será a chave primária no banco de dados. <br>
•	cep: É um atributo simples (atômico) pois recebe um único valor, já que um endereço cadastrado tem apenas um único CEP. <br>
•	logradouro: É um atributo simples (atômico) pois recebe um único valor, já que um endereço cadastrado tem apenas um único logradouro. <br>
•	numero: É um atributo simples (atômico) pois recebe um único valor, já que um endereço cadastrado recebe apenas um único número referente ao logradouro. <br>

<b> ENTIDADE BAIRRO: </b> <br>

•	id_bairro: É um atributo chave que irá identificar de forma única a entidade BAIRRO, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É um atributo simples (atômico) pois recebe um único valor, já que um bairro cadastrado recebe apenas um único nome. <br>

<b> ENTIDADE MUNICIPIO: </b> <br>

•	id_municipio: É um atributo chave que irá identificar de forma única a entidade MUNICIPIO, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É um atributo simples (atômico) pois recebe um único valor, já que um município cadastrado recebe apenas um único nome. <br>

<b> ENTIDADE ESTADO: </b> <br>

•	id_estado: É um atributo chave que irá identificar de forma única a entidade ESTADO, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É um atributo simples (atômico) pois recebe um único valor, já que um estado cadastrado recebe apenas um único nome. <br>

<b> ENTIDADE COMODO: </b> É uma entidade fraca, pois necessita da entidade LOCAL para existir. Sem um local, um cômodo não existe. <br>

•	id_comodo: É um atributo chave que irá identificar de forma única a entidade COMODO, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É atributo simples (atômico) pois recebe um único valor, já que cada cômodo do local só pode receber apenas um nome. <br>

<b> ENTIDADE ELETROELETRONICO: </b> É uma entidade forte, pois não necessita de outra entidade para existir. <br>

•	id_eletro: É um atributo chave que irá identificar de forma única a entidade ELETROELETRONICO, e por esse motivo será a chave primária no banco de dados. <br>
•	nome: É atributo simples (atômico) pois recebe um único valor, pois um eletreletrônico possui apenas um nome. <br>
•	status: É atributo simples (atômico) pois recebe um único valor, pois um eletreletrônico so pode estar ligado ou desligado em um determinado momento. <br>
•	hora: É atributo simples (atômico) pois recebe um único valor. <br>
•	potencia: É atributo simples (atômico) pois recebe um único valor, pois um eletreletrônico possui apenas uma potência (em Watts). <br>

<b> ENTIDADE DATA_USO: </b> <br>

•	id_data: É um atributo chave que irá identificar de forma única a entidade DATA_USO, e por esse motivo será a chave primária no banco de dados. <br>
•	data_uso: É um atributo simples (atômico) utilizado para armazenar várias datas diferentes dentro de uma tabela de datas. <br>

<b> ENTIDADE UTILIZACAO_ELETRO: </b> É uma entidade associativa, devido à necessidade de associar esta entidade ao relacionamento Utiliza. <br>

•	id_utilizacao: É um atributo chave que irá identificar de forma única a entidade UTILIZACAO, e por esse motivo será a chave primária no banco de dados. <br>
•	consumo_kwh: É um atributo derivado, pois através de um cálculo realizado com a potência do eletroeletrônico obtêm-se o consumo em KWh, e através deste consumo é possível saber o consumo semanal, mensal, anual ou em reais (moeda). <br>

<b> ENTIDADE NIVEL_ACESSO: </b> <br>

•	id_permissao: É um atributo chave que irá identificar de forma única a entidade NIVEL_ACESSO, e por esse motivo será a chave primária no banco de dados. <br>
•	descricao: É atributo simples (atômico) pois recebe um único valor, pois um tipo de permissão possui uma única descrição. <br>

>## Marco de Entrega 02 em: (23/04/2018)<br>
#### 5.3 DESCRIÇÃO DOS DADOS 

<b> ENTIDADE PESSOA: </b> Tabela que armazena os dados pessoais dos usuários (Master ou Comum) do aplicativo JARVIS. <br>

•	id_pessoa: Campo do tipo serial que contém o código identificador de cada pessoa/usuário do aplicativo. <br>
•	nome: Campo do tipo varchar que armazena o nome da pessoa. Exemplo: 'Maria da Silva'. <br>
•	data_nasc: Campo do tipo date que armazena a data de nascimento da pessoa. Exemplo: '20/06/1980'.  <br>
•	login: Campo do tipo varchar que armazena o nome do login de acesso da pessoa no aplicativo. Exemplo: 'maria.dasilva'. <br>
•	senha: Campo do tipo varchar que armazena a senha de acesso da pessoa no aplicativo. Exemplo: 'maria@123s80'. <br>
•	email: Campo do tipo varchar que armazena o endereço de e-mail da pessoa. Exemplo: 'mariadasilva@gmail.com'. <br>

<b> ENTIDADE LOCAL: </b> Tabela que armazena os dados dos locais/ambientes que serão adicionados pelo Master. <br>

•	id_casa: Campo do tipo serial que contém o código identificador de cada local (casa, escritório, empresa) cadastrado em um conta. <br>
•	nome: Campo do tipo varchar que armazena o nome fictício dado a cada local. Exemplo: 'Casa da Maria'. <br>

<b> ENTIDADE ENDERECO: </b> Tabela que armazena os dados do endereço onde localiza-se o local. <br>

•	id_endereco: Campo do tipo serial que contém o código identificador de cada endereço referente a cada local. <br>
•	cep: Campo do tipo char que armazena o Código de Endereçamento Postal (CEP). Exemplo: '29140-070'. <br>
•	logradouro: Campo do tipo varchar que armazena o nome da rua/avenida em que localiza-se o local cadastrado. Exemplo: 'Rua Humaitá'. <br>
•	numero: Campo do tipo varchar que armazena o número da rua/avenida. Exemplo: '2345'. <br>

<b> ENTIDADE BAIRRO: </b> Tabela que armazena os dados do bairro onde localiza-se o local. <br>

•	id_bairro: Campo do tipo serial que contém o código identificador de cada bairro referente a cada local. <br>
•	nome: Campo do tipo varchar que armazena o nome do bairro. Exemplo: 'Jardim América'. <br>

<b> ENTIDADE MUNICIPIO: </b> Tabela que armazena os dados do município onde localiza-se o local. <br>

•	id_municipio: Campo do tipo serial que contém o código identificador de cada município referente a cada local. <br>
•	nome: Campo do tipo varchar que armazena o nome do município. Exemplo: 'Cariacica'. <br>

<b> ENTIDADE ESTADO: </b> Tabela que armazena os dados do Estado onde localiza-se o local. <br>

•	id_estado: Campo do tipo serial que contém o código identificador de cada Estado/Unidade Federativa (UF) referente a cada local. <br>
•	nome: Campo do tipo char que armazena o nome do Estado/Unidade Federativa (UF). Exemplo: 'ES'. <br>

<b> ENTIDADE COMODO: </b> Tabela que armazena os dados dos cômodos do local. <br>

•	id_comodo: Campo do tipo serial que contém o código identificador de cada cômodo do local. <br>
•	nome: Campo do tipo varchar que armazena o nome fictício dado ao cômodo do local. Exemplo: 'Quarto da Ana'. <br>

<b> ENTIDADE ELETROELETRONICO: </b> Tabela que armazena os dados dos eletroeletrônicos dos cômodos. <br>

•	id_eletro: Campo do tipo serial que contém o código identificador de cada eletroeletrônico presente em casa cômodo. <br>
•	nome: Campo do tipo varchar que armazena o nome fictício dado ao eletroeletrônico presente no cômodo. Exemplo: 'Ar-condicionado Arno'. <br>
•	status: Campo do tipo varchar que armazena a situação em que se encontra um eletroeletrônico em determinado momento, informando se ele está ligado ou desligado. Exemplo: 'Ligado'. <br>
•	hora: Campo do tipo time que armazena a hora em que o eletroeletrônico foi ligado ou desligado. Este campo apenas armazena a hora, o que determina se ele foi ligado ou desligado é o seu status. Exemplo: ‘10:20:36.000’. <br>
•	potencia: Campo do tipo integer que armazena a potência em Watts do eletroeletrônico. Exemplo: 40. <br>

<b> ENTIDADE DATA_USO: </b> Tabela que armazena os dados referentes às datas que foram utilizados os equipamentos do local. <br>

•	id_data: Campo do tipo serial que contém o código identificador das datas de utilização dos eletroeletrônicos presentes em casa cômodo. <br>
•	data_uso: Campo do tipo date que armazena a data em que foi usado o eletroeletrônico. Exemplo: '04/05/2018'. <br>

<b> ENTIDADE UTILIZACAO_ELETRO: </b> Tabela que armazena os dados referentes à utilização do eletroeletrônico. <br>

•	id_utilizacao: Campo do tipo serial que contém o código identificador da utilização dos eletroeletrônicos presentes em casa cômodo. <br>
•	consumo_kwh: Campo do tipo float que armazena o valor do consumo de energia elétrica em KWh. Exemplo: 46,08. <br>

<b> ENTIDADE NIVEL_ACESSO: </b> Tabela que armazena os dados sobre os níveis de acesso (permissões) dadas aos Usuários Comuns. <br>

•	id_permissao: Campo do tipo serial que contém o código identificador do nível de permissão de cada usuário. <br>
•	descricao: Campo do tipo text que armazena um texto com a descrição dos níveis de acesso. Exemplo: 'A pessoa possui controle sobre o equipamento em questão, podendo ligá-lo e desligá-lo'.  <br>


### 6	MODELO LÓGICO<br>

![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Modelo%20Lo%CC%81gico%20-%20Jarvis.png "Modelo Lógico - JARVIS")

### 7	MODELO FÍSICO<br>

[Modelo Físico](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/ModeloFisico.sql)
        
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES

[Insert](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Insert.sql)

#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS

[Create + Insert](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/CreateInsert.sql)

#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS

[Drop + Create + Insert](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/DropCreateInsert.sql)

>## Marco de Entrega 03 em: (14/05/2018)<br>

### 9	TABELAS E PRINCIPAIS CONSULTAS<br>

    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.
    
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

    select * from comodo;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20comodo.PNG "Select - Cômodos")

    select * from eletroeletronico;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20eletroeletronico.PNG "Select - Eletroeletrônicos")

    select * from local;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20local.PNG "Select - Local")

    select * from nivel_acesso;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20nivel_acesso.PNG "Select - Nível Acesso")

    select * from pessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20pessoa.PNG "Select - Pessoa")

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

    select * from eletroeletronico where status='Ligado';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20eletroeletronico%20where%20status%3D'Ligado'.PNG "Where - Status Ligado")

    select id_eletro, nome, hora from eletroeletronico where status='Desligado';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20id_eletro%2C%20nome%2C%20hora%20from%20eletroeletronico%20where%20status%3D'Desligado'.PNG "Where - Status Deligado")

    select id_eletro, nome, potencia, fk_comodo from eletroeletronico where potencia>=1000;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20id_eletro%2C%20nome%2C%20potencia%2C%20fk_comodo%20from%20eletroeletronico%20where%20potencia1000.PNG "Where - Potência")

    select id_pessoa, nome, data_nasc from pessoa where data_nasc<='1980-01-01';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20id_pessoa%2C%20nome%2C%20data_nasc%20from%20pessoa%20where%20data_nasc'1980-01-01'%3B.PNG "Where - Data Nascimento")

#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    
<br>

    select * from eletroeletronico where status='Ligado' and potencia<300;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20%20from%20eletroeletronico%20where%20status%3D'Ligado'%20and%20potencia300%3B.PNG "Operadores Lógicos 1")
    
    select * from eletroeletronico where hora>='12:00:00' and hora<='20:00:00';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20%20from%20eletroeletronico%20where%20hora'120000'%20and%20hora'200000'%3B.PNG "Operadores Lógicos 2")    
    
    select * from comodo where not fk_local=4 and not fk_local=5 and not fk_local=7 and not fk_local=8 and not fk_local=10;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20%20from%20comodo%20where%20not%20fk_local%3D4%20and%20not%20fk_local%3D5%20and%20not%20fk_local%3D7%20and%20not%20fk_local%3D8%20and%20not%20fk_local%3D10.PNG "Operadores Lógicos 3")    
    
    select * from comodo where nome='Sala' or nome='Sala Principal' or nome='Sala Entrada' or nome='Minha Sala';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20%20from%20comodo%20where%20nome%3D'Sala'%20or%20nome%3D'Sala%20Principal'%20or%20nome%3D'Sala%20Entrada'or%20nome%3D'Minha%20Sala'.PNG "Operadores Lógicos 4")    
    
    select * from eletroeletronico where (nome='TV' or nome='TV Samsung' or nome='TV 42"') and (hora<'12:00:00') and (not potencia=2.0);
 ![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_3_a_1.PNG "Operadores Lógicos 5") 
    
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    
<br>

    select id_eletro, nome, potencia, (potencia / 1000.0) as Consumo_KWh from eletroeletronico limit 10
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20id_eletro%2C%20nome%2C%20potencia%2C%20(potencia%20%201000.0)%20as%20Consumo_KWh%20from%20eletroeletronico%20limit%2010.PNG "Select - Operadores Aritméticos")

    select id_eletro, nome, potencia, (potencia * 30 / 1000.0) * 0.485 as Consumo_R$_1hdia_30dias from eletroeletronico limit 7
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20id_eletro%2C%20nome%2C%20potencia%2C%20(potencia%20%2030%20%201000.0)%200.485%20as%20Consumo_R%24_1hdia_30dias%20from%20eletroeletronico%20limit%207.PNG "Select - Operadores Aritméticos")

    select id_pessoa, nome, (extract('month' from data_nasc))+(extract('day' from now()))+(extract('year' from data_nasc)) as "Soma dia+mes+ano" from pessoa limit 5
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9.3.b.3.PNG "Select - Operadores Aritméticos")

<br>

    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
    
<br>

    select * from comodo as c where c.nome ilike '%Sala%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20from%20comodo%20as%20c%20where%20c.nome%20ilike%20'Sala.PNG "Select - Renomear")

    select * from eletroeletronico as elt where elt.potencia<250;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20%20from%20eletroeletronico%20as%20elt%20where%20elt.potencia250%3B.PNG "Select - Renomear")

    select hora, nome from eletroeletronico as el where el.hora<'12:00:00' and el.nome like '%Ar%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/select%20hora%2C%20nome%20from%20eletroeletronico%20as%20el%20where%20el.hora120000'%20and%20el.nome%20like%20'Ar.PNG "Select - Renomear")
    
#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>

    a) Criar outras 5 consultas que envolvam like ou ilike
    
<br>

    select * from comodo where nome like 'Sala%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_1.PNG "Like")

    select * from eletroeletronico where nome ilike '%TV ';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_2.PNG "iLike")

    select * from local where nome ilike 'Casa d%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_3.PNG "iLike")

    select * from pessoa where nome ilike 'A%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_4.PNG "iLike")

    select * from pessoa where email like '%gmail.com';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_5.PNG "Like")

    select * from eletroeletronico where nome like '%Elétrico%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_6.PNG "Like")

    select * from eletroeletronico where status ilike 'Lig%';
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_a_7.PNG "iLike")

    b) Criar uma consulta para cada tipo de função data apresentada.
    
<br>

    select id_pessoa, nome, data_nasc, email, (age(current_date, data_nasc)) from pessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9.4.b.1.PNG "age, current_date")

    select id_pessoa, nome, data_nasc, email, date_part('year',(age(current_date, data_nasc))) as idade from pessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9.4.b.2.PNG "current_date, date_part, 'year', age")

    select id_pessoa, nome, data_nasc, email from pessoa where extract('year' from data_nasc)<1990;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_b_3.PNG "extract, 'year'")

    select id_pessoa, nome, data_nasc, email from pessoa where date_part('year', age(current_date, data_nasc))>40;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_b_4.PNG "date_part, 'year', age, current_date")

    select id_pessoa, nome, data_nasc, email, extract('month' from data_nasc) as MES_NASCIMENTO from pessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9_4_b_5.PNG "extract, 'month'")

>## Marco de Entrega 04 em: (04/06/2017)<br>
    
#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

<br> 

    update pessoa set nome='Vanessa Silva Cardoso' where login='vanessa.silva';
    select nome, login from pessoa;
    
Antes do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/blob/master/arquivos/1a.PNG?raw=true "Update")
<br>

Depois do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/1.PNG "Update")

    update local set nome='Casa do Santero' where id_local=11;
    select id_local, nome from local;
    
Antes do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/2a.PNG "Update")
<br>

Depois do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/2.PNG "Update")

    update pessoa set email='vanessacardoso@gmail.com' where login='vanessa.silva';
    select nome, login, email from pessoa;

Antes do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/3a.PNG "Update")
<br>

Depois do Update:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/3.PNG "Update")

    delete from eletroeletronico where fk_comodo=1;
    select * from eletroeletronico limit 7

Antes de Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/4a.PNG "Delete")
<br>

Depois do Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/4.PNG "Delete")

    delete from eletroeletronico where nome like '%Ar%';
    select id_eletro, nome, fk_comodo from eletroeletronico;

Antes de Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/5a.PNG "Delete")
<br>

Depois do Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/5.PNG "Delete")

    delete from eletroeletronico where potencia=2.0;
    select id_eletro, nome, potencia from eletroeletronico limit 7

Antes de Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/6a.PNG "Delete")
<br>

Depois do Delete:
<br>
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/6.PNG "Delete")

#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)

<br>

        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        
<br>

        select p.nome as "Pessoa", l.nome as "Local", c.nome as "Cômodo", e.nome as "Eletro" from eletroeletronico e
        inner join comodo c
        on (c.id_comodo=e.fk_comodo)
        inner join local l
        on (l.id_local=c.fk_local)
        inner join pessoa p
        on (p.id_pessoa=l.fk_pessoa)
        limit 7
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/7.PNG "Join")

      b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
      
<br>

    select p.nome as "Nome da Pessoa", l.nome as "Local da Pessoa" from local l
    inner join pessoa p
    on (p.id_pessoa=l.fk_pessoa)
    order by p.nome asc
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/8.PNG "Join")

    select l.nome as "Local", c.nome as "Cômodo", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    inner join local l
    on (l.id_local=c.fk_local)
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/9.PNG "Join")

    select l.nome as "Local", c.nome as "Cômodo" from comodo c
    inner join local l
    on (l.id_local=c.fk_local)
    order by l.nome ilike '%casa%' desc
    limit 10
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/10.PNG "Join")

    select c.nome as "Cômodo", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    order by c.nome asc
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/11.PNG "Join")

    select l.nome as "Local", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    inner join local l
    on (l.id_local=c.fk_local)
    order by e.nome asc
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/12.PNG "Join")
   
#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)

<br>

    select nome as "Eletros" from eletroeletronico group by nome;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/13.PNG "Group by")
    
    select fk_local as "Identificador do CÙmodo", count(fk_local) as "Contagem" from comodo group by fk_local;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/14.PNG "Count")
    
    select nome as "Eletro", count(*) as "Quantidade" from eletroeletronico group by nome;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/15.PNG "Group by e Count")
    
    select l.nome as "Local", count(*) as "Qtd Cômodos" from comodo c
    inner join local l
    on (l.id_local=c.fk_local)
    group by l.nome
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/16.PNG "Group by e count")
    
    select l.nome as "Local", count(l.nome) as "Qtd Eletros" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    inner join local l
    on (l.id_local=c.fk_local)
    group by l.nome
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/17.PNG "Group by e count")

    select avg(potencia) as "Média Potência dos Eletros" from eletroeletronico;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/18.PNG "Avg")

    select count(*) as "N˙mero de Pessoas" from pessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/19.PNG "Count")

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)

<br>

    select c.nome as "CÙmodo", c.fk_local, l.nome as "Local", l.id_local from local l
    right outer join comodo c
    on (l.id_local=fk_local)
    limit 7
![Alt text]( https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/20.PNG "Right Join")
    
    select p.id_pessoa, p.nome as "Nome da Pessoa", l.nome as "Local da Pessoa", l.fk_pessoa from local l
    right outer join pessoa p
    on (p.id_pessoa=l.fk_pessoa)
    limit 7
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/21.PNG "Right Join")
    
    select l.nome as "Local", e.nome as "Eletro" from eletroeletronico e
    left outer join comodo c
    on (c.id_comodo=e.fk_comodo)
    right outer join local l
    on (l.id_local=c.fk_local)
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/22.PNG "Left Join")
    
    select c.id_comodo, c.nome as "CÙmodo", e.nome as "Eletro", e.fk_comodo from eletroeletronico e
    left outer join comodo c
    on (c.id_comodo=e.fk_comodo)
    limit 7
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/23.PNG "Left Join")

#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)

<br>

        a) Uma junção que envolva Self Join
        
    select e1.id_eletro, e1.nome, e1.potencia, e2.id_eletro, e2.nome, e2.potencia
    from eletroeletronico as e2
    inner join eletroeletronico e1
    on (e2.potencia=e1.potencia and e2.id_eletro<>e1.id_eletro)
    order by 1, 2
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/24.PNG "Self Join")

    b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
    
<br>

    create view vwPessoa as
    select id_pessoa as "Identificação", nome as "Nome da Pessoa", email as "Endereço de e-mail", login as "Login", senha as "Senha", tipo_pessoa as "Tipo de Usuário" from pessoa
    
    select * from vwPessoa;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/25.PNG "View")

    create view viewComodo as
    select c.id_comodo as "ID CÙmodo", c.nome as "CÙmodo", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    
    select * from viewComodo;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/26.PNG "View")
 
    create view vwPessoaNasc as
    select id_pessoa as "ID", nome as "Nome", data_nasc as "Nascimento", (age(current_date, data_nasc)) as "Tempo de vida" from pessoa;

    select * from vwPessoaNasc;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/27.PNG "View")

    create view vwPessoaIdade as
    select id_pessoa as "ID", nome as "NOME", data_nasc "NASCIMENTO", date_part('year',(age(current_date, data_nasc))) as "IDADE" from pessoa;

    select * from vwPessoaIdade;
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/28.PNG "View")
    
    create view viewPessoaLocal as
    select p.id_pessoa, p.nome as "Nome da Pessoa", l.nome as "Local da Pessoa" from local l
    inner join pessoa p
    on (p.id_pessoa=l.fk_pessoa)
    order by 1, 3

    select * from viewPessoaLocal;  
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/29.PNG "View")

#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

    select c.nome as "Cômodo", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    where c.nome in (
        select nome from comodo where nome ilike 'a%')
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/30.PNG "Subconsulta")     
        
    select l.nome as "Local", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    inner join local l
    on (l.id_local=c.fk_local)
    where e.status in (
        select status from eletroeletronico where status='Desligado' )
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/31.PNG "Subconsulta") 

    select l.nome as "Local", c.nome as "CÙmodo", e.nome as "Eletro" from eletroeletronico e
    inner join comodo c
    on (c.id_comodo=e.fk_comodo)
    inner join local l
    on (l.id_local=c.fk_local)
    where c.nome in (
        select nome from comodo where nome ilike '%Sala%')
![Alt text](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/32.PNG "Subconsulta") 

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>

### 11 Backup completo do banco de dados postgres 

[Backup Jarvis](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/backupJarvis.backup)

Grupo que realizou o teste: Antônio, Jennifer, Joel e Larissa.

### 12	TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>

[Tutorial Jarvis](https://github.com/CasaInteligenteBD1/trab01_ci/raw/master/arquivos/Tutorial%20Jarvis.pdf)

        a) Outros grupos deverão ser capazes de restaurar o banco 
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho 
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho
        
### 13   DIFICULDADES ENCONTRADAS PELO GRUPO<br>

<p align = "justify"> - A maior dificuldade, quanto ao conteúdo, foi na construção do modelo conceitual e no diagrama de classes (da matéria de Análise de Sistemas). Ao final do trabalho pude perceber por conta própria que um bom modelo conceitual e teria me facilitado na implementação do banco de dados. </p>
<p align = "justify"> - Outra dificuldade foi quanto à falta do computador que dificultou com que eu realizasse todas as atividades e me sobrecarregou para entrega do trabalho num período curto de tempo (normalmente na última semana de entrega). Levando também em consideração as outras disciplinas com uma grande quantidade de trabalhos, e conciliando com a falta de um computador para realizar as tarefas, o tempo se tornou reduzido uma vez que para fazer os trabalhos de BDI eu tinha que utilizar os computadores do IFES. Dessa forma, não consegui realizar os trabalhos da melhor forma possível (o mesmo digo para a aprova). Queria ter tido um resultado melhor, dei o melhor de mim, porém, infelizmente, como você mesmo disse "o tempo é finito". Corri contra o tempo para entregar tudo, mesmo que não estivesse tão bom, mas se eu tivesse uma sobrecarga menor, com certeza entregaria um trabalho mais bem feito. </p>

### Observação

<p align = "justify"> <b> Além de fazer os tópicos da entrega final (9.5 a 13), fiz algumas pequenas alterações nas seções anteriores como no minimundo, regras de negócio, protótipos, modelo conceitual, modelo lógico e diagrama de classes. Também alterei algumas consultas e tabelas da seção 9.3b e 9.4b, além de adicionar as tabelas que estavam faltando da entrega anterior (seção 9 a 9.4), que não foram adicionadas por erro de digitação. </b> </p>

>## Marco de Entrega Final em: (25/06/2018)<br>




        
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/



    

    
### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")

