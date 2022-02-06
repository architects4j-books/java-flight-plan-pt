# Cloud

Ao longo do tempo vemos o termo cloud tomando cada vez mais formato e espaço dentro não apenas na área de tecnologia, mas dentro também da cultura popular. Mas de fato, o que significa cloud em termo de impacto tecnológico e qual a motivação dele ser tão crucial no nosso dia a dia. O objetivo desse capítulo é falar um pouco do seu histórico além da sua importância como arquiteto de software.

## Por que cloud?

O primeiro e mais importante passo dessa jornada é a sua motivação. Baseado no livro do [Simon Sinek](https://simonsinek.com/) [e o seu círculo dourado](https://simonsinek.com/product/start-with-why/?ref=home). Falaremos o porquê deveríamos conhecer e explorar o ambiente de nuvem.

Ao acompanhar a história da engenharia de software e sua metodologia sempre vimos a necessidade de uma entrega mais rápida para se obter constante feedback, principalmente, falhar rápido. Os softwares vem se tornando cada vez mais complexo, envolvendo um número maior de especialistas, logo, mais caro. Assim, garantir que o software está na direção certa não é apenas o receio da perda to time to market, mas a garantia que o investimento está indo na direção correta.

O desfecho dessa história é o que já conhecemos. Aos poucos o modelo cascasta ou waterfall, do qual esperamos meses ou anos para o primeiro feedback do usuário, foi dando espaço é um modelo que foca em pequenas entregas e estar mais apto a mudanças garantido com que o usuário esteja o mais próximo possível do time de desenvolvimento.

O [manifesto ágil](https://agilemanifesto.org/) se tornou uma grande revolução, principalmente, entendo a importância de ser apto a mudanças de acordo a necessidade do cliente. Além de entender que o cliente precisa fazer parte do time e não ser apenas um personagem distante no processo do desenvolvimento.

Colocar o usuário próximo do time de desenvolvimento resultou em novas formas, até mesmo, de escrever o código. Por exemplo, diversas literaturas e metodologias nasceram oriundos dessa metodologia. Podemos citar em destaque, por exemplo, o [DDD](https://www.amazon.com/dp/0321125215) que frisa a importância do código refletir diretamente dentro do negócio.

A integração com o desenvolvimento foi uma excelente experiência, porém, não era suficiente. Afinal, ter o software pronto e não em produção é apenas meio caminho andado. A solução é trazer mais áreas para dentro do mesmo time focando sempre em uma entrega mais rápida para o usuário. Com isso, nasceu a cultura [DevOps](https://aws.amazon.com/devops/what-is-devops/) cujo foco é uma maior integração entre o time de desenvolvimento com o time de operação. 

A cultura DevOps resultou em diversas boas práticas como [Continuous Integration](https://www.amazon.com/dp/0321336380) para melhorar a qualidade e a redução de riscos. E a consequência foi a inclusão de mais culturas de integração como [DevSecOps](https://dzone.com/articles/starting-with-information-security-how-to-avoid-he).

Mas então, onde entra a [cloud](https://www.nist.gov/news-events/news/2011/10/final-version-nist-cloud-computing-definition-published)? A computação em nuvem veio e se tornou popular devido a sua facilidade em entregar o software. Ou seja, cloud não é apenas o servidor de outra pessoa, mas o problema de outra pessoa. É quando delegamos a gestão de hardware, operações ou todo o processo de desenvolvimento de software para outra empresa com o intuito principal de realizar entregas mais rápidas.

## Por que a adoção é crítica para o sucesso da organização?



Simplificando drasticamente a definição de cloud para simplesmente: o problema de outra pessoa. Cloud é uma excelente opção para delegar todas as operações que não fazem parte do core da sua organização.



Pensando tecnologia como uma escolha estratégica para um negócio e parafraseando o livro [Learning Domain-Driven Design](https://www.amazon.com/dp/1098100131). É crítico colocar um esforço naquilo que será um diferencial para o negócio ou seja o core ao invés de recursos que apoiam. 

![Descrição e relação da complexidade e o diferencial](images/chapter_01_01.png)

Com isso em mente, faz sentido para uma organização manter e organizar o seu próprio hardware ao redor do mundo ao invés de pagar uma organização?



Certamente, muitos dos leitores aqui conhecem a clássica comparação entre pizza e serviço cloud, principalmente, na perspectiva do usuário.



Com isso em mente, faz sentido para uma organização manter e organizar o seu próprio hardware ao redor do mundo ao invés de pagar uma organização?



Certamente, muitos dos leitores aqui conhecem a clássica comparação entre pizza e [serviço cloud, principalmente, na perspectiva do usuário definido pelo Albert Barron](https://www.linkedin.com/pulse/20140730172610-9679881-pizza-as-a-service/).



Porém, focando em organização, ou seja, ao invés do usuário focaremos na pizzaria em si.



No primeiro cenário, temos uma pizzaria do qual ela é responsável por todo o processo:

- Pela fazenda, colheita de trigo, queijo
- Logística dos materiais entre a fazenda e a pizzaria
- A criação da pizza (o core do meu negócio)
- A entrega da pizza na casa dos usuários



Esse primeiro também é o pior cenário ao negócio, uma vez que como pizzaria se gasta muita carga cognitiva em diversos processos além da parte mais importante que é a confecção da pizza. 



Esse ponto se torna ainda mais explícito para pequenas empresas ou com recursos limitados, afinal, terá que gastar os poucos recursos em diversos fatores além do seu diferencial como pizzaria.



Caminhando para o outro extremo, do qual essa mesma pizzaria é responsável apenas pela criação da pizza e todo o restante é terceirizado. Garantimos um maior investimento ou foco no que é importante para a organização. 



Dessa forma, todo o problema de logística, praga nas fazendas, problemas ambientais, dentre outros fatores não impactarão diretamente o seu negócio.



Em resumo, a maior motivação de cloud é o poder de delegar tudo aquilo que não corresponde o core-business do negócio e partir para a parte mais importante do negócio. Ao tempo de não deixar a qualidade dos serviços tercerizados.

## Entenda os diversos serviços gerenciados

Quando falamos de recursos e serviços de nuvem, novamente, usando o nosso princípio tudo dependerá do quê você deseja delegar de algum nível. 

Como toda escolha que passa no ponto arquitetural é sempre importante que existe o trade-off. Por exemplo, ao passo que uma maior abstração nos garante um menor risco isso pode fazer com que o preço seja maior além existir um cloud vendor lock-in dentro da sua pilha tecnológica a ponto de ser difícil sair desse provider a medida que você utiliza esse recurso exclusivo.



Salientando o que [Neal Ford](https://twitter.com/neal4d) disse em seu livro sobre [os fundamentos de arquitetura](https://www.amazon.com/dp/B08X8H15BW/). O papel principal de um arquiteto é entender e fazer um bom balanço dentre do possível, analisando os trade-offs.



Com base nisso definimos o seguinte diagrama do qual descutiremos melhor dentro desse capítulo.

KARINA PRECISAMOS FECHAR OS QUADRANTES AQUI COM UMA IMAGEM, PULAREI ESSE PONTO



### IaaS, PaaS,SaaS

O primeiro ponto dentro da nossa jornada e na perspectiva de serviço dentro de cloud. Estão os três serviços mais estáveis no sentido de que não existem muitas discussões e variações sobre a sua definição. Inclusive, tendo seu conceito explorado dentro de um grande e forte instituto de normalização como o [NIST](https://www.nist.gov/).

Numa leitura de abstração, podemos pensar que cada serviço trabalha na abstração de hardware, operação e o software em si.



No **IaaS** ou instructure as service, estamos delegando o hardware. Em outras palavras, nós como organização não nos preocupamos com a gestão do servidor, energia, alugar um local para ter os servidores, refrigeração dos mesmos. Fazendo que o maior cliente ou público-alvo seja os engenheiros que tenham que lidar com operações como o SRE, por exemplo.



No lado do **PaaS** ou platform as a service, damos um próximo passo na abstração. De modo que, além do hardware também delegamos toda a parte de operações. Com isso, o foco maior será com a criação de código e todo o restante será responsabilidade de outra pessoa. No geral, o público-alvo ou os seus maiores usuários são desenvolvedores ou engenheiros focados na entrega de código em si.



No último e no maior passo de abração de nuvem como serviço temos **SaaS** ou software as a service. É a última camada de abstração do qual além de se delegar as duas camadas anteriores, hardware e operações, também se delega a codificação também. De modo que o público-alvo são usuários que não precisam ter nenhum conhecimento de prévio de computação.



Recapitulando:

| Tipo de serviço | O problema de outra pessoa                    | Exemplos                                                    |
| --------------- | --------------------------------------------- | ----------------------------------------------------------- |
| IaaS            | hardware                                      | Configuração de servidor, energia elétrica, refrigeração    |
| PaaS            | O anterior além dos  os detalhes de operações | Atualização de sistema operacional, firewall, backup        |
| SaaS            | Todos os anterioes além do software           | Codificação, escolha de linguagem, definição de arquitetura |



### CaaS

### Managed Application Services
