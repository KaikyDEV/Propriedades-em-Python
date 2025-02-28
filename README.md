# Propriedades-em-Python

As propriedades em Python são uma forma de controlar o acesso aos atributos de uma classe, permitindo a definição de comportamentos personalizados para a leitura, escrita e exclusão de atributos. Elas são definidas usando os decoradores @property, @atributo.setter e @atributo.deleter.
Exemplo 1: Classe Foo

Vamos analisar a classe Foo.

__init__ Method

O método __init__ inicializa a instância da classe com um atributo _x.
@property x

O método x decorado com @property define um getter para o atributo _x. Ele retorna _x se _x for um valor válido, caso contrário retorna 0.
@x.setter

O método x decorado com @x.setter define um setter para o atributo _x. Ele adiciona o valor passado ao valor atual de _x, tratando os valores None como 0.
@x.deleter

O método x decorado com @x.deleter define um deleter para o atributo _x. Ele define _x como -1 quando deletado.

Uso da Classe Foo

Exemplo 2: Classe Pessoa

Agora, vamos analisar a classe Pessoa.

__init__ Method

O método __init__ inicializa a instância da classe com os atributos _nome e _ano_nascimento.
@property nome

O método nome decorado com @property define um getter para o atributo _nome. Ele simplesmente retorna o valor de _nome.
@property idade

O método idade decorado com @property define um getter para o atributo idade. Ele calcula a idade da pessoa com base no ano atual (2024) e no ano de nascimento.

Uso da Classe Pessoa

Resumo

As propriedades em Python permitem encapsular a lógica de acesso a atributos, proporcionando maior controle e flexibilidade. No exemplo da classe Foo, mostramos como usar getters, setters e deleters para controlar o acesso ao atributo _x. Na classe Pessoa, mostramos como usar getters para fornecer acesso a atributos calculados, como idade.

