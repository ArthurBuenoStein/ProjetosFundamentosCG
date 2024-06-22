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

## M4

Adicionando o projeto M4 - Iluminação

Nesse projeto foi adicionado iluminação da Suzanne.

Esse código foi desenvolvido a partir do projeto do M3 e com o auxílio do projeto Hello3D Phong que a professora disponibilizou no repositório. A partir disso foi criado um vetor para armazenar os vertices normais do OBJ da Suzanne, foi lido do MTL as constantes necessárias para o modelo de iluminação Phong. No fragment shader foi usado as fórmulas passadas em aula para criar o efeito de iluminação.

## M5

Adicionado o projeto M5 - Camera

Nesse projeto foi adicionado uma câmera em primeira pessoa que pode ser rotacionada pelo mouse e movida via WASD no teclado.

Esse código foi evoluido do código de iluminação do M4, primeiramente configurando a câmera conforme visto em aula, criando uma classe Camera capaz de configurar os parâmetros e com funções auxiliares de movimentação e rotação. Além disso foi utilizada a classe Mesh disponibilizada no exemplo Hello3D Phong para deixar mais limpo e simples o código de como a Suzanne é renderizada em tela.

## M6

Adicionado o projeto M6 - Trajetórias

Nesse projeto foi adicionado uma trajetória na Suzanne a partir de uma interpolação bezier.

O código foi evoluido a partir do projeto de câmera do M5, adicionei as classes de curva disponibilizadas no projeto exemplo, estou entregando utilizando a classe Bezier no código, porém as outras classes estão disponíveis no código para alternar entre elas.

Os pontos de controle da trajetória são configurados a partir do arquivo config.txt na pasta animation, lá eles podem ser alterados e refletir no objeto. A trajetória da Suzanne é alterada a partir desse conjunto de pontos, que são lidos e iterados atualizando a posição do objeto dentro do loop principal.
