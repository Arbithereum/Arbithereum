Editando_

PS. neste momento o modelo está em "rascunho".
Imagem com diagrama do projeto https://scontent-gru2-1.xx.fbcdn.net/hphotos-xtf1/t31.0-8/s960x960/12633715_10209067863563857_8838783255422100994_o.jpg


#####Tópicos a serem adicionados e resolvidos: <br>
- Benefícios do negócio <br>
- Ramificação técnica <br>
- Problemas de colisão lógica da solução (leis estatais de um ou mais países) <br>
- Solução de colisões <br>
- Teorias economicas aplicáveis <br>


#Resumo

Todo o projeto é feito na plataforma Ethereum, porém, a ideia em si, pode ser aplicada a qualquer plataforma que crie Dapp (como Dash) ou mesmo copiando projetos como Bitcoin e iniciando uma plataforma em si. O que requer mais recurso e tempo. Ethereum não requer tanto recurso. Lembre que esse projeto é baseado em licença GNU.

Está é uma proposta levemente complexa de ser efetivada, não por conta de codificação, mas de problemas lógicos de colisão com leis de vários países. Porém, os resultados da ideia para o atual senário brasileiro ou de qualquer outro país (Venezuela? Paises pobres da Africa?) são de grande utilidade e vem a calhar. Eliminando até o uso de papéis em modelos parecidos (como Boleto Bancário).

Continuando. Locais onde pessoas não tem acesso a tecnologia, mas entendem como funciona um "check", "boleto", "Western Union" ou "Moneygram" por exemplo. Iria se beneficiar do Arbithereum. 

A ideia partiu de problemas que exchanges brasileiras enfrentavam ao ter suas contas bancárias canceladas. Tanto clientes como exchanges eram punidos com cancelamento de contas. O modelo trás primordialmente duas soluções. A "brincadeira" de arbitragem entre exchanges e a possibilidade de um sistema mais eficiente que "boleto bancário". 

Onde em um cenário em que bancos passam a negar a abertura de contas de clientes e exchanges, que compram e vendem Bitcoins e outras Altcoins, favorece-os de forma justa e descentralizada. O Arbithereum viria para tomar o papel que o banco fazia e agora se nega a fazer por vontade própria, por decisões sem base lógica. Até o momento nem um representante do governo brasileiro abriu qualquer restrição, regulação ou proibição do uso de Bitcoins. Então não faria sentido um banco punir seus clientes assim. Por isso o Arbithereum se faz necessário.

As estruturas de taxas seriam elaboradas pelos contratantes em suas próprias plataformas. Mas como o Arbithereum utiliza uma plataforma Ethereum, há taxas próprias a se pagar por transação. Então o contratante deve fazer suas "contas" para decidir quanto cobrar de seus clientes por "sub-contratos".


#Estrutura incial


#####Contrato de arbitragem
É um contrato "superior", o sistema só funciona se houve interesse de instituições, como exchanges por exemplo. Através dele é possível criar Sub-contratos. Também é aceito contrato de arbitragem feito por autônomos. Basta ele inserir Bitcoins ao contrato dele. (Seria interessante criar um sistema de certificação para instituições permitirem "sidechains" de autônomos e outras instituições se comuniquem com a blockchain deles. Assim, quando a instituição achar que deve dar "baixa" no certificado. Ele pode "cortar relações" com a sidechain do "autônomo" ou instituição. A ideia é permitir uma relação de parceirias mais facilmente através do sistema. Com garantias que tanto "A" como "B" e "C" achem justa. A justiça seria feita pelo smartcontract normalmente. Podemos restringir essa regra para contratos que o sistema pode considerar de "risco".)

Um contrato de arbitragem é nada mais que um código inteligente que tem uma "blockchain" que identifica a "blockchain" de terceiros como uma "sidechain" ligada a dele. Informações de entrada e saída são inseridas na Blockchain da instituição "A" sobre a instituição "B" e tais blockchains conversam entre si pelo smartcontract.

