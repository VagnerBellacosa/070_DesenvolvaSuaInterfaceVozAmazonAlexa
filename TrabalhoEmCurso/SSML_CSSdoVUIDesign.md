# SSML, o CSS do VUI design.

[![Billy Garcia](https://miro.medium.com/fit/c/96/96/1*MBcYVSPMiox8pYQXAW7nDA.jpeg)](https://medium.com/@billygarcia_34772?source=post_page-----dc31e5b48b93--------------------------------)

[Billy Garcia](https://medium.com/@billygarcia_34772?source=post_page-----dc31e5b48b93--------------------------------)Follow

[Aug 22, 2019](https://medium.com/botsbrasil/ssml-o-css-do-vui-design-dc31e5b48b93?source=post_page-----dc31e5b48b93--------------------------------) · 5 min read













Este não é um artigo técnico, mas falando de nerd para nerd, vou assumir que você conheça o básico do *HTML* e entenda a importância do *CSS* como guia do design de projetos web. Na prática, é nesse arquivo externo que definimos coisas que estão simultaneamente ligadas a estética, acessibilidade e produtividade de todo o projeto. Este arquivo de estilos é responsável pela experiência de uso de quem acessa e por aumentar a performance de quem, por exemplo, desenvolve um website. Muitas coisas boas podem acontecer da combinação correta desses dois arquivos.

Ainda estamos na infância das interfaces e *gadgets* orientados por comandos de voz, e justamente por isso, dispor de alguns truques que possam refinar ou melhorar a experiência de uso da sua *skill* pode fazer toda a diferença no momento de publicar para Alexa ou Google Assistant.
Uma das maneiras de fazer a diferença é usando as marcações *SSML*, ou, *Speech Synthesis Markup Language* para dar mais dimensão e profundidade em projetos conversacionais.

Assim como o *CSS* serve de guia de estilo para o *HTML* de um projeto web, o *SSML* vai possibilitar que você [edite a voz sintética do seu projeto *VUI*](https://developers.google.com/actions/reference/ssml), de maneira que pareça mais natural ou, caso seja sua intenção, semelhante a voz de um *zombie* para um *voice game.*

Acredite; estamos dando pouco valor a questões como velocidade, tom de voz e pausas dramáticas quando o assunto são *skills* para *gadgets* conversacionais, e isso já foi estudado no começo da década de 70.

# Mehrabian, prosódias e SSML

Albert Mehrabian, em seu livro [*Mensagens Secretas* de 1971](https://www.amazon.com/Silent-messages-Albert-Mehrabian/dp/0534000592), citou pela primeira vez um estudo que apontava a voz como responsável por [apenas 7% de uma mensagem, deixando os outros 93% restantes sob responsabilidade de expressões faciais, movimentos corporais e outras prosódia](https://e-edu.nbu.bg/pluginfile.php/855150/mod_resource/content/1/Albert-Mehrabian - Silent Messages 1971 - red.size.pdf)s, que são as funções linguísticas associadas a entonação, ritmo e tonalidade da voz humana.

O uso do *SSML* é recomendado pelo W3C e suas marcações são baseadas numa mistura de *JSML* — *Java Speech Markup Language* — e *XML*. Essas marcações podem alterar volume, duração, *pitch* e outros aspectos da fala sintética diretamente no código da *skill* e vão funcionar de maneiras diferentes na Alexa, Google Assistant, Watson ou Cortana.

O cérebro humano, sempre que identifica um novo interlocutor, busca preencher algumas lacunas de informação para entender de que maneira deve “catalogar” esse novo contato na nossa “agenda cerebral”. As informações que não estiverem disponíveis, como no caso de uma voz no rádio, serão preenchidas por dados que nosso cérebro entenda como “normais”— condição conhecida como Defeito do Ventríloco.

O Defeito do Ventríloco já foi citado em diversas pesquisas como origem de vieses machistas ou racistas em projetos de IA, e justamente em consequência disso é que se torna fundamental a desconstrução de “verdades” como as que assumimos ao criar uma grande maioria de assistentes femininos que estão ligados diretamente ao papel de subserviência.

# Joshua Davis e os sentimentos do IBM Watson

Criamos personas para dar vida a quase todo o tipo de interface interativa, usando avatares e nomes na esperança que os usuários tenham uma experiência mais confortável e personalizada, engajando mais e talvez consumindo melhor. Mas numa interface de voz com suporte limitado a imagens, como é o caso do *Echo Spot*, como fornecer essas informações extras?

Uma das experiências mais relevantes já criadas para o uso da persona numa plartaforma "*voice first*", foi a participação do IBM Watson num episódio especial do programa americano Jeopardy.

Aos 2m11seg, Joshua Davis, [CEO da Praystation](https://joshuadavis.com/IBM-Watson), demonstra como [criou um sistema de partículas capaz de reagir as emoções das respostas](https://www.fastcompany.com/1663236/joshua-davis-creates-the-face-of-watson-ibms-jeopardy-supercomputer). Impressiona a enorme quantidade de variáveis pela qual cada emoção pode ser representada e de que maneira essas emoções podem influenciar a voz.

2m11s Joshua Davis explica o processo criativo por trás do projeto The Face of Watson.

![img](https://miro.medium.com/max/60/1*BB_0yVQ8QVJ6tNNBM7cSPA.jpeg?q=20)

![img]()

O caminho que as emoções podem percorrer entre um sentimento e outro demonstrado em fluxo.

![img](https://miro.medium.com/max/60/1*3gqyzF3wGttm7tRe0FOuFA.jpeg?q=20)

![img](https://miro.medium.com/max/630/1*3gqyzF3wGttm7tRe0FOuFA.jpeg)

A antecipação da derrota.

![img](https://miro.medium.com/max/60/1*Mk7WniImKzhAwn3uF9VXhA.jpeg?q=20)

![img](https://miro.medium.com/max/630/1*Mk7WniImKzhAwn3uF9VXhA.jpeg)

A excitação da vitória.

# Áudios, poesias e prosódias

A utilização de áudios pode ser facilmente implementada na sua *skill* utilizando marcadores *SSML* e costumam enriquecer muito a experiência de uso, para isto basta habilitar a edição de código e utilizar o marcador ***<prosody>\*** acompanhado por ***Rate\***, ***Pitch\*** ou ***volume\***.
Com a utilização combinada desses marcadores torna-se possível a dar ênfase em palavras específicas ou acelerar partes inteiras de frases sintetizadas.

![img](https://miro.medium.com/max/30/1*6Un2MnLFrL-LEJYMMDMIfA.jpeg?q=20)

![img](https://miro.medium.com/max/630/1*6Un2MnLFrL-LEJYMMDMIfA.jpeg)

A maioria das plataformas possibilitam a edição direta da skill de maneira que os marcadores SSML possam ser adicionados e editados. No exemplo, a interface da Alexa.

![img](https://miro.medium.com/max/60/1*-a9qtCqK2pfdtrdKgc2lHQ.png?q=20)

![img](https://miro.medium.com/max/630/1*-a9qtCqK2pfdtrdKgc2lHQ.png)

Interface de edição das skills na plataforma Google Actions.

A voz sintetizada é pouco dimensional e oferece uma sensação achatada, ou flat, para usar termos técnicos. Esta falta de profundidade impossibilita, por exemplo, a criação de *skills* que envolvam citações poéticas ou *voice games*.

O marcador **<\*audio\*>** vai adicionar uma nova camada de experiência na sua *skill*.

As duas plataformas mais populares — [Amazon](https://developer.amazon.com/docs/custom-skills/ask-soundlibrary.html) e [Google](https://developers.google.com/actions/tools/sound-library/) — , oferecem bancos de áudio próprios que podem ser incorporados apenas ao código de seus gadgets proprietários, mas bancos de áudio gratuitos que funcionem em ambas as plataformas são bastante fáceis de encontrar na internet.

Existem alguns hacks capazes de dar brilho a sua *skill*:

. Crie *skills* usando apenas vozes pré-gravadas e faça a integração desses arquivos via **<\*audio\*>**, dessa maneira, sempre que precisar de alguma emoção extra não precisará se contentar com as limitações das poucas vozes sintéticas disponíveis nessas plataformas. Isso resolve, por exemplo, o problema com as citações poéticas e o *storytelling* de *voice games*.

. Grave a voz sintética — feature disponível no Google Actions — e trate o arquivo no seu software de áudio preferido, depois faça a integração do arquivo de som via ***<audio>\***, o efeito é surpreendente e bastante útil para *voice games*.

. Ao utilizar arquivos de som, uma boa prática é criar uma trilha introdutória para a *skill*, de maneira que o usuário já esteja habituado a feature quando escutar eventuais efeitos ou trilhas incidentais.

. O marcador ***Gender\***, em algumas plataformas é capaz de mudar temporariamente o gênero da voz de sua skill, dando a impressão de estarmos falando com dois indivíduos diferentes. Não é necessário explicar a utilidade dessa feature para a criação de jogos mais elaborados.

# Simuladores SSML

Existem ótimos simuladores SSML capazes de mostrar na prática alguns dos assuntos que foram tratados neste artigo, o [VocalWare](https://www.vocalware.com/index/demo) é um dos mais simples e serve para perceber a importância desses marcadores.

Se uma simples risadinha fora de hora bastou para viralizar videos da Alexa pelo mundo inteiro, imagine o que o bom uso do *SSML* pode fazer pela sua skill.