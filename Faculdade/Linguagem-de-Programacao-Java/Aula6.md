﻿## Aula 6 - Encapsulamento e associações de classes
**Encapsulamento** 

Mecanismo utilizado na Programação Orientada a Objetos, que visa obter segurança, modularidade e autonomia para os objetos; 
Conseguido, através da definição de visibilidade privada dos atributos, ganhando-se, assim, autonomia, para definir o que o mundo externo a classe poderá visualizar e acessar, normalmente através de métodos públicos. 
**O Encapsulamento protege os atributos de acesso direto e permite apenas acesso através de métodos públicos.**

**Modificadores de visibilidade** 

Um modificador de acesso determina como será a visibilidade de uma classe, método ou atributo a partir de outras classes.  

**Modificadores de acesso**

| Modificador     | Classe | Pacote | SubClasse | Mundo |
|-----------------|--------|--------|-----------|-------|
| public          | ✅      | ✅      | ✅         | ✅     |
| protected       | ✅      | ✅      | ✅         | ❌     |
| sem modificador | ✅      | ✅      | ❌         | ❌     |
| private         | ✅      | ❌      | ❌         | ❌     |

  * _public_: atributos e métodos são acessíveis __em todos os métodos de todas as classes__. Este é o __nível menos rígido de encapsulamento__, que dizemos que o encapsulamento é rompido. 
  * _protected_: atributos e métodos são acessíveis no pacote, __nos métodos da própria classe e suas subclasses__.  
  * _sem modificador_: a visibilidade nas __classes do mesmo pacote e a própria classe__. 
  * _private_: atributos e métodos são acessíveis __somente nos métodos da própria classe__. Este é o __nível mais rígido de encapsulamento__. 
  
 __Abstract__: Um método abstrato não implementa nenhuma funcionalidade, somente assina o método e faz com que a primeira subclasse concreta seja obrigada a implementar. Uma classe que possui um método abstrato deve ser obrigatoriamente abstrata, como vimos na aula passada. 

__Final__: Pode ser aplicado em classes, métodos e atributos. Indica que esta é a última atribuição ou definição da estrutura. Não será permitida uma nova re-escrita. Para uma classe, não há herança em classes final. Um método não pode ser sobrescrito; e um atributo é considerado uma constante. 

**Métodos Get’s e Set’s**

O método **set atribui valores** ao atributo, enquanto que o método **get obtém seus valores**. 
A composição do nome destes métodos é sempre com o **nome set + <nome atributo> ou get + <nome atributo>**

**Associação de Classes**

É um vínculo que permite que objetos de uma ou mais classes se relacionem. Através destes vínculos, é possível que um objeto troque mensagens ou chame os métodos de outros objetos.

**Composição**

Tipo de associação onde uma nova classe usa classes existentes como atributos;  
Relacionamento “tem um”. 
Ex.: uma conta tem um dono (cliente), um cliente tem um nome (string); 
Ex.: uma conta tem um dono (cliente), um cliente tem um nome (string);  