# carrinho-compra-java-jsp-session
 

## Sessão JSP - Objeto Implícito

Em JSP, a sessão é o objeto implícito usado com mais frequência do tipo HttpSession . É usado principalmente para abordar todos os dados do usuário até que a sessão do usuário esteja ativa. 

Os métodos usados ​​na sessão Objeto implícito são os seguintes:

**Método 1:** isNew(): Este método é usado para verificar se a sessão é nova ou não. O valor booleano (verdadeiro ou falso) é retornado por ele. Principalmente, é usado para rastrear os cookies estão habilitados no lado do cliente ou não. Se os cookies não estiverem habilitados, o método session.isNew() deve retornar verdadeiro o tempo todo.

**Método 2:** getId(): ao criar uma sessão, o contêiner de servlet atribui um identificador de string distinto à sessão. Este identificador de string distinto é retornado pelo método getId .

**Método 3: **getAttributeNames(): Todos os objetos armazenados na sessão são retornados pelo método getAttributeNames . Fundamentalmente, esse método resulta em uma enumeração de objetos.

**Método 4:** getCreationTime(): A hora de criação da sessão (a hora em que a sessão se tornou ativa ou a sessão começou) é retornada pelo método getCreationTime .

**Método 5:** getAttribute (String name): Usando o método getAttribute , o objeto que é armazenado pelo método setAttribute() é recuperado da sessão. Por exemplo, precisamos armazenar o “userid” na sessão usando o método setAttribute() se houver a necessidade de acessar o userid em cada página jsp até que a sessão esteja ativa e quando necessário, ela pode ser acessada usando o método getAttribute().

**Método 6: **setAttribute (String, object): O método setAttribute é usado para armazenar um objeto na sessão atribuindo uma string única ao objeto. Posteriormente, usando a mesma string, este objeto pode ser acessado da sessão até que ela esteja ativa. No JSP, ao lidar com a sessão, setAttribute() e getAttribute() são os dois métodos mais usados ​​regularmente.

**Método 7:** getMaxInactiveInterval(): o intervalo de tempo máximo de inatividade da sessão de retorno getMaxInactiveInterval em segundos.

**Método 8:** getLastAccessedTime: O método getLastAccessedTime é usado principalmente para observar a hora do último acesso de uma sessão.

**Método 9:** removeAttribute (String name): Usando o método removeAttribute (String name) , os objetos que estão armazenados na sessão podem ser removidos da sessão.

### Referências Estudos
- https://acervolima.com/sessao-jsp-objeto-implicito/
- https://www.softblue.com.br/course/home/id/4

**Método 10** : invalidate(): O método invalidate() termina uma sessão e interrompe a conexão da sessão com todos os objetos armazenados.
