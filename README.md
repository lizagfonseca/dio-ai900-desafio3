# dio-ai900-desafio3

> Análise de sentimentos de sentenças e textos com Language Studio no Azure AI

Seguindo o [tutorial](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html) disponibilizado pela Microsoft, foi criado o ambiente de análise de linguagem no Language Studio -- com a exceção de utilizar o idioma Português (Brasil) para os testes.

O texto utilizado para teste foi uma _review_ um tanto mista de um livro, utilizando frases mais longas e um pouco menos diretas para testar a performance do modelo nesse caso.

> Desde as primeiras páginas, há algo na escrita que prende a atenção. A narrativa flui com naturalidade, criando uma imersão que, em alguns momentos, parece quase cinematográfica. Os personagens têm profundidade e nuances interessantes, ainda que alguns diálogos soem um pouco artificiais. A trama se desenvolve com um ritmo instigante, embora existam trechos que parecem se alongar mais do que o necessário.
> 
> A maneira como certos temas são abordados adiciona camadas à história, despertando reflexões que permanecem mesmo depois de fechar o livro. No entanto, algumas reviravoltas podem parecer previsíveis para leitores mais atentos. No fim, é uma leitura que provoca sentimentos mistos — há momentos de verdadeiro impacto, enquanto outros deixam a sensação de que algo a mais poderia ter sido explorado.

A análise do texto, como um todo, é coerente com o conteúdo apresentado:

![Sentimento do texto](https://github.com/user-attachments/assets/1650a921-65a8-4350-a51b-4f05f171684c)


A primeira sentença teve seu sentimento mal compreendido, provavelmente devido à falta de adjetivos diretos -- mesmo que "prender a atenção" seja um elogio quando se trata de escrita.

![Sentença 1](https://github.com/user-attachments/assets/d6baa5b0-9f95-4ba2-bbc9-1a0efebc1595)


A segunda sentença também não teve opiniões detectadas, mas o sentimento foi reconhecido corretamente.

![Sentença 2](https://github.com/user-attachments/assets/554c564d-8e58-4a6f-8045-25c34abe0302)


Na terceira frase o algoritmo já detectou opiniões acertadas, mas falhou em detectar a negativa. 

![Sentença 3](https://github.com/user-attachments/assets/929481b1-3910-47a2-b134-8f81bf3d92c9)


Na quarta sentença, o sentimento também foi corretamente detectado, mas não a opinião negativa. A diferença entre as duas é a presença do adjetivo na opinião positiva.

![Sentença 4](https://github.com/user-attachments/assets/912e77f4-9294-446d-8a79-ee1f617efd28)


O sentimento da quinta frase também foi bem categorizado. 

![Sentença 5](https://github.com/user-attachments/assets/cd90cfda-e461-4359-b074-4bdc50f15ecf)


A sexta sentença também teve seu sentimento corretamente classificado como neutro.

![Sentença 6](https://github.com/user-attachments/assets/1d555dc2-bdcd-47d9-bb4b-27b1c1a6e204)


Por fim, a última sentença teve o sentimento classificado de forma muito semelhante ao texto como um todo. É um resultado coerente com a natureza conclusiva dessa frase.

![Sentença 7](https://github.com/user-attachments/assets/4d2faee9-2c2e-4c53-9016-b4d3e862d89e)


**Conclusão:** esse modelo, no geral, parece capturar muito bem  o sentimento misto dessa _review_, mas falha em categorizar opiniões mais sutis e que demandam um poder de interpretação menos direto devido à falta de adjetivos. A análise de sentimentos não parece ter sofrido com esse "problema", pois teve uma taxa de acerto relativamente alta.
