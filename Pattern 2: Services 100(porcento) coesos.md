Aqui é explicado um pattern derivado do design de código pelo olhar da teoria da carga cognitiva que chamamos de Services 100% coesos.

A ideia é que todo service, por ser uma classe sem estado inteligente(atributos de dependência), seja 100% coeso. A ideia é que todos os atributos sejam utilizados por todos os métodos que são configurados para lidar com requisições para a aplicação. Perceba que não tem nada a ver com ter apenas um método. Você pode ter quantos quiser, portanto que respeite a restrição da coesão + limite de pontuação máxima para classes sem estado inteligente.

Num cenário de controllers 100% coesos, o service geralmente aparece em duas situações:

1.O limite de 7 pontos do controller foi estourado e você precisa dividir a responsabilidade. Geralmente essa classe nova tende a ser um service do DDD  
2.A entrada de dados do sistema não é feita apenas pela web e agora você mais de um ponto de entrada. O código pode ser isolado para ser reaproveitado. Geralmente essa classe também vai ser um Service do DDD. 
