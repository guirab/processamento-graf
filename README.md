# P: O que é a GLSL? Quais os dois tipos de shaders são obrigatórios no pipeline programável da versão atual que trabalhamos em aula e o que eles processam? 
R: GL Shading Language é uma linguagem de programação usada para o desenvolvimento de shaders dentro da pipeline do OpenGL, sendo obrigatório estágio de Vertex shading(processa cada vértice separadamente) e estágio de Fragment shading(processa cada fragmento separadamente).
# P: O que são primitivas gráficas? Como fazemos o armazenamento dos vértices na OpenGL?
R: As primitivas gráficas são "dicas" que passamos para o OpenGL em um comando de desenho, como GL_POINTS, GL_TRIANGLES... O armazenamento é feito em um buffer.
# P: Explique o que é VBO, VAO e EBO, e como se relacionam (se achar mais fácil, pode fazer um gráfico representando a relação entre eles). 
R: 
	VBO -> Vertex Buffer Objects é um array de dados(geralmente float) que envia dados dos vértices para a GPU, sendo alocados diretamente na memória da GPU, permitindo que os objetos sejam renderizados pela placa gráfica com maior velocidade.
	VAO -> Vertex Array Objects tem como objetivo fazer a ligação dos atributos dos vértices(posição, cores, normais). Além disso, qual VBO será usado, onde estão e qual o formato deles.
	EBO -> Element Buffer Objects é um buffer, assim como um VBO, que armazena índices que o OpenGL usa para decidir quais vértices desenhar.


