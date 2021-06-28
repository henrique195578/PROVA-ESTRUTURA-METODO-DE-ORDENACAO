# PROVA-ESTRUTURA-METODO-DE-ORDENACAO

![UNIPAR ](https://www.calendariodovestibular.com.br/wp-content/uploads/2013/03/post_unipar.png) 

2º A.A.R.E - ESTRUTURA DE DADOS
=============================
   ## Métodos de Ordenação  

### Acadêmico: Henrique Borges da Silva 
### R.A: 00195578
### Orientador: Geferson Luis Simonette
*******
##### Toledo, 27/06/2021

*****
# Ordenação de Dados

Ordenação é o ato de se colocar os elementos de uma sequência de informações,
ou dados, em uma ordem predefinida. O termo técnico em inglês para ordenação é
sorting, cuja tradução literal é "classificação"
****
## Bubble Sort

- - O algoritmo de “ordenação bolha”, ou “bubble sort”, recebeu este nome pela imagem pitoresca usada para descrevê-lo: os elementos maiores são mais leves, e sobem como bolhas até suas posições corretas. A ideia fundamental é fazer uma série de comparações entre os elementos do vetor. 
- - Quando dois elementos estão fora de ordem, há uma inversão e esses dois elementos são trocados de posição, ficando em ordem correta. Assim, o primeiro elemento é comparado com o segundo. Se uma inversão for encontrada, a troca é feita. 
- - Em seguida, independente se houve ou não troca após a primeira comparação, o segundo elemento é comparado com o terceiro, e, caso uma inversão seja encontrada, a troca é feita. O processo continua até que o penúltimo elemento seja comparado com o último.
- - Com este processo, garante-se que o elemento de maior valor do vetor será levado para a última posição. A ordenação continua, posicionando o segundo maior  elemento, o terceiro, etc., até que todo o vetor esteja ordenado.
### Exemplo

![Bubble Sort ](https://1.bp.blogspot.com/-ze-d6TojsIc/WosqmlzytjI/AAAAAAAAHgk/WwtlW8Mxl1kksEFTRMwYdPOGy-VkkvERgCLcBGAs/s1600/img_post.png)
* Uma função que implementa esse algoritmo. A função recebe como
parâmetros o número de elementos e o ponteiro do primeiro elemento
do vetor que se deseja ordenar.

***
## Selection Sort
- - Ordenação por seleção do inglês, “selection sort” é um algoritmo de ordenação baseado em se passar sempre o menor valor do vetor para a primeira posição ou o maior dependendo da ordem requerida, depois o de segundo menor valor para a segunda posição, e assim é feito sucessivamente com os {n-1} n-1 elementos restantes, até os últimos dois elementos. 
- - O selection sort compara a cada interação um elemento com os outros, visando encontrar o menor. Dessa forma, podemos entender que não existe um melhor caso mesmo que o vetor esteja ordenado ou em ordem inversa serão executados os dois laços do algoritmo, o externo e o interno. Algoritmo breve de como faz para ordenar os números, assumimos que o menor elemento está no índice 0: encontra o índice do menor elemento

 ### Exemplo
![Selection Sort ](https://2.bp.blogspot.com/-2rFqCKDe6FU/WyQtfeORR0I/AAAAAAAAIAw/UcxMCjSWhrghkyYgcxLHE_xeljmLmM7CACLcBGAs/s1600/selection-sort.jpg)

***
## Insertion Sort
- - Algoritmo de ordenação que, dado uma estrutura (array, lista) constrói uma matriz final com um elemento de cada vez, uma inserção por vez. Assim como algoritmos de ordenação quadrática, é bastante eficiente para problemas com pequenas entradas, sendo o mais eficiente entre os algoritmos desta ordem de classificação.
- - O Insertion Sort inicia a ordenação dividindo o vetor em duas partições: uma ordenada à esquerda e outra não ordenada à direita. Inicialmente, a partição esquerda só terá um elemento é o caso trivial da ordenação. 
- - A inserção dos elementos na partição ordenada é realizada em duas etapas. Na primeira etapa, procuramos a posição de inserção. Na segunda etapa, deslocamos os elementos da esquerda para a direita para que a posição de inserção fique livre para que o elemento seja inserido.

### Exemplo
![Insertion Sort ](https://3.bp.blogspot.com/-XJYmRJQI5bk/WzFtRxaY5dI/AAAAAAAAIGY/lxOyWLFCenUkndIJfDVQGS7p1zowhxQbwCLcBGAs/w960/insertion-sort.jpg)
****
##  Quick sort
- - O algoritmo quicksort é um método de ordenação muito rápido e eficiente, inventado por C.A.R. Hoare em 1960, quando visitou a Universidade de Moscovo como estudante. Naquela época, Hoare trabalhou em um projeto de tradução de máquina para o National Physical Laboratory
- - Algoritmo de ordenação mais utilizado no desenvolvimento de aplicações. Mesmo quando temos os dados organizados em listas encadeadas, e precisamos colocá-los de forma ordenada, em geral, optamos por criar um vetor temporário com ponteiros para os nós da lista, fazer a ordenação usando quicksort e reencadear os nós montando a lista ordenada.

### Exemplo
![Quick Sort ](https://1.bp.blogspot.com/-ozQq0I2cN5Q/W4OikPQAGaI/AAAAAAAAIhQ/8fu07RueeDU8zeaqMZz0m-6y2hzOh7wOwCLcBGAs/s1600/quicksort-algoritmo-de-ordenacao.jpg)



### Estudo dos casos de uso
-- Foram testadas 3 ordens de listas com 3 tamanhos diferentes cada:
 * Ordem 1: lista ordenada em ordem crescente.
* Ordem 2: lista ordenada em ordem decrescente.
* Ordem 3: lista desordenada com números aleatórios.

*** 
### Lista 1 - Comparativos
-  **Tamanho do vetor: 100**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------  | --------- |----------- | ------------- |
|Bubble Sort     |0,0988     |5050        | 0
|Selection Sort  |0,0602     |4950        |297
|Insertion Sort  | 0,0038    |99          | 198
|Quick Sort      |0,0141     |606         |189

- **Tamanho do vetor: 1000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------  | --------- |----------- | ------------- |
|Bubble Sort     |9,5451     |500500      | 0
|Selection Sort  |5,4587     |499500      |2997
|Insertion Sort  |0,0359     |999         | 1998
|Quick Sort      |0,1602     |9009        |1533

- **Tamanho do vetor: 10000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------  | --------- |----------- | ------------- |
|Bubble Sort     |934,5364     |50005000  | 0
|Selection Sort  |508,5891     |49995000  |29997
|Insertion Sort  |0,3558       |9999      | 19998
|Quick Sort      |2,0824       |125439    |17712

***
### Lista 2 - Comparativos
-  **Tamanho do vetor: 100**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |0,2045     |5050        | 14850
|Selection Sort   |0,0750     |4950        |297
|Insertion Sort   | 0,1173    |99          | 5148
|Quick Sort       |0,0147     |610         |336

- **Tamanho do vetor: 1000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |20,3377    |500500      | 1498500
|Selection Sort   |6,9038     |499500      |2997
|Insertion Sort   |11,4277    |999        | 501498
|Quick Sort       |0,1622     |9016        |3030

- **Tamanho do vetor: 10000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |1838,0272  |50005000    | 149985000
|Selection Sort   |665,2050   |49995000    |29997
|Insertion Sort   |1074,1171  |9999        | 50014998
|Quick Sort       |2,1279     |125452      |32712

***
### Lista 3 - Comparativos
-  **Tamanho do vetor: 100**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |0,1596     |5050        |6777
|Selection Sort   |0,0698     |4950        |297
|Insertion Sort   |0,0570     |99          |2457
|Quick Sort       |0,0314     |897         |576

- **Tamanho do vetor: 1000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |16,6730    |500500      |756840
|Selection Sort   |5,6664     |499500      |2997
|Insertion Sort   |5,7523     |999         |254278
|Quick Sort       |0,3725     |13138        |7983

- **Tamanho do vetor: 10000**

|   Algoritmo     |Tempo (ms) |Comparações | Movimentações
| -------------   | --------- |----------- | ------------- |
|Bubble Sort      |1455,9734  |50005000    | 74237889
|Selection Sort   |545,1068   |49995000    |29997
|Insertion Sort   |539,6891   |9999        | 24765961
|Quick Sort       |4,5072     |176065      |103635
***
## Conclusão 
 * O algoritmo **Bubble Sort**, apesar de ser o de mais fácil implementação, não apresenta resultados satisfatórios, principalmente no número de comparações. A ineficiência desse algoritmo pode ser traduzida como um grande consumo de processamento, o que, para máquinas com poucos (ou limitados) recursos computacionais, resulta em lentidão e longos períodos de espera. Sua aplicação é, na opinião dos autores, indicada somente para fins educacionais, visto que um projeto com o mesmo pode ser considerado ineficiente e/ou fraco. Para listas já ordenadas em ordem crescente é o único algoritmo que não realiza movimentações, mas em compensação é o que tem o maior tempo e o maior número de comparações. Não só em listas já ordenadas, mas em todos os casos o bubble sort se mostrou um algoritmo ineficiente.
 
 * O **Selection Sort** nas listas de ordem 1 e ordem 3, o selection sort foi o segundo pior algoritmo, mas se mostrou mais eficiente do que o Insertion sort em relação ao tempo e a quantidade de movimentações na lista de ordem 2. 
 Ele torna-se útil em estruturas lineares similares ao do Insertion Sort, porém, com o número de elementos consideravelmente maior, já que, o número de trocas é muito inferior ao número de comparações, consumindo, assim, mais tempo de leitura e menos de escrita. A vantagem de seu uso ocorre quando se trabalha com componentes em que, quanto mais se escreve, ou reescreve, mais se desgasta, e, consequentemente, perdem sua eficiência, como é o caso das memórias EEPROM e FL
 
 * O **Insertion Sort** na lista de ordem 1, o Insertion sort se mostrou mais eficiente que todos os outros algoritmos em relação ao tempo e comparações. Na lista de ordem 2 foi menos eficiente do que o selection sort e na lista de ordem 3 a diferença de tempo entre o insertion e o selection foi pequena. 
 Sendo que por sua vez, é útil para estruturas lineares pequenas, geralmente entre 8 e 20 elementos, sendo amplamente utilizados em sequências de 10 elementos, tendo ainda, listas ordenadas de forma decrescente como pior caso, listas em ordem crescente como o melhor caso e, as demais ordens como sendo casos medianos. Sua principal vantagem é o pequeno número de comparações, e, o excessivo número de trocas, sua desvantagem. Como exemplo de uso, tem-se a ordenação de cartas de um baralho
 
* O algoritmo **Quick Sort** certamente é o algoritmo mais eficiente em listas totalmente desordenadas, ele se torna muito eficiente em relação aos outros no quesito de tempo. Na lista de ordem 3 e na de ordem 2 a diferença de tempo do quick sort em comparação aos outros foi absurdamente grande. 
Ao subdividir o vetor e fazer inserções diretas utilizando um valor de referência o pivô, reduz seu tempo de execução, mas, as quantidades de comparações de leitura e, principalmente, trocas escrita ainda são muito altas. Apesar disso, o Quick Sort se apresenta uma boa opção para situações em que o objetivo é a execução em um menor tempo, mesmo que para isso haja um detrimento em recursos computacionais de processamento


# Referência 
*  [Bubble Sort](https://pt.wikipedia.org/wiki/Bubble_sort)
 * [Quick Sort](https://pt.wikipedia.org/wiki/Quicksort)
 * [Insertion Sort](https://pt.wikipedia.org/wiki/Insertion_sort)
 *  [Selection Sort](https://pt.wikipedia.org/wiki/Selection_sort)
 * [Métodos de Ordenação](https://homepages.dcc.ufmg.br/~cunha/teaching/20121/aeds2/sortingcmp.pdf)
  * [Comparativos](https://www.devmedia.com.br/algoritmos-de-ordenacao-analise-e-comparacao/28261)
