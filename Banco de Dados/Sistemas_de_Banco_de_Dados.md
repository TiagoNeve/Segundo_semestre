# Sistemas de Banco de Dados

## Tema 01 -> Reconhecer o histórico dos bancos de dados e suas tecnologias

* Definição de Banco de Dados
    O termo banco de dados, no sentido técnico, origina-se de 
    **database**. "Banco de dados é uma coleção de dados relacionados"
    Ou seja, Dados são **fatos conhecidos que podem ser registados e possuem significado implícito.**
    Ex: Nome, data de nascimento, endereço e telefone são dados
    relacionados entre si, inerentes a uma pessoa conhecida em
    certo contexto.
    No contexto histórico, banco de dados sempre existiu, mas
    foi bem explorado nos sistemas de informações. Por exemplo, 
    sempre houve armários dedicados a guardar arquivos de 
    clientes e funcionários, para posterior consulta, isso pode
    ser qualificado como banco de dados, pois é dedicado a 
    guardar informações. É de se esperar que a cada nova 
    tecnologia desenvolvida, alguma área da inteligência 
    humana há de mudar.

* Evolução dos sistemas de informação em computador
    ### Era do processamento de dados 
    Basicamente quando o computador foi inventado o seu 
    principal uso era o de fazer cálculos, com o tempo foi 
    percebido que tal máquina poderia fazer muito mais do que 
    apenas isso, no começo ele conseguia guardar programas e 
    dados em sua memória, logo tentaram fazer esses dados 
    serem processados pelo computador e funcionou, dessa forma
    foi dado um novo olhar a essa "calculadora gigante"
    Com essa nova oportunidade a IBM lançou um disco magnético,
    capaz de guardar mais informações que a memória que o 
    computador tinha, essa invenção foi denominado de DASD -
    **Direct Acess Storage Device**, precursor do HD.
    Com a possibilidade de guardar mais dados, iniciou-se a era
    do processamento de dados do computador.
    Utilizando as linguagens de programação é possível manipular
    os dados guardados nesses HD's, essa utilidade é chamado de
    Sistema de arquivos, desta forma os programas passaram a 
    acessar as informações nesses sistemas de arquivos, evitando
    ter que deixar esses dados internamente no seu aplicativo.
    Logo, dando uma segurança maior dos dados e tornando os 
    programas mais leves, utilizando a métrica binária.
    Porém, antes de termos os banco de dados como eles são hoje
    tivemos alguns problemas com eles, como por exemplo 
    compartilhamento de dados com outros sistemas e aplicativos.
    Antes cada aplicação, sistema tinha o seu próprio Banco de
    Dados, quando precisava compartilhar esses dados com outro
    sistema era feito uma cópia do banco e implementado ao outro,
    Dessa forma os gerava uma sobrecarga de dados e duplicidade,
    para resolver essa questão foi desenvolvido um software 
    intermediário, que recebe as solicitações dos sistemas para 
    manipular os dados e ele mesmo faz o processo de buscar os
    dados e entregar para o sistema ou então substituir os dados 
    que se encontram no sistema de arquivos, esse software foi 
    denominado de SGBD. **Sistema de gerência de banco de dados**
    Assim fica: BD <-> SGBD <-> Aplicação
    ### Estágio atual dos sistemas de informação (na Web)
    Atualmente o uso de SGBD's são básicos para um controle das
    informações, nesse mundo de internet e globalizado mais tipos
    de sistemas foi desenvolvido e linguagens diferentes foram 
    criadas e utilizadas, desta forma o SGBD evoluiu para se 
    adequar a linguagens e sistemas diferentes, atuando como um
    middleware, aquele que é usado no meio do sistema para ajudar
    na comunicação entre o lado do cliente e do servidor. Com o
    uso desse Middleware é possível acessar banco de dados em 
    locais diferentes, manipular com maior velocidade, segurança a mais, escalabilidade e ter uma comunicação melhor e precisa
    com a fonte de dados, com esse tipo de sistema foi possível
    a evolução da Big Data. 
    Separando as funcionalidades desse jeito, foi possível a
    multiconexão entre os dispositivos, desta forma tanto um
    computador como um smartphone ou tv pode acessar os mesmos 
    dados, até mesmo sistemas em Cloud Computing, que estão 
    quase sempre conectados a internet consegue solicitar as infos
    de uma aplicação, e essa aplicação solicita do SGBD. Portanto, 
    a evolução desse campo deixou tudo mais conectado.

