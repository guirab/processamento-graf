P: O que � a GLSL? Quais os dois tipos de shaders s�o obrigat�rios no pipeline program�vel da vers�o atual que trabalhamos em aula e o que eles processam? 
R: GL Shading Language � uma linguagem de programa��o usada para o desenvolvimento de shaders dentro da pipeline do OpenGL, sendo obrigat�rio est�gio de Vertex shading(processa cada v�rtice separadamente) e est�gio de Fragment shading(processa cada fragmento separadamente).
P: O que s�o primitivas gr�ficas? Como fazemos o armazenamento dos v�rtices na OpenGL?
R: As primitivas gr�ficas s�o "dicas" que passamos para o OpenGL em um comando de desenho, como GL_POINTS, GL_TRIANGLES... O armazenamento � feito em um buffer.
P: Explique o que � VBO, VAO e EBO, e como se relacionam (se achar mais f�cil, pode fazer um gr�fico representando a rela��o entre eles). 
R: 
	VBO -> Vertex Buffer Objects � um array de dados(geralmente float) que envia dados dos v�rtices para a GPU, sendo alocados diretamente na mem�ria da GPU, permitindo que os objetos sejam renderizados pela placa gr�fica com maior velocidade.
	VAO -> Vertex Array Objects tem como objetivo fazer a liga��o dos atributos dos v�rtices(posi��o, cores, normais). Al�m disso, qual VBO ser� usado, onde est�o e qual o formato deles.
	EBO -> Element Buffer Objects � um buffer, assim como um VBO, que armazena �ndices que o OpenGL usa para decidir quais v�rtices desenhar.


