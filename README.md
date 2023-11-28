
**PROJETO FINAL**

tópicos avançados em sistemas digitais

**Cálculo de área de círculo:**

- consideramos PI = 3,125
- área = 3,125 \* R²
- área otimizada = 99,41% da área original
- diferença de apenas **0,52%**

**Cálculo do volume de esfera:**

- consideramos 4\*PI/3 = 4,25
- volume = 4 \* PI \* R³ / 3
- volume otimizado = 101,461% do volume original
- diferença de apenas **1,46%**

**Modo de utilização:**

SW(17) = 0 => cálculo de área

SW(17) = 1 => cálculo de volume

SW(3 downto 0) => raio

LEDR(17 downto 4) => resultado casas inteiras

LEDR(3) => vírgula

LEDR(2 downto 0) => resultado casas decimais





**ÁREA:**



|pi = 3.141|pi = 3.125|r² otimizado|tudo otimizado|
| :- | :- | :- | :- |
|352 somas|80 somas|15 somas|4 somas|

*análise de área*

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.001.png)


*análise de* timing

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.002.png)

*análise de potência*

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.003.png)




||||||c d|b d|a d|a c|a b||a|
| :- | :- | :- | :- | :- | -: | -: | -: | -: | -: | :- | -: |
||||||d||b c||b|||
|||||x|||c|||||
||||||||1|1,,|0|0|1|


|v1|||||c d|b d|a d|a c|a b||a|
| :- | :- | :- | :- | :- | -: | -: | -: | -: | -: | :- | -: |
|v2|||||d||b c||b|||
|v3|||||||c|||||
|v4||||0|0|0|0|0|0|0|x|
|v5||||0|0|0|0|0|0|0|x|
|v6||||0|0|0|0|0|0|0|x|
|v7|||0|0|0|0|0|0|0|x|x|
|v8|||0|0|0|0|0|0|0|x|x|
|v9|||0|0|0|0|0|0|0|x|x|
|v10||c d|b d|a d|a c|a b||a|x|x|x|
|v11||d||b c||b|||x|x|x|
|v12||||c|||||x|x|x|
|v13|c d|b d|a d|a c|a b||a|x|x|x|x|
|v14|d||b c||b|||x|x|x|x|
|v15|||c|||||x|x|x|x|


|v1|c d|b c|a c|!a !b c|! c d|a d|a !d|a !c|!a b|0|a|
| :- | -: | -: | -: | -: | -: | -: | -: | -: | -: | -: | -: |
|v2|c d|!c d|c|a b !c|b|!a b|a c|a b||||
|v3|d|b d|b d|c d|a c|b c|!b c|||||
|v4|||a d|a d||b d||||||




**VOLUME:**



|4\*pi/3 = 4.19|4\*pi/3 = 4.25|r³ otimizado|tudo otimizado|
| :- | :- | :- | :- |
|1472 somas|320 somas |24 somas|5 somas|

*análise de área*

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.004.png)


*análise de* timing

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.005.png)


*análise de potência*

![](imgs/Aspose.Words.728e20fa-5609-48df-9739-ffceb2a7bd85.006.png)


||||||cd|d|b c d|b c|a b d|a b c|a b|a c|a c|a b|a|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
||||||||b d|a c d|a c d|a c|a d|b||||
|||||||||b d|a d|b d|a b c|a d||||
|||||||||a d|b d|a b d|a c|||||
|||||||||b c d|c||b c|||||
|||||||||c d||||||||
||||||x||||||1|0|0,,|0||


|v01|||||cd|d|b c d|b c|a b d|a b c|a b|a c|a c|a b|a|
| :-: | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|v02|||||||b d|a c d|a c d|a c|a d|b||||
|v03||||||||b d|a d|b d|a b c|a d||||
|v04||||||||a d|b d|a b d|a c|||||
|v05||||||||b c d|c||b c|||||
|v06||||||||c d||||||||
|v07||||0|0|0|0|0|0|0|0|0|0|0||
|v08||||0|0|0|0|0|0|0|0|0|0|0||
|v09||||0|0|0|0|0|0|0|0|0|0|0||
|v10||||0|0|0|0|0|0|0|0|0|0|0||
|v11|||0|0|0|0|0|0|0|0|0|0|0|||
|v12|||0|0|0|0|0|0|0|0|0|0|0|||
|v13|||0|0|0|0|0|0|0|0|0|0|0|||
|v14|||0|0|0|0|0|0|0|0|0|0|0|||
|v15||0|0|0|0|0|0|0|0|0|0|0||||
|v16||0|0|0|0|0|0|0|0|0|0|0||||
|v17||0|0|0|0|0|0|0|0|0|0|0||||
|v18||0|0|0|0|0|0|0|0|0|0|0||||
|v19|cd|d|b c d|b c|a b d|a b c|a b|a c|a c|a b|a|||||
|v20|||b d|a c d|a c d|a c|a d|b||||||||
|v21||||b d|a d|b d|a b c|a d||||||||
|v22||||a d|b d|a b d|a c|||||||||
|v23||||b c d|c||b c|||||||||
|v24||||c d||||||||||||


|v1||b d|b c d|b c|a c|a d|b c d|b !c|a b|a b c|a !b|a c|a c|a b|a|
| :-: | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|v2||d|c d|a c d|c !d|b c|b d|a c d|a b d|c|a d|b||||
|v3||cd|0|a d|a b d|!b d|a b|b d|a c d|b d|a b c|a d||||
|v4||cd|0|b c d|a c d|a b c|a b c|b c d|a d|a b d|a c|||||
|v5||0|0|0|a d|a b d|0|c d|b d|!a c|b c|||||
