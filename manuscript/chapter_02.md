# Cloud-native

O desafio de mover e otimizar a aplicação dentro do ambiente de nuvem a ponto de focar no seu negócio, como mencionado no capítulo anterior. É o sonho e o objetivo das organizações indiferente do seu tamanho. Nesse cenário um termo se tornou em voga: o cloud-native. Nesse capítulo, conversaremos um pouco sobre esse conceito e como isso impacta dentro da arquitetura da sua aplicação.

## Definição

A definição do termo cloud-native é improvável que chegamos num consenso nesse exato momento, principalmente, por que ele se tornou um conceito mais filosófico, mercadológico e principalmente subjetivo. Isso quer dizer que a depender da empresa, organização ou indivíduo que seja questionado com esse termo a resposta tende a ser diferente.

### Cloud-Enabled

É uma aplicação que foi conteinerizada e roda na cloud, mas que originalmente foi criada para rodar em ambiente tradicional, como por exemplo um data-center local, máquinas virtuais com cluster de servidores de aplicação tradicional. Essas aplicações podem ser categorizadas como *cloud-enabled* e têm maior consumo de recursos (cpu, memória, storage), em comparação a aplicações cloud-native.

Uma aplicação cloud-enabled passou por refatorações e ajustes para rodar em ambiente conteinerizado e também para suportar orquestração por plataformas como Kubernetes. Afinal de contas, não é mais o tradicional cluster de WildFly (a.k.a. JBoss EAP) ou GlassFish (Weblogic) clusterizados, que permitem que você use a rede ou sistema de arquivos a seu bel-prazer. Agora, esses serviços rodam em pods, em contêineres efêmeros.

Apesar dos "contras" de se possuir uma aplicação cloud-enabled, o custo ou esforço de se refatorar toda a aplicação não são viáveis. Desta forma, a aplicação pode rodar em cloud, mas não pode usufruir de todos os benefícios existentes em um ambiente de cloud.

> **INFO:** [Kubernetes](https://kubernetes.io/): É uma ferramenta open-source de orquestração de containers e trabalha muito bem com o [Docker](https://www.docker.com/). Atualmente, é a ferramenta mais popular na comunidade. Outros exemplos de ferramenta de orquestração de containers são Docker Swarm, Mesos e Amazon ECS.

Para entender melhor tudo o que uma aplicação cloud-enabled *não* é capaz de utilizar nativamente, vamos falar sobre o conceito cloud-native.

### Perspectivas sobre o conceito cloud-native

No momento da escrita deste livro, não há um consenso ou definição exata acerca do termo. Portanto, vejamos posicionamentos:

> "Cloud-native é uma abordagem para criar e executar aplicações que explora as vantagens do modelo de computação em nuvem. (...)"
>
> —[VMWare Tanzu (Pivotal)](https://tanzu.vmware.com/cloud-native)

> "Cloud-native é uma maneira diferente de pensar e raciocinar sobre sistemas de software. Ele incorpora os seguintes conceitos: alimentado por infraestrutura descartável, composta por limites, escala globalmente, adota a arquitetura descartável. (...)"
>
> — [Architecting Cloud Native Applications](https://www.amazon.com/Architecting-Cloud-Native-Applications-high-performing-ebook/dp/B07QTJ8WW8/ref=sr_1_4?keywords=cloud+native+applications&qid=1575059989&sr=8-4)

> "De maneira geral, “cloud-native” é uma abordagem para criar e executar aplicações que explora as vantagens do modelo de entrega de computação em nuvem. "Cloud-native" é sobre como as aplicações são criadas e implantadas, não onde. (...)"
>
> — [InfoWorld](https://www.infoworld.com/article/3281046/what-is-cloud-native-the-modern-way-to-develop-software.html)

> "As tecnologias cloud-native capacitam as empresas a criar e executar aplicações escaláveis em ambientes modernos e dinâmicos, como públicos, privados e nuvens híbridas. Containers, service meshes, microservices, infraestrutura imutável e APIs declarativas exemplificam essa abordagem. (...) "
>
> — [Cloud-Native Computing Foundation](https://www.cncf.io/)

> 'Cloud native' é um adjetivo que descreve as aplicações, arquiteturas, plataformas/infraestrutura e processos que, juntos, tornam o trabalho *econômico* de uma forma que nos permite melhorar nossa capacidade de responder rapidamente às mudanças e reduzir a imprevisibilidade
>
> — [Christian Posta](https://www.infoq.com/articles/cloud-native-panel/)

> "Um conjunto de boas práticas para otimizar uma aplicação na nuvem por meio de: conteinerização, orquestração e automação."
>
> — [Otávio Santana](https://twitter.com/otaviojava)

Além dos conceitos acima, um conjunto de padrões bem recebido pela comunidade é o [12-factor](https://12factor.net/). As excelentes práticas de arquitetura de software sugeridas nessa metodologia originam do livro [Patterns of Enterprise Application Architecture, escrito por Martin Fowler e David Rice](https://books.google.com.br/books/about/Patterns_of_enterprise_application_archi.html?id=FyWZt5DdvFkC&redir_esc=y). Tendo em mente que o livro foi publicado em 2003, tempos em que ainda não se falava em "cloud-native", podemos considerar que, ao adotar os conceitos do 12-factor, você estará não apenas criando uma aplicação cloud-native, mas também implementando boas práticas arquiteturais e culturais no desenvolvimento e entrega de software.

> **TIP**: Nomes de projetos que serão detalhados a seguir podem evoluir e mudar com o tempo. Porém as definições e padrões esperados de uma aplicação cloud-native permanecerão. Portanto, recomendamos a leitura das referências citadas e aprofundamento no entendimento do conceito.

### Capabilities for cloud

Veja alguns dos recursos que estão disponíveis e são comumente utilizados em suas aplicações que são concebidas para rodar na cloud:

- Gerência de configurações (Configuration Management)
- API Management
- Scheduling (of workloads)
- Distributed Tracing
- Service Security
- Centralized Metrics
- Auto Scaling / Self healing
- Service Discovery and Load Balancing
- Centralized Logging

## Java e sua jornada de mais de vinte e cinco anos

### Evoluções JVM
### Especificação vs Implementação
### Quais as diferenças entre JavaEE e JakartaEE?
### Microprofile: a virada de jogo para o Java
### O que é compilação nativa?
