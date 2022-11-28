Aqui é explicado um pattern derivado do design de código pelo olhar da teoria da carga cognitiva que chamamos de Controllers 100% coesos.

A ideia é que todo controller, por ser uma classe sem estado inteligente(atributos de dependência), seja 100% coeso. A ideia é que todos os atributos sejam utilizados por todos os métodos que são configurados para lidar com requisições para a aplicação. Perceba que não tem nada a ver com ter apenas um método. Você pode ter quantos quiser, portanto que respeite a restrição da coesão + limite de pontuação máxima para classes sem estado inteligente. 

Claro que em casos como o do Spring, onde a configuração da validação customizada é feita através de um método extra no próprio controller, quebra um pouco a coesão, mas a sugestão ainda vale. 

ps: você pode ler um pouco mais sobre coesão aqui(https://www.aivosto.com/project/help/pm-oo-cohesion.html#LCOM1​) 
