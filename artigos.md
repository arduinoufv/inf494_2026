## Alocar tarefas - Luiz, Lucas, Henrique, Caio
# Colabs

* [Float4 e 3](https://colab.research.google.com/drive/1_Sz2RDr3mAZvfZ4FZZdYUM07d0A5aFhm?usp=sharing)
    * fazer uma simulação da soma, multiplicacao Float 4 ou 3
         * definir a faixa
         * simular com dados do makeclassification para KNN
         * medir tempo com tabela em memória versus código emulado em GPU 

* Algoritmos de ordenação e PTX
* Ferramentas para estatisticas do PTX, editor que marca "trechos PTX" e mostra grafos
* Uso de instruções especiais em assembler para "campos de bits"
* teste se "forcamos uma ordem no PTX" (exemplo ordenação, IF de árvores, Kmeans)
* Gráficos de desempenho 
*      

# Artigos

Ian/Leanderson/Nicolas

## KNN e Quantização
### IAN 
 * Mnist com 1,2,3, 4 e 8 bits - KNN 50k 40k (fake 4x10K)
 *  1 bit = Xor e Popcount , acuracia ok, 
 *  2 bit = shift e subtracao - ADICIONAR xor e popcount APROXIMADO
 *  3,4 e 8 bits = shift e subtracao  (teste PAD 3bits + pad, não mudou tempo)
### Nicolas
 
 * ADICIONAR CIFAR10, baseline CUML, 2 CNN pytorch resnet18 e lenet
 * ADICIONAR Drop com Clock e grupo

## Placement
### Leanderson
### Luis
--------------------------------------------------

Isabela/Pedro/Mariana/Ellen/Matheus
## Kmeans e DBSCAN
 ### Pedro e Isabela (IC)
    * Kmeans
       * Arvores - Explicabilidade   
    * DBSCAN
       * Arvores
       * Heuristica com Grafo (em andamento)
### Mariana, Ellen e Matheus  
    * DBSCAN 
    * Cuml, Gemini-pro (Colab)
    * Aproximado - Drop nos "cores point"
    * Pacotes 8 e 4 bits. 
    * Gerar datasets: variação de densidade e variação heterogenea (versão multi EPS)
    
## Estratégias de Árvores 

* [click here](https://colab.research.google.com/drive/1Fh49wZ9V1M5ju_cahO0FTUKKsBQCTIti?usp=sharing)
----------------------------------

Guilherme TCC
* Variar o tamanho da arvores

## Placement

## PTX instruções especiais
------------------------------------------
# Operadores Tensores
## Caio
* GEMM demonstração
* KNN
      * CUDA com tensores
      * Makeclassification
      * baseline: "Pytorch", CuML float16, int8 (CUDA)
      * Float16
      * Artigos que usam tensores em outras aplicações
------------------------------
## Luiz, Lucas, Henrique
* Ler segmentos (pulos de grid) de um vetor
* Validar os algoritmos de ordenação (bolha, insercao, merge, odd-even, quick, radix, selecao)
* Ferramentas de visualizacao e estatistica de PTX.
