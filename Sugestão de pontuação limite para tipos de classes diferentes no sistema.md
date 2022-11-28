Dentro de uma aplicação web temos alguns tipos de classes diferentes. 

1.Controllers  
2.Services  
3.Classes que representam requests e responses  
4.Entidades  
5.Value objects  
6.Classes de configuração  
7.Classes que isolam código comum a toda aplicação  

Cada uma das classes listada acima aparecem em todo tipo de sistema. O problema é que com esse nível de granularidade fina, você sempre vai ter classes diferentes. Um jeito mais fácil de olhar é da seguinte forma:

1.Classes com atributos de dados(estado inteligente)  
2.Classes com atributos de dependência(sem estado inteligente)  
3.Classes sem nenhum atributo(apenas métodos estáticos mesmo, basicamente são funções)  
4.Classes com estado inteligente, geralmente têm manipulação de estado e são ​passíveis de terem mais lógica. Por isso a sugestão é deixá-las com um limite de 9 pontos.  

Classes sem estado inteligente, geralmente cuidam mais de fluxos, então a sugestão é limitar a 7 pontos.   

Voltando para uma aplicação web, temos a seguinte sugestão:  

1.Controllers com no máximo 7 pontos  
2.Services com no máximo 7 pontos  
3.Entidades com no máximo 9 pontos  
4.Classes de entrada e saída de dados com no máximo 9 pontos  
5.Classes de configuração e que isolam código para toda aplicação mais liberadas, já que são pouco mexidas.   
