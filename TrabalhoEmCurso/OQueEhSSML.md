- [Amazon Alexa](https://celsokitamura.com.br/category/amazon-alexa/)
- [Conceitos Básicos da Programação](https://celsokitamura.com.br/category/conceitos/)

# O que é SSML?

 Tempo de leitura: 3 min

![img](https://secure.gravatar.com/avatar/bf285b30916c369737c23bab9144b63b?s=45&d=mm&r=g)

Escrito por Celso Kitamura em 13 de fevereiro de 2020

#### Compartilhe agora mesmo:

![O que é SSML?](https://celsokitamura.com.br/wp-content/uploads/2020/02/123-O-Que-%C3%89-SSML-742x200.jpg)

Como vimos, a revolução da voz já começou! Graças ao lançamento da linha de dispositivos Amazon Echo no Brasil (com maciça divulgação) mais atenção está sendo dada aos aplicativos e dispositivos habilitados para voz. Mas a tecnologia de voz não é precisamente uma novidade, a linguagem de marcação de síntese de fala (SSML – Speech Synthesis Markup Language) já existe há algum tempo. Mas o que é SSML?

 

## Um Pouco De História

 

O SSML se baseou na JSML (Java Speech Markup Language) desenvolvida pela Sun Microsystems, mas a recomendação atual da W3C foi desenvolvida principalmente por fornecedores de síntese de fala.

 

Ele cobre praticamente todos os aspectos da síntese da fala. Embora algumas áreas não tenham sido especificadas, cada fornecedor aceita uma variante diferente do idioma.

 

Além disso, na ausência de marcação, espera-se que o sintetizador faça sua própria interpretação do texto.

 

## O Que É SSML?

 

O SSML oferece aos desenvolvedores e criadores de conteúdo a capacidade de não apenas gerar fala, mas também controlar os aspectos mais refinados, como pronúncia, inflexão, afinação e muito mais.

 

Não é objetivo deste artigo esgotar o assunto SSML, mas podemos ver alguns atributos para que você tenha uma ideia de como a coisa funciona.



 

SSML especifica várias marcações para prosódia. Isso inclui as marcações:

 

- pitch
- contour
- pitch range
- rate
- duration
- volume

 

Nem todas as implementações incluem suporte para todos os atributos. A Alexa Voice Service oferece suporte apenas aos atributos de rate, pitch e volume, por isso vamos ver estes atributos com mais detalhes.

 

 

### pitch

 

O atributo pitch aumenta ou diminui o tom da fala. Podemos utilizar cinco valores predefinidos: x-low, low, medium, high e x-high. Ou pode-se ainda usar um valor percentual (variando de -33,3% a + 50%) para um controle mais preciso.

 

<speak>

<prosody pitch="+50%">Isto é alto

e

<prosody pitch="-33.3%">isto é baixo</prosody>.

</speak>

 

### rate

 

O atributo rate controla a velocidade da fala. Podemos usar alguns valores predefinidos: x-slow, slow, medium, fast e x-fast.

Podemos usar também valor percentual. Qualquer coisa abaixo de 100% diminui a velocidade e valores acima de 100% aceleram.

 

<speak>

  <prosody rate="x-slow">As vezes eu falo bem bem devagar</prosody>.

Posso também falar normal e as vezes

  <prosody rate="x-fast">também falo bem bem rápido </prosody>.

</speak>

 

### volume

 

O atributo volume controla o volume da fala. Temos seis valores predefinidos: silent, x-soft, soft, medium, loud e x-loud. Podemos também usar um valor positivo ou negativo. Importante: desta forma, não se está atribuindo um volume fixo, mas alterando-o em relação ao volume atual.

 

<speak>

  <prosody volume="x-soft">Um sussurro.</prosody>

  <prosody volume="x-loud">Falo alto.</prosody>

  <prosody volume="-6dB">Metade da altura.</prosody>

</speak>

 

## Palavras Finais

 

Ao criar skills para Alexa muito provavelmente você não precisará utilizar SSML, a não ser em casos muito específicos. Mas é muito importante saber que podemos alterar vários aspectos da nossa resposta em voz apenas utilizando alguns atributos no texto de retorno que geramos para o dispositivo do usuário.

 

Este artigo não pretende ser um texto definitivo sobre SSML, apenas um apanhado para você ter ideia dos conceitos de o que é SSML.



 

Se você quiser saber mais detalhes, a recomendação completa do SSML pode ser vista aqui: [Recomendação SSML no W3C](https://www.w3.org/TR/speech-synthesis11/).

 

E se você quer saber mais sobre como desenvolver skills para Alexa, me acompanhe nesta jornada!

 

Meu e-book com 4 passos para criar sua primeira skill Alexa está GRATUITO por tempo limitado!



Olha o link: ![👉🏼](https://s.w.org/images/core/emoji/13.0.1/svg/1f449-1f3fc.svg) https://celsokitamura.com.br/minha-primeira-skill-alexa

Bora aprender a desenvolver skills para Alexa!