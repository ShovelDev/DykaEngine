# DykaEngine

## Regras

### Inicie a Engine
Quando for usar a engine você precisa colocar no começo da tag _SCRIPT_ _initDyka()_

### Loop
Na **Dyka** você usa um tipo de game loop similar ao game loop que usa o _requestAnimationFrame()_ mais você coloca _Dyka.update(nome da function)_ <br>

Exemplo: <br>

_function loop(){_ <br>
 _**Dyka.update(loop)**_ <br>
_}_ <br>
_loop()_ <br>

### Prefixo
Todo script que você for fazer, caso seja um da DykaEngine coloque o prefixo dela(_Dyka_) antes do script <br>
Exemplo:<br>
_var player = new Dyka.obj(...)_ <br>
O unico script que você não precisa usar o prefixo é o _initDyka()_

### Tools
O _TOOLS_ é um conjunto de ferramentas que auxiliam na criação do mapa, ui, e sprites.

#### Tools/Print
O _Print_ serve para desenhar um texto na tela, você escreve o código da segunte maneira <br> _Dyka.print("Texto", PosX, PosY, Tamanho, "Cor", "Fonte(opicional)")_

### Objetos
Na **DykaEngine** possuí 1 tipo de objeto, com ele já é possivel fazer tudo, você precisa de um loop para criar um objeto.

**Syntax**

_var nomeDoObj = new **Dyka.obj(x, y, largura, altura, "cor", rotação(opicional))**_

Agora para desenhar o objeto na tela, dentro do loop coloque _nomeDoObj.add()_

Variáveis

para usar as váriaveis do objeto só colocar _nomeDoObj.váriavel_

X: x
Y: y
LARGURA: width
ALTURA: height
COR: color
ROTAÇÃO: rotation
SELF: self
