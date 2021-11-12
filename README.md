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

### Scene
O _Scene_ é as configurações da cena como _Cor de Fundo_, para usar ou modificar uma configuração utilize _Dyka.scene.configuração()_

Configurações

background("cor") - define a cor de fundo da cena

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


Funções

para usar as funções do objeto só colocar _nomeDoObj.função()_

hover() - retorna true para quando o mouse estiver dentro do objeto

click() - retorna true para quando o objeto for clicado pelo mouse

colliding(**obj2**) - retorna true para caso o objeto esteja colidindo com o **obj2**

### Mouse
Na ***DykaEngine*** contém um objeto ***mouse*** que possuí os valores do cursor, para retornar um valor do objeto ***mouse*** coloque _Dyka.mouse.valor_

Valores

x - retorna o valor x

y - retorna o valor y

click - retorna true se o botão(qualquer botão) do mouse estiver pressionado

btn - retorna o botão usado quando o valor _click_ for true (botão esquerdo - 0, botão do meio - 1, botão direito - 2)

### Memory

A ***DykaEngine*** possuí uma função que salva uma _string_ ou uma _int_, _float_ na memória do navegador, para usar uma função do ***memory*** use _Dyka.memory.função()_

Funções

define("chave", "valor(string, int ou float") - salva um novo valor

locate("chave") - retorna um valor

remove("chave") - remove um valor
