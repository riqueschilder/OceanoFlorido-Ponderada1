
comandos:

#inicia o turtlesim
ros2 run turtlesim turtlesim_node
#executa o arquivo .py
python3 turtle.py

Turtle.py:

código Python que controla o movimento da tartaruga (turtlesim) simulada em um ambiente ROS 2. O código faz uso das bibliotecas rclpy, que é a biblioteca de cliente para ROS 2, e da mensagem de geometria "Twist". Alem de importar Time.

A classe "TurtleController" é criada como um nó ROS 2 que publica mensagens Twist para o tópico "turtle1/cmd_vel". O método "move_turtle" é chamado pelo temporizador criado na inicialização da classe e controla o movimento da tartaruga em diferentes velocidades lineares e angulares, em um padrão repetitivo.

Ao executar o programa, a tartaruga se moverá em um padrão circular, onde ela se moverá para a frente e girará para a esquerda em um meio ciclo, depois se moverá para frente novamente e girará para a esquerda em outro ciclo, e repetirá esse padrão 12 vezes, formando 12 petalas de uma flor. Em seguida, a tartaruga se moverá em uma reta com uma curva suave para a esquerda para sair da area da primeira flor e começar outra, assim formando um oceano florido.