(Podemos avaliar se os contratos superiores terão "validade" de tempo, onde a instituição deve refazer um contrato e os créditos e depósitos são repassados para esse novo contrato. Que pode ser um cancelamento de contrato)

Um cancelamento de contrato vai automaticamente pagar todos os débitos. E se preciso consumir o "seguro" dos 20% de bitcoins que ficam retidos e inutilizados para contratos.


#####Sub-contrato de arbitragem
É um contrato que age como uma ordem de pagamento que vai para a instituição destinatária. Os valores enviados ficam "retidos" pelo contrato. Podendo a isntituição "A" fechar o contrato informando que a instituição "B" lhe pagou em espécie os valores devidos. Ou, pode optar pelo padrão que é compensado dentro do próprio sistema.

#####Sub-contrato de ordem de pagamento via parceiros de instituição
É um contrato que age como uma ordem de pagamento que vai para a parceiros da instituição. Os valores enviados ficam "retidos" pelo contrato até o destinatário comparecer com o QR-Code que pode liberar essa ordem de pagamento. 

#####Sub-contrato de ordem de pagamento via Arbithereum.
É um contrato que age como uma ordem de pagamento que vai via Arbithereum que não são ligados a uma instituição especifica, são autonomos. Os valores enviados ficam "retidos" pelo contrato até o destinatário comparecer com o QR-Code que pode liberar essa ordem de pagamento. Podemos implementar também uma "autenticação em dois passos" para ordem de pagamento.

#####Sub-contrato de depósito via parceiros de instituição.
É um contrato que age como uma depósito que vai para um instituição que aceita depósitos desta origem (ele pode ser parceiro ou autonomo). Os valores depositados ficam "retidos" pelo contrato até o destinatário (no caso uma instituição, ex: Exchange) der baixa com o QR-Code que pode liberar essa ordem de pagamento. Ao faze isso ele reconhece que houve o depósito de fato. E o sistema credita automaticamente. Erros humanos são resolvidos entre as partes.  

##Mais detalhes

###Contrato de arbitragem:

O contrato exige que o contratante adicione dados dele mesmo. CNPJ é um exemplo. Para motivos de verificação o CNPJ deve estar em um PDF registrado em sites como "originalmy" e haverá um campo no contrato onde o contratante deve inserir os dados de Hash gerado pelo certificado do site. O PDF deve está disponível o tempo todo*. Pode ser solicitado Website com "trigger" verificando se o site responde e está "online". Seria necessário uma API, e também verificar se a plataforma Ethereum pode gerar triggers do tipo.

O contrato exige o depósito de uma quantidade de Bitcoins. A quantidade vai definir o "limite" de quanto (em reais) ele pode "emitir" em contratos para seus clientes em sua própria plataforma.

Haverá outras regras a ser elaborada de acordo com novas necessidades.

*Talvez seja necessário desenvolver um "trigger" para que o contrato verifique se o PDF está disponível. Ou donos de contratos de arbitragem (ou seja, outras exchanges) pondem "acionar" uma votação para cobrar do contratante a disponibilidade do contrato dele. O contratante não exibir defesa será considerado quebra de contrato. Podendo haver sanções como por exemplo congelamento dos depósitos que estão no contrato. Ou solver todos os débitos e devolver o restante dos Bitcoins retidos no contrato.

###Sub-contrato de arbitragem:

É um contrato que só o cliente da instituição (entidade? exchange? banco? instituição financeira?) pode gerar através do sistema da instituição. Esse contrato liga o cliente e a exchange ao contrato especifico. E ele será debitado posteriormente em nome da instituição que lhe é destinado.

A instituição deve inserir espaços de entrada de dados ou gerar automaticamente o preenchimento dos mesmos que são:
* Endereço do contrato destinatário. (exemplo Exchange "B")
* Endereço do sub-contrato destinatário. (ex: Carteira "ExchangeBtxyiaskspleeixcmlpkwuiiksllaç")
* Endereço do sub-contrato do requerente. (Carteira de quem está enviando dinheiro para outra instituição preenchido automaticamente pela API)
* Endereço da instituição (que irá ser preenchido automaticamente pela API)
* A quantidade em reais a ser enviada.
* Dados pessoais do cliente para avaliação da instituição de destino.
* Um campo contendo URL de um jpeg contendo preferencialmente a foto do cliente.
* CPF do cliente requerente. (pode ser preenchido pela API da instituição que já o tem em cadastro)

