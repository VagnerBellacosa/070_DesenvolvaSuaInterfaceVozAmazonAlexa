# Geração de fala a partir de documentos SSML

[PDF](https://docs.aws.amazon.com/pt_br/polly/latest/dg/polly-dg.pdf#ssml)

[RSS](https://docs.aws.amazon.com/pt_br/polly/latest/dg/doc-history.rss)



Você pode usar o Amazon Polly para gerar fala a partir de texto sem formatação ou de documentos marcados com o Speech Synthesis Markup Language (SSML). Usar um texto aprimorado por SSML permite exercer controle adicional sobre como o Amazon Polly gera fala com base no texto fornecido.

Por exemplo, você pode incluir uma pausa longa dentro do texto ou alterar a velocidade ou o tom da fala. Outras opções incluem:

- enfatizar palavras ou frases específicas
- usar a pronúncia fonética
- incluir sons de respiração
- sussurrar
- usar o estilo de locutor.

Para obter detalhes completos sobre as tags SSML compatíveis com o Amazon Polly e como usá-las, consulte[Tags SSML compatíveis](https://docs.aws.amazon.com/pt_br/polly/latest/dg/supportedtags.html)

Ao usar SSML, há vários caracteres reservados que exigem tratamento especial. Isso ocorre porque o SSML usa esses caracteres como parte de seu código. Para usá-los, você usa uma entidade específica para *escapá-los*. Para obter mais informações, consulte[Caracteres reservados no SSML](https://docs.aws.amazon.com/pt_br/polly/latest/dg/escapees.html)

O Amazon Polly fornece esses tipos de controle com um subconjunto de tags SSML definidas pelo[Speech Synthesis Markup Language (SSML) Version 1.1, W3C Recommendation (](https://www.w3.org/TR/2010/REC-speech-synthesis11-20100907/).

Você pode usar o SSML no console do Amazon Polly ou com aAWS CLI. Os tópicos a seguir mostram como você pode usar o SSML para gerar a fala e controlar a saída de modo que ele atenda perfeitamente às suas necessidades.

**Tópicos**

- [Caracteres reservados no SSML](https://docs.aws.amazon.com/pt_br/polly/latest/dg/escapees.html)
- [Usar SSML (Console)](https://docs.aws.amazon.com/pt_br/polly/latest/dg/ssml-to-speech-console.html)
- [Uso de SSML (AWS CLI)](https://docs.aws.amazon.com/pt_br/polly/latest/dg/ssml-synthesize-speech-cli.html)
- [Tags SSML compatíveis](https://docs.aws.amazon.com/pt_br/polly/latest/dg/supportedtags.html)