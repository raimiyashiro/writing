# Quality Assurance on Pipelines

## Introdução

> Olá, sejam muito bem-vindos. Nesta pequena demonstração, falaremos um pouco sobre Garantia de Qualidade em Pipelines. Para dar contexto ao assunto, vamos começar com alguns conceitos básicos.

- O que são Pipelines?
> No contexto DevOps, pipelines são ferramentas ou pacotes de ferramentas que agilizam o processo de integração e entrega de software. Uma Pipeline faz o meio-campo entre o código em si, normalmente armazenado em um repositório Git, e a sua parada final, ou seja um ambiente de produção ou desenvolvimento hospedado na Cloud.
- CI & CD?
> O nome Pipeline, que significa literalmente "cano" ou "tubo", é frequentemente substituído por Esteira DevOps ou, mais assertivamente, Esteira de CI & CD.
> Estes dois termos significam, respectivamente, "Integração Contínua" e "Entrega Contínua" ou mesmo "Implantação Contínua". Existe uma diferença bem clara entre uma esteira de CD e uma de CI, e a própria nomenclatura nos permite raciocinar da seguinte maneira:
> Uma esteira de Integração Contínua é responsável por unir todas as dependências desde o commit até o build. Em outras palavras, uma esteira de CI, geralmente disparada por um "commit" ou um "push", o qual chamamos de Trigger, é responsável pelas etapas iniciais da Pipeline: ler o código do repositório > instalar as dependências necessárias > integrar serviços adicionais, como veremos mais a frente, e finalmente, rodar o build do software recebido.
> Apesar de todas essas etapas, ainda falta uma coisa. Como eu disse anteriormente, uma Pipeline faz a ponte entre o código e o ambiente ao qual o mesmo está destinado. Isso significa que uma Pipeline é responsável inclusive pela entrega desse novo código aos seus usuários finais. A partir desse momento, não estamos mais falando de integração, mas sim de entrega e implantação. Isso define bem a responsabilidade de uma Esteira de CD, que consiste basicamente em entregar um software pronto, já compilado e tudo mais, ao seu ambiente público, por exemplo: www.minha-webapp.com.br

- Final da Introdução
> E se a explicação teórica parece um tanto nebulosa, não se preocupa! Nós veremos na prática o funcionamento de uma Pipeline em alguns momentos. O importante é ter ao menos uma certa noção de que os processos de CI e CD constituem esse "tubo", a Pipeline, que leva o código de um software até o servidor onde ele ficará hospedado.

## Desenvolvimento
> Como mencionei no começo do vídeo, nessa demonstração falaremos não só sobre Pipelines, apesar da vastidão de coisas que poderíamos falar acerca desse assunto. Porém, falaremos também sobre Garantia de Qualidade, uma peça que não pode faltar na composição de qualquer projeto de software.
 
- O que é Garantia de Qualidade?
> Brevemente, é um caminho de prevenir erros em produtos manufaturados. No escopo do desenvolvimento de software, uma linha de código ou uma variável toma o papel de “produto manufaturado”, pois são manualmente concebidos, na maior parte dos casos, por um desenvolvedor ou um arquiteto de software, e entregues para o uso de algum público ou cliente específico.	

> Entre outras práticas, para "garantir" a qualidade do software entregue, surgem ferramentas de inspeção de código como o Sonar, que o faz por diversos meios, principalmente através da busca de codesmells (ou, num português bem claro, "porquices") num código. Em alguns cenários, o Sonar atua literalmente como um "blocker" na subida de um código. Se o software que está prestes a ser entregue não passa pela inspeção e suas respectivas métricas, o deploy pode mesmo ser cancelado, a fim de evitar bugs, vulnerabilidades e comportamentos indesejados naquele produto.

(...) vamos fazer uma breve tangente que, de um modo geral, estabelece uma conexão muito formidável entre o mundo DevOps e o mundo do desenvolvimento de software: o TDD, ou Test-Driven Development”




