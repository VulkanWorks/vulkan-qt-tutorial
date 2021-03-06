# Aplicações gráficas interativas com Vulkan e Qt

Neste repositório, fornecemos um guia introdutório para o desenvolvimento de aplicativos gráficos interativos usando Vulkan e Qt.

<p align="center">
  <img width="536" height="480" src="https://user-images.githubusercontent.com/3193712/85233784-644bf580-b3df-11ea-9b64-c451106dac10.gif">
</p>

Todo conteúdo deste repositório pode ser acessado em [https://gustavohb.github.io/vulkan-qt-tutorial-site/](https://gustavohb.github.io/vulkan-qt-tutorial-site/).

Os arquivos contendo todo código do programa estão organizados na pasta `code`. Cada subpasta deste diretório contém o código por capítulo.

O código apresentado neste repositório é baseado no tutorial de Vulkan escrito por Alexander Overvoorde disponível em [https://vulkan-tutorial.com/](https://vulkan-tutorial.com/). Este tutorial, além de cobrir boa parte do que veremos, também trata do uso de *index buffer*, mapeamento MIP e *multisampling*, que não trataremos aqui. Por outro lado, cobriremos alguns tópicos que não são cobertos nele, como iluminação local e implementação de um *trackball* virtual. Além disso, trataremos de especifidades do Qt, como criação de janela, uso de suas classes auxiliares para criação e gerenciamento de recursos do Vulkan, e uso de seu sistema interno de eventos. Para aprender mais sobre Vulkan, recomendamos que o leitor também consulte o material escrito por Overvoorde.

---

* [Introdução](https://gustavohb.github.io/vulkan-qt-tutorial-site/)
* [Vulkan e Qt](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt)
   * [Sobre Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt/sobre-vulkan)
     * [Comparação entre Vulkan e OpenGL](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt/sobre-vulkan/comparacao-entre-vulkan-e-opengl)
     * [Objetos Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt/sobre-vulkan/objetos-vulkan)
   * [Sobre Qt](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt/sobre-qt)
   * [Comparação do Qt com OpenGL e o Qt com o Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/vulkan-e-qt/comparacao-do-qt-com-opengl-e-o-qt-com-o-vulkan)
* [Inicializando um projeto no Qt com Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan)
  * [Preparando o ambiente de desenvolvimento](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/preparando-o-ambiente-de-desenvolvimento)
  * [Instância, janela e renderizador Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/instancia-janela-e-renderizador-vulkan)
  * [Criando o projeto Vulkan mínimo](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/criando-o-projeto-vulkan-minimo)
  * [Selecionando um dispositivo físico](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/selecionando-um-dispositivo-fisico)
  * [Acessando comandos principais do Vulkan](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/acessando-comandos-principais-do-vulkan)
  * [Camadas de validação e *logs*](https://gustavohb.github.io/vulkan-qt-tutorial-site/inicializando-um-projeto-qt-com-vulkan/camadas-de-validacao-e-logs)
* [Renderizando um triângulo](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo)
  * [Pipeline gráfico](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/pipeline-grafico)
     * [*Shaders*](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/pipeline-grafico/shaders)
     * [Estágios de função fixa](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/pipeline-grafico/estagios-de-funcao-fixa)
     * [Criação do *pipeline* gráfico](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/pipeline-grafico/criacao-do-pipeline-grafico)
  * [Iniciando um *render pass*](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/iniciando-um-render-pass)
  * [*Viewport* e *scissor*](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/viewport-e-scissor)
  * [Comandos básicos de desenho](https://gustavohb.github.io/vulkan-qt-tutorial-site/renderizando-um-triangulo/comandos-basicos-de-desenho)
* [Usando *buffer* de vértice](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice)
  * [Acessando o *buffer* de vértice no *vertex shader*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/acessando-o-buffer-de-vertice-no-vertex-shader)
  * [Dados de vértice](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/dados-de-vertice)
  * [Abstraindo a criação de *buffer*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/abstraindo-a-criacao-de-buffer)
  * [Criação do *buffer* de vértices](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/criacao-do-buffer-de-vertices)
  * [Descrições de ligações](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/descricoes-de-ligacoes)
  * [Descrições de atributos](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/descricoes-de-atributos)
  * [Entrada de vértice do *pipeline*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/entrada-de-vertice-do-pipeline)
  * [Vinculando o *buffer* de vértice](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-buffer-de-vertice/vinculando-o-buffer-de-vertice)
* [Usando texturas em shaders](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders)
  * [Carregando uma imagem](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/carregando-uma-imagem)
  * [Copiando dados de uma imagem para um *staging* buffer](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/copiando-dados-de-uma-imagem-para-um-staging-buffer)
  * [Imagem de textura](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/imagem-de-textura)
  * [Transições de *layout*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/transicoes-de-layout)
  * [Copiando o *buffer* para a imagem](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/copiando-o-buffer-para-a-imagem)
  * [Preparando a imagem de textura](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/preparando-a-imagem-de-textura)
  * [Criando uma *image view*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/criando-uma-image-view)
  * [Criando um *sampler*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/criando-um-sampler)
  * [Conjuntos de descritores](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/conjuntos-de-descritores)
  * [Coordenadas de textura](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/coordenadas-de-textura)
  * [Modificando os *shaders*](https://gustavohb.github.io/vulkan-qt-tutorial-site/usando-texturas-em-shaders/modificando-os-shaders)
* [Utilizando uniform buffers em shaders](https://gustavohb.github.io/vulkan-qt-tutorial-site/utilizando-uniform-buffers-em-shaders)
  * [Matrizes MVP e uniform buffer](https://gustavohb.github.io/vulkan-qt-tutorial-site/utilizando-uniform-buffers-em-shaders/matrizes-mvp-e-uniform-buffer)
  * [Criando o *uniform buffer*](https://gustavohb.github.io/vulkan-qt-tutorial-site/utilizando-uniform-buffers-em-shaders/criando-o-uniform-buffer)
  * [Atualizando os dados *uniform*](https://gustavohb.github.io/vulkan-qt-tutorial-site/utilizando-uniform-buffers-em-shaders/atualizando-os-dados-uniform)
  * [Atualizando os descritores](https://gustavohb.github.io/vulkan-qt-tutorial-site/utilizando-uniform-buffers-em-shaders/atualizando-os-descritores)
* [Carregando modelos 3D](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d)
  * [Geometria 3D](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/geometria-3d)
  * [Integrando a biblioteca tinyobjloader no projeto](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/integrando-a-biblioteca-tinyobjloader-no-projeto)
  * [Carregando vértices do modelo](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/carregando-vertices-do-modelo)
  * [*Signals* e *slots* do Qt](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/signals-e-slots-do-qt)
  * [Habilitando o teste de profundidade](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/habilitando-o-teste-de-profundidade)
  * [Carregando texturas dinamicamente para o modelo 3D](https://gustavohb.github.io/vulkan-qt-tutorial-site/carregando-modelos-3d/carregando-texturas-dinamicamente-para-o-modelo-3d)
* [Adicionando mais recursos ao projeto](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto)
  * [Iluminação básica](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/iluminacao-basica)
     * [Trabalhando com um modelo de iluminação local](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/iluminacao-basica/trabalhando-com-um-modelo-de-iluminacao-local)
     * [Modelo de reflexão de Phong](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/iluminacao-basica/modelo-de-reflexao-de-phong)
     * [Phong *shading*](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/iluminacao-basica/phong-shading)
     * [Implementação do modelo de Phong e o Phong shading](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/iluminacao-basica/implementacao-do-modelo-de-phong-e-o-phong-shading)
  * [*Trackball* virtual](https://gustavohb.github.io/vulkan-qt-tutorial-site/adicionando-mais-recursos-ao-projeto/trackball-virtual)
* [Conclusão](https://gustavohb.github.io/vulkan-qt-tutorial-site/conclusao)

## Licença

Consulte o arquivo [LICENÇA](https://github.com/gustavohb/vulkan-qt-tutorial/blob/master/LICEN%C3%87A) para obter os direitos e limitações da licença (MIT)
