# O que é AWS Lambda?

Nesse artigo vamos conhecer o AWS Lambda, serviço de computação Serveless da AWS especializado em executar funções sem a necessidade de se preocupar com servidores.

 cerca de 1 ano atrás

[Artigos](https://www.treinaweb.com.br/blog)O que é AWS Lambda?

O [AWS](https://www.treinaweb.com.br/blog/introducao-a-amazon-web-services-aws/) Lambda é um serviço de computação que executa suas aplicações em um modelo serveless, onde você pode desenvolver sem a necessidade de se preocupar com servidores.

É possível utilizar as principais linguagens do mercado, como Java, Pyhton, Node.JS, .NET Core, e Go, podendo expandir essa lista para outras linguagens utilizando um [custom Lambda Runtime](https://docs.aws.amazon.com/lambda/latest/dg/runtimes-custom.html), adicionando [suporte até para COBOL](https://github.com/BluAge/ServerlessCOBOLforAWS)!

Além disso, com o Lambda você só paga pelo o que você consumir para executar sua função. Não é necessário pagar por capacidade ociosa e, por fim você pode publicar sua aplicação de forma mais ágil. Vamos entender a seguir como e quando utilizar o Lambda pode ser interessante.



![Amazon Web Services (AWS) - Fundamentos](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/aws.svg)

##### CursoAmazon Web Services (AWS) - Fundamentos

[Conhecer o curso](https://www.treinaweb.com.br/curso/amazon-web-services-aws-fundamentos)

## O que é serverless?

Antes de falarmos sobre Lambda, vamos esclarecer o que é Serveless. Muitos já devem ter ouvido falar sobre esse termo associando ao pensamento de executar sem precisar de um servidor.

Na verdade, serverless é um modelo de serviço de nuvem onde você não precisa se preocupar com a infraestrutura da sua aplicação. Esse servidor ainda existe, entretanto ele é totalmente gerenciado pelo provedor de nuvem, te permitindo focar somente na lógica do seu negócio.

Um diferencial do Serveless é que você paga somente o que sua aplicação utilizar. Ao contrário de uma [EC2](https://www.treinaweb.com.br/blog/criando-instancias-no-amazon-ec2/) tradicional, você pode ser cobrado pelo tempo ocioso nessa EC2, em momentos onde sua aplicação não tem nenhuma atividade.

Além do Lambda, temos outros exemplos de serviços da AWS que funcionam no modelo de Serveless. Alguns exemplos são o [S3](https://www.treinaweb.com.br/blog/o-que-e-aws-s3/) para armazenamento de arquivos, o AWS RDS Aurora e DynamoDB para banco de dados, e SNS e SQS, serviços usados para gerenciar filas e mensageiria.



![Amazon Web Services (AWS) - S3 - Fundamentos](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/aws.svg)

##### CursoAmazon Web Services (AWS) - S3 - Fundamentos

[Conhecer o curso](https://www.treinaweb.com.br/curso/amazon-web-services-aws-simple-storage-service-s3-fundamentos)

## Características do Lambda

Agora que já conhecemos um pouco mais sobre Serveless, podemos discutir quais as principais características do Lambda.

Com o Lambda podemos construir aplicações baseadas em pequenas funções, com uma responsabilidade única iniciada a partir de eventos. Essa é a principal diferença com uma aplicação web, pois nosso código implementa somente o que é necessário para ser executado. Podemos por exemplo, responder a uma requisição HTTP, ou redimensionar uma imagem salva no [S3](https://www.treinaweb.com.br/blog/o-que-e-aws-s3/), ou processar uma mensagem enviada numa fila do SQS, com o mínimo de código possível.

Entretanto, para aproveitar de modo efetivo esse serviço, vamos levantar algumas considerações sobre o Lambda.

## Quais os benefícios do Lambda?

Ao desenvolver uma solução com Lambda, primeiramente temos que conhecer quais serão os benefícios que podemos observar:

- **Quantidade de código reduzida**: Ao contrário de uma aplicação web MVC, onde temos que configurar conexões com banco de dados, configurar rotas, entre outros, podemos ir direto ao ponto e executar só o que é necessário no Lambda. O gerenciamento de rotas, bem como conexões com o banco de dados, e outras configurações são delegados para outros serviços, como um API Gateway, e são configurados fora do seu código.
- **Escalabilidade instantânea**: Para os casos onde nossa função recebe um pico de acessos, é possível escalar automaticamente sua função para atender um número maior de clientes. Como a AWS é responsável por gerenciar nossa infraestrutura, podemos delegar essa responsabilidade sem precisar se preocupar alocar previamente mais servidores.
- **Sem cobrança de recursos ociosos**: Para soluções com tráfego pequeno ou pouco constante, temos um grande potencial economia, pois com o Lambda nós não precisamos pagar por recursos ociosos de uma EC2, mesmo com a menor máquina possível.

## Quando não utilizar Lambda?

Contudo existem algumas situações onde não é interessante utilizar Lambda. A primeira situação é rodar uma aplicação web tradicional. Você até consegue fazer isso, mapeando os eventos enviados com uma requisição web que sua aplicação utiliza, porém você estará subutilizando o potencial do Lambda, publicando uma aplicação completa dentro de uma única função e executando trechos de código que podem ser redundantes, como a configuração de rotas.

Processos de longa duração também não são recomendados. O tempo limite de execução de uma função é de 15 minutos. Isso pode acontecer ao processar um grande volume de dados de uma só vez. O ideal nesse caso é quebrar esse processo em partes menores, e executar somente uma unidade por função, ao invés de processar várias unidades de uma vez.

Uma função lambda também não tem acesso a um disco permanente. A manipulação de arquivos pelo lambda acontece em um disco efêmero e de baixa capacidade, tornando impossível manipular arquivos muito grandes numa função. Dessa forma é necessário recorrer a um serviço de armazenamento externo como o [S3](https://www.treinaweb.com.br/blog/o-que-e-aws-s3/).

Por fim, temos que considerar o vendor lock-in. Em outras palavras, ao desenvolver uma função lambda não será possível migrar o código para outro provedor no futuro. Para migrar o Lambda para Azure Functions, por exemplo, posteriormente você precisa reimplementar toda a lógica que trata os eventos e suas integrações com outros serviços. Praticamente, você irá criar uma nova função.

## Conclusão

Essa foi uma breve introdução sobre o AWS Lambda. Vimos aqui algumas vantagens e quando utilizar esse serviço que é bastante famoso na AWS.

Confira o curso AWS Lambda Fundamentos para conhecer com muito mais detalhes esse serviço.



![Amazon Web Services (AWS) - Lambda - Fundamentos](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/aws.svg)

##### CursoAmazon Web Services (AWS) - Lambda - Fundamentos

[Conhecer o curso](https://www.treinaweb.com.br/curso/amazon-web-services-aws-lambda-fundamentos)

Fiquem ligados e nos sigam nas nossas redes sociais, como [Twitter](https://twitter.com/treinaweb), [Instagram](https://www.instagram.com/treinaweb/), [Facebook](https://www.facebook.com/TreinaWeb/) e [LinkedIn](https://www.linkedin.com/company/treinaweb/). Assim que esse curso for lançado você saberá em primeira mão!

- [#AWS](https://www.treinaweb.com.br/blog/tag/aws)
- [#lambda](https://www.treinaweb.com.br/blog/tag/lambda)
- [#serveless](https://www.treinaweb.com.br/blog/tag/serveless)