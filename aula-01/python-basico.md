# Python Básico

Como muitas já sabem, Python é a linguagem mais querida quando se trata de ciência de Dados. Isso se deve ao fato de, além de ser uma ferramenta open source, Python também é bastante flexível, têm várias bibliotecas para manipulação de dados e é extremante fácil de aprender, podendo ser usado por todo tipo de analistas de dado.

## Regras Básicas

### Identação D:

Uma das coisas que mais causa dor de cabeça pra quem está vindo de outras linguagens, é o fato de Python ser bastante baseado em identação.

__JavaScript__

```JavaScript
if (batata == 'batata doce') {
  result = "maromba"
}
```

__Python__

```Python
if batata == 'batata doce':
    result = "maromba"
```

### Esquece o ";"

Em Python, não existe o __;__, então não precisamos nos preocupar em esquecer de colocar ele em algum lugar.

### Comentários

```Python
#Isso é um comentário de uma linha

'''
Esse
Pode ser
Um comentário
Gigante
'''
```

### Escrevendo coisas na Tela

```Python
print('Eu amo batata')
```

### Definindo variáveis

Python é um linguagem fracamente tipada, o que significa que não é necessário dizer qual o tipo da variável (string, int, float, ect) na hora de criá-la.

```Python
oitava_maravilha = 'batata'
```

### Criando funções

Na hora de criar uma função, as três principais coisas que você precisa lembrar são:

- __def__: A palavra chave para definir uma função.
- __Dois pontos__: Assim como no if, precisamos colocar dois pontos após a definição dos parametros para marcar o inicio do corpo da função
- __Identação__: O corpo da função deve estar identado;

``` Python
#Função com retorno
def soma(num1, num2):
    return num1 + num2

#Função sem retorno e sem parâmetros
def escreve_batata():
    print('Batata')

#Chamando as funções
soma(num1=2, num2=4)
>>> 6

escreve_batata()
>>> 'Batata'
```

## Listas

Uma lista é uma estrutura de dados composta por itens organizados de forma linear, na qual cada um pode ser acessado a partir de um índice, que representa sua posição na lista (iniciando em zero).

Listas em Python são bem flexíveis, sendo possível ter items de tipos diferentes na mesma lista e até uma lista de listas.

```Python
beatles = ['John', 'Ringo', 'Paul', 'George']

generos = [['rock', 'metal'], ['pop', 'funk', 'electronic'], ['sertanejo']]

mistura = [1,2,'pato',[3,4]]
```

Acessando os conteúdos das listas

```Python
beatles[0]
>>> 'John'

generos[2]
>>> ['sertanejo']
```

## Tulpas

Tuplas podem ser consideradas similares às listas, mas suas diferenças são cruciais:

- __Sintaxe__: A tupla se diferencia por substituir os colchetes ([]) das listas por parênteses (())

```Python
tulpa1 = ('121234.44', '78878.4445')
```

- __Imutabilidade__: Ao contrário das listas, as tulpas são imutáveis.

## Dicionários

Vamos pensar temos várias tulpas:

```Python
filme1 = ('Dunkirk', 'Christopher Nolan')
filme2 = ('Princesa Prometida', 'Rob Reiner')
```
e queremos criar um catálogo de filmes, poderíamos fazer isso criando uma lista de tulpas:

```Python
catalogo = [filme1, filme2]
```

porém, dessa forma teríamos um pouco de dificuldade em acessar o conteúdo dessa lista. Digamos que a gente queira o diretor de Princesa prometida. Para isso, teremos que saber que esse filme é o segundo da lista e pegar o segundo parâmetro da tulpa, o que pode se tornar inviável conforme a lista vai escalando. Para isso, temos os dicionários.

Dicionários são estruturas de dados que implementam mapeamentos, onde um mapeamento é uma coleção de associações entre pares de valores, o primeiro elemento do par é chamado de chave e o outro de conteúdo.

```Python
#Criando
catalogo =
    {
        'Dunkirk': 'Christopher Nolan',
        'Princesa Prometida': 'Rob Reiner'
    }

#Descobrindo o diretor de Princesa Prometida
catalogo['Princesa Prometida']
>>> 'Rob Reiner'
```

## Saiba mais
- [Introdution to Python (DataCamp)](https://www.datacamp.com/courses/intro-to-python-for-data-science)

### [>>> Próximo Capitulo - Pandas](pandas.md)