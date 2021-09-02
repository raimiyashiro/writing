# Quality Assurance on Pipelines

## Introdução

> Olá, sejam **todos** muito bem-vindos. Nesta pequena demonstração, falaremos um pouco sobre Garantia de Qualidade em Pipelines.

- O que são Pipelines?
> No contexto DevOps, pipelines são ferramentas ou **pacotes de ferramentas** (...) => que agilizam o processo de integração e entrega contínua de software. Uma Pipeline faz o meio-campo entre o código **em si**, normalmente armazenado em algum repositório Git, e a sua parada final, como um ambiente de produção ou desenvolvimento hospedado na Cloud.

* IDEIA: explicar DevOps entre dev e infra, code-dev ; pipe-devops ; environment-infra

- CI & CD?
> O nome Pipeline, que significa literalmente "cano" ou "tubo", é frequentemente substituído por Esteira DevOps ou, mais assertivamente, Esteira de CI & CD.
> Estes dois termos significam, respectivamente, "Integração Contínua" e "Entrega Contínua" ou mesmo "Implantação Contínua". Existe uma diferença bem clara entre uma esteira de CD e uma de CI, e a própria nomenclatura nos permite raciocinar da seguinte maneira:
> Uma esteira de Integração Contínua é responsável por unir todas as dependências relacionadas ao software, desde a instalação de pacotes até o build. Normalmente, uma esteira de CI é disparada quando um "commit" ou um "push" chega ao servidor git remoto, como o próprio Github. Esse "gatilho" que inicia a esteira de CI tem o nome de Trigger. Em resumo, a Integração contínua é responsável pelas primeiras fases desse nosso "tubo" ou Pipeline: identificar o código novo que foi empurrado até o repositório > instalar as dependências necessárias para o build ou a compilação > integrar serviços adicionais, como veremos mais a frente, e finalmente, deixar esse novo software pronto para ser entregue ou implantado em algum lugar.
> Apesar de todas essas etapas, ainda falta uma coisa. Como eu disse anteriormente, uma Pipeline faz a ponte entre o código e o ambiente ao qual o mesmo está destinado. Isso significa que uma Pipeline é responsável inclusive pela entrega desse novo código aos seus usuários finais. É aqui que começa a fase de entrega ou implantação contínua, que consiste basicamente em entregar um software pronto, já compilado e tudo mais, ao seu ambiente final, por exemplo: www.minha-webapp.com.br. Então, quando começamos a falar de hospedagem, implantação, ambientes produtivos ou de desenvolvimento, a entidade responsável pela execução automatizada desses processos é uma Esteira de CD.

- Final da Introdução
> E se a explicação teórica parece um tanto nebulosa, não se preocupa! Nós veremos na prática o funcionamento de uma Pipeline em alguns momentos. O importante é ter ao menos uma certa noção de que os processos de CI e CD constituem esse "tubo", a Pipeline, que leva o código de um software até o servidor onde ele ficará hospedado.

## Desenvolvimento
> Como mencionei no começo do vídeo, nessa demonstração falaremos não só sobre Pipelines, apesar da vastidão de coisas que poderíamos abordar acerca desse assunto. Mas falaremos também sobre Garantia de Qualidade, uma peça que não pode faltar na composição de qualquer projeto de software.
 
- O que é Garantia de Qualidade?
> Brevemente, é um caminho de prevenir erros em "produtos manufaturados". No escopo do desenvolvimento de software, uma linha de código ou uma variável toma o papel de “produto manufaturado”, pois são manualmente concebidos, na maior parte dos casos, por um desenvolvedor ou um arquiteto de software, e entregues para o uso de algum público ou cliente específico.	É aí que surge um problema: erros. É da natureza humana errar, e nós erramos feio! Quem nunca usou o "this" da maneira errada que atire a primeira pedra!

> E é justamente visando resolver ou diminuir esse problema dos nossos erros que surgem ferramentas de inspeção de código como o Sonar. O Sonar vem para "garantir" a qualidade do software entregue, ou pelo menos diminuir a sua suscetibilidade à falhas. E essa ferramenta o faz por diversos meios, principalmente através da busca de codesmells (ou, num português bem claro, "porquices") num código, imprecisões, incoerências e pontos de segurança graves ou moderados. Em alguns cenários, o Sonar atua literalmente como um "blocker" na subida de um código. Se o software que está prestes a ser entregue não **passa** pela inspeção do Sonar com suas respectivas métricas, o deploy pode mesmo ser cancelado, a fim de evitar bugs, vulnerabilidades e comportamentos indesejados naquele produto.

(...) vamos fazer uma breve tangente que, de um modo geral, estabelece uma conexão muito formidável entre o mundo DevOps e o mundo do desenvolvimento de software: o TDD, ou Test-Driven Development”




