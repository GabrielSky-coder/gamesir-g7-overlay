GameSir G7 Pro Aimlabs — GamePad Viewer Skin V2
=====================================================

Esta V2 corrige principalmente:

1. LT/RT:
   - opacity:0 fica na regra base.
   - O GamePad Viewer pode alterar a opacity inline conforme o curso analógico.
   - Foi removida a variável CSS --trigger-opacity da versão anterior.

2. Analógicos:
   - Nenhum transform é imposto pelo skin.
   - Isso evita bloquear transformações/movimentação inline do GamePad Viewer.
   - As posições base ficam dentro do container .sticks.

3. ABXY:
   - Compatibilidade com .a/.b/.x/.y e .button.a/.button.b/.button.x/.button.y.
   - Estados ficam invisíveis em repouso e aparecem apenas em .pressed.

4. D-pad:
   - Cada direção tem seu PNG independente.
   - Sem deslocamento de margem quando pressionado.

5. LB/RB e View/Menu:
   - Invisíveis em repouso, aparecem apenas em .pressed.

6. Layout:
   - Tamanho fixo de referência: 420x326.
   - Fundo transparente para OBS.

COMO USAR
---------
Hospede todos os arquivos desta pasta no mesmo diretório público HTTPS.

Exemplo:
https://gamepadviewer.com/?p=1&css=https://SEU-DOMINIO/g7/style.css

Você também pode experimentar:
https://gamepadviewer.com/?p=1&nocurve=1&css=https://SEU-DOMINIO/g7/style.css

No OBS:
Width  = 420
Height = 326

IMPORTANTE
----------
A arte enviada é um PNG achatado. Portanto o base.png contém o controle inteiro,
e os outros PNGs funcionam como overlays transparentes de estado.

Se algum elemento aparecer 2-6 px fora do lugar no seu navegador/controle,
isso pode ser refinado depois do primeiro teste real no GamePad Viewer.
