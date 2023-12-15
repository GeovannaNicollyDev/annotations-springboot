# annotations-springboot
Repositório com annotations mais usadas no SpringBoot

-Annotations comuns:

@Autowired: A anotação @Autowired é usada para injetar dependências automaticamente em um objeto. Por exemplo, se um objeto precisa de uma instância de um serviço, a anotação @Autowired pode ser usada para injetar essa instância no objeto.
@controller: A anotação @controller é usada para indicar que uma classe é um controlador de Spring MVC. Essa anotação é frequentemente usada em conjunto com as anotações @RequestMapping e @responsebody.
@RequestMapping: A anotação @RequestMapping é usada para mapear uma solicitação HTTP para um método em um controlador. Essa anotação pode ser usada para especificar a URL da solicitação, o método HTTP e os parâmetros.
@service: A anotação @service é usada para marcar uma classe como um serviço. Essa anotação é frequentemente usada em conjunto com a anotação @Autowired para injetar dependências em um serviço.
@repository: A anotação @repository é usada para marcar uma classe como um repositório. Essa anotação é frequentemente usada em conjunto com a anotação @Autowired para injetar dependências em um repositório.
@transactional: A anotação @transactional é usada para indicar que um método deve ser executado dentro de uma transação. Essa anotação é frequentemente usada em conjunto com as anotações @service e @repository.
@component: A anotação @component é usada para marcar uma classe como um componente do Spring. Essa anotação é usada quando não há uma anotação mais específica disponível.
@PathVariable: A anotação @PathVariable é usada para mapear uma variável de caminho em uma URL para um parâmetro de método em um controlador. Essa anotação é útil quando uma parte da URL contém dados que precisam ser passados para o método do controlador.
@requestbody: A anotação @requestbody é usada para indicar que o corpo de uma solicitação HTTP deve ser convertido em um objeto Java. Essa anotação é útil quando um método de controlador espera um objeto JSON ou XML no corpo da solicitação.
@ModelAttribute: A anotação @ModelAttribute é usada para vincular um objeto de modelo a um formulário ou a uma solicitação HTTP. Essa anotação é útil quando um método de controlador precisa preencher um objeto de modelo com dados do usuário.
@ResponseStatus: A anotação @ResponseStatus é usada para definir o status HTTP de uma resposta gerada por um método de controlador. Essa anotação é útil quando um método de controlador precisa gerar um status HTTP personalizado.
Essas são apenas algumas das anotações Spring mais comuns. Existem muitas outras anotações disponíveis no Spring Framework para ajudar a simplificar o desenvolvimento de aplicativos empresariais. O uso de anotações pode ajudar a tornar o código mais claro e fácil de entender, e pode reduzir significativamente a quantidade de código necessário para implementar recursos específicos.

-Annotations avançadas:

@configuration: A anotação @configuration é usada para indicar que uma classe contém definições de beans do Spring. As definições de beans podem ser usadas para configurar o contexto do aplicativo Spring, como a configuração de bancos de dados, a criação de instâncias de beans, etc.
@bean: A anotação @bean é usada para marcar um método que retorna um objeto que deve ser gerenciado pelo contêiner do Spring como um bean. Esta anotação é frequentemente usada em conjunto com a anotação @configuration.
@componentscan: A anotação @componentscan é usada para indicar que o contêiner do Spring deve procurar por classes anotadas com @component, @service, @repository, @controller, etc., e registrá-las como beans no contexto do aplicativo.
@Profile: A anotação @Profile é usada para indicar que um bean deve ser registrado apenas se um perfil específico do Spring estiver ativado. Esta anotação é usada para permitir que diferentes configurações sejam usadas com base no ambiente de execução do aplicativo, como “dev”, “test” ou “production”.
@conditional: A anotação @conditional é usada para registrar um bean somente se uma determinada condição for atendida. Esta anotação é usada para permitir que diferentes beans sejam registrados com base nas condições de tempo de execução, como o sistema operacional ou a presença de uma determinada classe no classpath.
@async: A anotação @async é usada para indicar que um método deve ser executado de forma assíncrona. Esta anotação é usada para permitir que métodos longos ou intensivos em recursos sejam executados em segundo plano, sem bloquear a thread principal.
@transactional: A anotação @transactional é usada para indicar que um método deve ser executado dentro de uma transação. Esta anotação é frequentemente usada em conjunto com as anotações @service e @repository para garantir a integridade dos dados em operações de banco de dados.
Essas são algumas das anotações mais avançadas disponíveis no Spring Framework. Essas anotações permitem que os desenvolvedores implementem recursos mais avançados e flexíveis em seus aplicativos, além de simplificar o código e aumentar a produtividade.

