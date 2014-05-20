ATPS – CONSULTA E ORDENAÇÃO
=========================

### Propósito desta aplicação:
Criar uma lista única de clientes, que serão ordenados por idade e categorizados como
normais e acima de 50 anos.

### Metodologia:
Separar e tratar grupos de clientes que entram em um estabelecimento juntos, de forma
a categorizar de forma justa.
Foi escolhida a utilização de Double bubble sort para a ordenação das listas, uma vez
que os elementos ordenados são objetos, impedindo a utilização de helpers.

### Fundamento:
Seguenciar a fila única por chegada, idade e categoria, de forma que os acima de 50
são classificados de forma independente e somados os normais, no entanto estes
grupos ordenados são acumulados sequencialmente por chegada de grupo.


### Tecnologia:
Com o intuito de melhor apresentar as ações concorrentes, escolhemos o uso de
HTML5 e JavaScript, permitindo a migração desta para mobile.

### Fases do Desenvolvimento
1. Preparar um contador para acompanhar as chegadas;
2. Crirar um vetor para a fila de comuns;
3. Criar um vetor para a fila de preferenciais;
4. Criar um vetor para uma fila única;
5. Preencher a lista comum;
6. Preencher a lista preferencial;
7. Classificar as listas em ordem crescente, considerando a idade como chave de
ordenação;
8. Precorrer a lista preferencial de baixo para cima e alimentar na fila única;
9. Precorrer a lista normal de baixo para cima e alimentar na fila única;
10. Remover das lista normal e preferencial os ítens conforme inclui na fila única;

### Requisitos técnicos:
1. Utilizar uma classe ou estrutura (JSON) para representar um indivíduo;
2. Ordenar estes indivíduos por idade utilizando Double bubble sort
