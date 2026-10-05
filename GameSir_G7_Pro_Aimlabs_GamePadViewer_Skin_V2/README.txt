GameSir G7 Pro Aimlabs - GamePad Viewer Custom Skin
========================================================

Pacote criado a partir da imagem enviada (420x326).

ARQUIVOS
--------
- base.png                    arte principal
- stick_left_pressed.png      clique do analógico esquerdo
- stick_right_pressed.png     clique do analógico direito
- button_a_pressed.png
- button_b_pressed.png
- button_x_pressed.png
- button_y_pressed.png
- dpad_up_pressed.png
- dpad_down_pressed.png
- dpad_left_pressed.png
- dpad_right_pressed.png
- lb_pressed.png
- rb_pressed.png
- lt_pressed.png
- rt_pressed.png
- view_pressed.png
- menu_pressed.png
- style.css

COMO PUBLICAR
-------------
1. Coloque TODOS os arquivos na mesma pasta pública na web.
2. Garanta que style.css e todos os PNGs tenham URL HTTPS pública.
3. Abra o GamePad Viewer usando o parâmetro css apontando para o style.css.

Exemplo:
https://gamepadviewer.com/?p=1&css=https://SEU-DOMINIO/skins/gamesir-g7/style.css

OBS / STREAMLABS
----------------
Adicione a URL do GamePad Viewer como Browser Source.
Sugestão inicial:
- Width: 420
- Height: 326
- Background: transparente

IMPORTANTE
----------
Este pacote usa a imagem original como camada de base e adiciona sprites transparentes
por cima para os estados pressionados. Isso evita degradar a arte e permite alinhar
os estados visualmente com o controle.

Como a imagem fornecida é um screenshot/raster único, os elementos originais não
existem como camadas independentes. Os PNGs extras deste pacote são overlays
transparentes para os estados pressionados.

AJUSTE FINO
-----------
Dependendo do template interno que o GamePad Viewer estiver usando, 2 a 6 pixels de
ajuste podem ser necessários em left/top para algum botão. Os pontos principais já
foram posicionados com base na imagem de 420x326.

LT/RT
-----
O CSS está preparado para overlay visual dos gatilhos. O comportamento de pressão
analógica depende de como a versão atual do GamePad Viewer aplica opacity/style ao
elemento .trigger.

Percentual numérico dinâmico (por exemplo 37%) não pode ser calculado apenas por CSS.
Para isso seria necessário um overlay HTML/JavaScript próprio.
