Dentro de uma aplicação web temos alguns tipos de classes diferentes. 

Controllers  
Services  
Classes que representam requests e responses  
Entidades  
Value objects  
Classes de configuração  
Classes que isolam código comum a toda aplicação  
Cada uma das classes listada acima aparecem em todo tipo de sistema. O problema é que com esse nível de granularidade fina, você sempre vai ter classes diferentes. Um jeito mais fácil de olhar é da seguinte forma:

Classes com atributos de dados(estado inteligente)  
Classes com atributos de dependência(sem estado inteligente)  
Classes sem nenhum atributo(apenas métodos estáticos mesmo, basicamente são funções)  
Classes com estado inteligente, geralmente têm manipulação de estado e são ​passíveis de terem mais lógica. Por isso a sugestão é deixá-las com um limite de 9 pontos.  

Classes sem estado inteligente, geralmente cuidam mais de fluxos, então a sugestão é limitar a 7 pontos.   

Voltando para uma aplicação web, temos a seguinte sugestão:  

Controllers com no máximo 7 pontos  
Services com no máximo 7 pontos  
Entidades com no máximo 9 pontos  
Classes de entrada e saída de dados com no máximo 9 pontos  
Classes de configuração e que isolam código para toda aplicação mais liberadas, já que são pouco mexidas.   
