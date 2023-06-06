# Moxila
Algoritmo para resolver o problema da mochila

1-Definir a representação dos indivíduos:
Utilizei um vetor binário para representar a presença ou ausência de cada item na mochila. Onde se tiver N itens, o vetor terá tamanho N, onde o valor 1 representa a inclusão de um item e o valor 0 representa a exclusão.

2- Inicializar a população:
Desenvolvi uma população inicial de indivíduos de forma aleatória. Onde cada indivíduo deve ter um cromossomo que represente uma possível solução para o problema da mochila.

3- Avaliar a aptidão dos indivíduos:
Implementei uma função de avaliação que atribua uma pontuação (ou fitness) a cada indivíduo com base no valor total dos itens incluídos e na violação das restrições de capacidade da mochila. Quanto maior o valor e menor a violação, melhor será a aptidão do indivíduo.

4- Seleção:
Utilizei um método de seleção, como a seleção por roleta, para escolher indivíduos com maior aptidão para serem pais da próxima geração. Quanto maior a aptidão, maior a probabilidade de um indivíduo ser selecionado.

5- Cruzamento:
Apliquei um operador de cruzamento (recombinação) para gerar descendentes a partir dos indivíduos selecionados. Onde utilizei o crossover de um ponto, onde um ponto de corte é escolhido aleatoriamente e os genes são trocados entre os pais para criar os descendentes.

6- Mutação:
Introduzi mutações aleatórias nos descendentes gerados para garantir diversidade genética na população. Sendo assim, será alterado aleatoriamente alguns genes do cromossomo (mudando de 0 para 1 ou vice-versa) para explorar novas soluções.

7- Atualizar a população:
Foi substituido a população atual pelos descendentes gerados (juntamente com alguns indivíduos selecionados da população anterior). Isso formou a nova geração de indivíduos.

8- Critério de parada:
Defini um critério de parada, como um número máximo de iterações ou uma condição de convergência, para encerrar o algoritmo genético.