###Sub-contrato de ordem de pagamento via parceiros de instituição:

É um contrato que só o cliente da instituição pode gerar através do sistema da instituição. Esse contrato liga o cliente, a exchange e um empreendedor terceiro ao contrato especifico que é destinado a quem tem o QR-Code que libera o contrato. E ele será debitado posteriormente em nome do empreendedor (terceiros) que lhe é autorizado pela exchange e tem conta na mesma. E a exchange é responsável por repassar o pagamento ao empreendedor.

A instituição deve inserir espaços de entrada de dados ou gerar automaticamente o preenchimento dos mesmos que são:
* Endereço do contrato destinatário. (exemplo Exchange "B")
* Endereço do sub-contrato destinatário. (ex: Carteira "ExchangeBtxyiaskspleeixcmlpkwuiiksllaç")
* Endereço do sub-contrato do requerente. (Carteira de quem está enviando dinheiro para outra instituição preenchido automaticamente pela API)
* Endereço da instituição (que irá ser preenchido automaticamente pela API)
* A quantidade em reais a ser enviada.
* Dados pessoais do cliente para avaliação da instituição de destino.
* Um campo contendo URL de um jpeg contendo preferencialmente a foto do cliente.
* CPF do cliente requerente. (pode ser preenchido pela API da instituição que já o tem em cadastro)

###Sub-contrato de ordem de pagamento via Arbithereum:

É um contrato que só o cliente da instituição pode gerar através do sistema da instituição. Esse contrato liga o cliente e a exchange ao contrato especifico. E ele será debitado posteriormente em nome do empreendedor (terceiros) que não é ligado a alguma exchange. E a Arbithereum é responsável por repassar o pagamento ao empreendedor via os mesmo modelo de contratos inteligentes.

A instituição deve inserir espaços de entrada de dados ou gerar automaticamente o preenchimento dos mesmos que são:
* Endereço do contrato destinatário. (exemplo Exchange "B")
* Endereço do sub-contrato destinatário. (ex: Carteira "ExchangeBtxyiaskspleeixcmlpkwuiiksllaç")
* Endereço do sub-contrato do requerente. (Carteira de quem está enviando dinheiro para outra instituição preenchido automaticamente pela API)
* Endereço da instituição (que irá ser preenchido automaticamente pela API)
* A quantidade em reais a ser enviada.
* Dados pessoais do cliente para avaliação da instituição de destino.
* Um campo contendo URL de um jpeg contendo preferencialmente a foto do cliente.
* CPF do cliente requerente. (pode ser preenchido pela API da instituição que já o tem em cadastro)

###Sub-contrato de depósito via parceiros de instituição.

É um contrato que só o parceiro da instituição (entidade? exchange? banco? instituição financeira?) pode gerar através do sistema da instituição. Esse contrato liga o parceito e a exchange ao contrato especifico. E ele será debitado posteriormente em nome do cliente da instituição devidamente informado, que então lhe é destinado.

A instituição deve inserir espaços de entrada de dados ou gerar automaticamente o preenchimento dos mesmos que são:
* Endereço do contrato destinatário. (exemplo Exchange "B")
* Endereço do sub-contrato destinatário. (ex: Carteira "ExchangeBtxyiaskspleeixcmlpkwuiiksllaç")
* Endereço do sub-contrato do requerente. (Carteira de quem está enviando dinheiro para outra instituição preenchido automaticamente pela API)
* Endereço da instituição (que irá ser preenchido automaticamente pela API)
* A quantidade em reais a ser enviada.
* Dados pessoais do cliente para avaliação da instituição de destino.
* Um campo contendo URL de um jpeg contendo preferencialmente a foto do cliente.
* CPF do cliente requerente. (pode ser preenchido pela API da instituição que já o tem em cadastro)


Obrigado pelo seu tempo!
