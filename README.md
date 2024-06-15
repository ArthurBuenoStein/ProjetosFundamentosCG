# ProjetosFundamentosCG - Computação Gráfica
 
Aluno: Arthur Bueno Stein

## M1

Seguindo como base o exemplo passado na tarefa e fazendo as alterações solicitadas.

Execução do Hello3D com as pirâmides, rotação nos eixos e alteração da nome da janela.

## M2

O projeto M2 - Cubo foi adicionado.

Esse projeto foi baseado na pirâmide. Primeiro, o vetor de vértices e a função de desenhar triângulos foram alterados para representar um cubo.

Após isso, o glm:scale e o glm:translate foram usados para criar funcionalidades de escala e translação. permite alterar a escala do cubo e move-lo a partir do teclado.

Finalmente, foi modificado o vertexShader, alterada a função de desenho para ser uma função com instâncias e alterado o método setupGeometry para incluir um segundo VBO que regula as instâncias.

## M3

O projeto M3 com as texturas foi adicionado.

Suzanne recebeu texturas neste projeto.

Eu decidi não mudar do projeto vivencial porque achei que seria melhor para o objetivo da atividade após ver o projeto de exemplo do HelloTextures. O vertex shader e o fragment shader estão separados em outros arquivos, o que facilita a leitura do código. Além disso, a base já suporta o carregamento de texturas.

Além disso, refatorei o método loadOBJ para adaptá-lo à atividade e eliminei o uso de recursos deprecateds, como o fscanf. Foi adicionada uma função para ler arquivos.mtl também.