* Evolução dos sistemas de Banco de Dados
    ### Bancos de dados navegacionais
    Dois sistemas iniciaram essa evolução, o IDS e o IMS.
    O IDS foi desenvolvido por Charles Bachman, do comitê de
    padronização, o mesmo que padronizou a linguagem COBOL.
    O IMS foi desenvolvido pela IBM, após criar os discos
    magnéticos.
    São chamados dessa maneira pois o método de busca dos dados
    eram do tipo de navegação, esses sistemas iam de registro em 
    registro comparando as informações com os dados solicitados.
    IDS -> Usa o sistema de Grafos ou Redes, Network databases
    IMS -> Usa o sistema de Árvores, Hierarchical databases
    Na evolução desses sistemas foram desenvolvidos os SGBD's 
    DMS (Data Management System) e o IDMS (Integrated Database Management System).
    ### O modelo relacional de banco de dados
    Pensado por um matemático pesquisador da IBM, Edgar Codd, em 
    que gera uma relação entre diversos bancos de dados, evitando
    uma super aglomeração de informações em um único banco, assim
    se um banco se relacionar com outro, se comunicando, é possível
    organizar melhor as informações e não gerará tanto impacto no
    desempenho de buscas. Com essa ideia, a IBM patrocionou o 
    projeto System R (Relational) e com isso foi desenvolvido o 
    modelo de banco de dados mais utilizado atualmente.
    ### Principais SGBDs relacionais
    O projeto System R deu origem ao SGBD comercial da IBM
    inicialmente denominado SQL/DS (Structured Query Language / Data System), depois renomeado de DB2. A IBM criou a linguagem
    SQL, usada por vários Bancos de dados e modificadas para 
    algumas outros bancos de dados. No decorrer dos anos houveram
    muitos nomes associados a esse sistema de banco de dados, mas
    o que perdurou foi o Oracle Corporation, um dos maiores SGBD
    usado comercialmente. Além de ter adquirido a Sun Microsystems
    e ter tomado o controle do MySQL, um dos maiores SGBDs de
    software livre e usado amplamente pela comunidade.
    Houve vários outros pesquisadores que tomaram a ideia de SGBD
    relacionais, como por exemplo o projeto Ingres que mais tarde
    gerou o SQL Server da Microsoft.
    Além do SQL Server o projeto Ingres também teve um público
    voltado a comunidade, com o desenvolvimento do SGBD Postgress,
    que tem como base o modelo relacional e com conceitos de
    programação orientada a objetos. Conhecido atualmente como 
    PostgreSQL.
    ### Outros modelos de SGBDs
    Tais SGBDs possum muitos recursos além do Relacional. 
    Oracle: Relacional e multimodelo (Documentos, grafos e RDF)
    MySQL: Relacional e multimodelo (Documentos)
    SQL Server: Relacional e multimodelo (Documentos e grafos)
    PostgreSQL: Relacional e multimodelo (Documentos)
    IBM DB2: Relacional e multimodel (RDF)
    Mesmo com toda essa tecnologia de banco de dados Relacionais 
    em algum momento não será possivel dar conta de alguns sistemas
    como é o caso de aplicações robustas de cunho científico, que
    utiliza a tecnologia de Big Data, Internet of Things e Data
    Science, para esses sistemas em que ocorre muita manipulação de
    dados em pouco período de tempo é necessário utilizar um novo
    tipo de Banco de dados, chamado de NoSQL. São bancos de dados
    que não tem como linguagem principal o SQL, mas podem também
    utilizar para manipulações básicas, sempre recomendado para 
    sistemas que irão tratar muitos dados em pouco tempo.
    