-Annotations para Injeção de dependência:

@Autowired: A anotação @Autowired é usada para injetar uma dependência em um objeto. A dependência é automaticamente resolvida pelo contêiner do Spring e atribuída à variável anotada. Essa anotação pode ser usada em construtores, métodos e campos.
@qualifier: A anotação @qualifier é usada para especificar qual implementação de uma interface ou classe abstrata deve ser injetada em um objeto. Esta anotação é usada quando há várias implementações disponíveis e o contêiner do Spring precisa saber qual implementação usar.
@value: A anotação @value é usada para injetar valores de propriedades em uma classe. Os valores podem ser definidos em um arquivo de propriedades externo ou em um arquivo de configuração do Spring.
@resource: A anotação @resource é usada para injetar uma dependência em um objeto. Ela é semelhante à anotação @Autowired, mas permite especificar o nome do bean que deve ser injetado.
@Inject: A anotação @Inject é semelhante à anotação @Autowired. Ela é usada para injetar uma dependência em um objeto e pode ser usada em construtores, métodos e campos.
@lazy: A anotação @lazy é usada para atrasar a criação de um bean até que ele seja necessário. Isso pode ajudar a melhorar o desempenho e a eficiência do aplicativo, pois os beans não são criados até que sejam necessários.
@primary: A anotação @primary é usada para indicar que um bean deve ser usado como o bean principal quando há várias implementações disponíveis. Essa anotação é usada quando o contêiner do Spring não sabe qual implementação usar.
Essas são algumas das anotações de injeção de dependência disponíveis no Spring Framework. O uso dessas anotações pode ajudar a simplificar o código e melhorar a legibilidade do código, além de permitir que as dependências sejam gerenciadas pelo contêiner do Spring.

-Annotations para tratamento de Exceções:

@ExceptionHandler: A anotação @ExceptionHandler é usada para tratar exceções lançadas por um controlador. Quando uma exceção é lançada, o controlador correspondente ao tipo de exceção é chamado e pode executar uma ação personalizada, como retornar uma página de erro personalizada.
@ControllerAdvice: A anotação @ControllerAdvice é usada para definir um controlador global que pode interceptar exceções lançadas por outros controladores. Isso permite que um único controlador trate exceções em toda a aplicação.
@ResponseStatus: A anotação @ResponseStatus é usada para definir o código de status HTTP que deve ser retornado quando uma exceção é lançada. Isso pode ajudar a fornecer informações adicionais aos usuários sobre a natureza do erro que ocorreu.
@ExceptionHandlerAdvice: A anotação @ExceptionHandlerAdvice é usada para definir um controlador que pode tratar exceções em toda a aplicação. Essa anotação é semelhante à anotação @ControllerAdvice, mas permite definir um controlador que pode tratar exceções de forma mais geral.
@ControllerAdvice(basePackages=”com.example”): A anotação @ControllerAdvice pode ser usada com um parâmetro “basePackages” para especificar o pacote ou pacotes que o controlador deve monitorar para exceções. Isso pode ser útil para definir controladores diferentes para diferentes áreas da aplicação.

-Annotations do Spring JPA:

@entity: anotação utilizada para indicar que uma classe é uma entidade JPA, ou seja, será mapeada para uma tabela no banco de dados.
@table: anotação utilizada para especificar o nome da tabela correspondente à entidade.
@id: anotação utilizada para indicar a chave primária da tabela. É possível especificar o tipo de dado da chave primária com a anotação @GeneratedValue.
@column: anotação utilizada para especificar o nome da coluna correspondente a um atributo da entidade. Também é possível especificar o tipo de dado da coluna com as anotações @TeMPOraL e @Enumerated.
@OnetoOne, @OneToMany, @manytoone, @manytomany: anotações utilizadas para especificar os relacionamentos entre as entidades. É possível configurar as propriedades de cada relacionamento, como nome da coluna de junção.
@transient é utilizada no Spring JPA (Java Persistence API) para indicar que um determinado atributo de uma entidade não deve ser persistido no banco de dados.

Ao marcar um atributo com a anotação @transient, o Spring JPA irá ignorar esse campo durante as operações de persistência e recuperação de dados. Isso significa que o valor desse atributo não será armazenado no banco de dados e nem será recuperado quando a entidade for carregada.
Essa anotação pode ser útil em situações em que você tem um atributo em uma entidade que não precisa ser persistido no banco de dados, como um campo calculado ou um atributo temporário que não deve ser armazenado permanentemente.


