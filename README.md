# PratosDeMassa
Através de um artefato criador de fusão de multiversos (ACFM) é possível criar experimentos muito engraçados.
Um deles é juntar o universo de N Robin Hood e ver o caos rolar a partir de um ciclo de roubos sem fim.....

Funciona mais ou menos assim: Cada Robin Hood tem uma aldeia. Nessa aldeia existem X pratos de massa na qual o pessoal guarda para ter o que comer na janta. Porém os Robin Hood sempre acham que uma aldeia ter mais pratos de massa do que as outras é injusto. Vamos supor que há quatro Robin Hood por exemplo, assim nós teríamos quatro aldeias com seus respectivos pratos de massa conforme o exemplo abaixo:

0 2 7 0

Nesse exemplo significa que a aldeia 1 não tem nenhum prato de massa, a aldeia 2 tem 2 pratos de massa, a aldeia 3 tem 7 pratos de massa e a última aldeia também não tem nenhum prato de massa. Para deixar os pratos mais "balanceados" um Robin Hood encontra a aldeia que possui mais pratos de massa e rouba-os, distribuindo um a um para cada aldeia (saindo da aldeia vizinha que se encontra mais a direita). Assim, a partir do primeiro exemplo, a nova distribuição de pratos ficaria assim:

2 4 1 2

Como nesse "mashup" de universos há mais de um Robin Hood, o próximo deles, sem saber das alterações feitas pelo último Robin Hood, também tenta balancear os pratos de massa entre as aldeias, executando o mesmo protocolo do último e assim deixando os pratos de massa dessa distribuição:

3 1 2 3

Se os Robin Hood continuarem nesse mesmo processo eles vão chegar, nessa sequência, nas seguintes distribuições:

0 2 3 4
1 3 4 1
2 4 1 2

Porém caso o próximo Robin execute os mesmos passos dos anteriores ele chegará novamente na distribuição 2 4 1 2 e assim entrando em um loop infinito.... Para quem só está assistindo (o nosso caso) parece ser um ótimo passatempo de final de domingo ficar apenas observando-os.

Junto a isso você fica curioso(a): e se fossem "grudados" outros universos com mais Robin Hood e consequentemente com mais aldeias com outras quantidades de pratos de massa? Quantas "rodadas" demoraria para entrar um loop infinito? No caso acima demorou 5 rodadas. Será que com outros testes demoraria muito mais? Quanto tempo exatamente?

Vetor utilizado no código: 4	1	15	12	0	9	9	5	5	8	7	3	14	5	12	3
