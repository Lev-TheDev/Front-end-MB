# Anotações Front-End

- **HTML**:

Linguagem de marcação; objetivo = estruturar páginas web; esqueleto de uma página web; botão direito, inspecionar = serve para pegar dicas de outras páginas para estilizar a sua;

- **CSS**:
Linguagem de estilização de sites; cores, tamanhos de fonte, bordas de elementos, etc; aplicar regras a elementos; utilizado em conjunto com html; "styles";

- **Editor de código**:
Visual Studio Code; extensões, pluggins;
Index.html = arquivo principal de uma aplicação;
Ir até a pasta do arquivo, botão direito, abrir com Chrome;
Tag h1 = heading, usada para títulos;

- **TAG**:
Quando se coloca qualquer elemento dentro do sinal de menor e maior (<>); toda TAG tem nome e propósito; [<p>Texto</p>] = isso cria um elemento de parágrafo.

- **ESTRUTURA HTML**:
1. DOCTYPE: declara versão do HTML; não aparece, está intrínseca;
2. hmtl: envolve todo o código;
3. head: colocamos configurações de um site, como importação do CSS e título (meta tags);
4. body: onde todos os elementos visíveis estão;

- **Títulos**:
São conhecidos como `headings`, utilizado para separar seções, tag h* (* = 1 a 6);
Estilo não é um fator importante, o que determina a importância é a tag, um h1 sempre será mais importante na página do que um h3 paesar de às vezes por estilo poder ser menor em tamanho;

- **Parágrafos**:
Tag `<p>` cada parágrafo começa uma nova linha;

- **Tags sem conteúdo**:
Possuem recursos como `quebrar linha` (`<br/>`), para linha horizontal (`<hr/>`), não possuem tag de fechamento.

- **Comentários no HTML**:
Não aparecerão na página, mas poderão ser acessados na ferramenta `inspecionar`;
Utilizado para separar seções de sites;

- **Atributos**:
Servem para adicionar funcionalidades às tags;
1. A tag `a` nos direciona a uma nova página ou site (`ancor`), o endereço ou URL é adicionado no atributo `href`:
`<a href="https://www.google.com">Google</a>`
2. Adicionar ao body um atributo chamado style para adicionar espaçamento inferior `style="padding-bottom: 500px"`;
3. Outro atributo para a tag `a` é `target` com o valor `_blank`, que faz com que o link abra em nova página;

- **Imagens**:
Tag `img`; o caminho relativo at[e a imagem [e inserido no ATRIBUTO `src`;
Colocamos imagens na pasta `img` ou `assets`;
Imagem é uma SELF CLOSING TAG (não tem tag de fechamento);

- **Atributo ALT**:
Nas tags de imagem temos um atributo chamado `ALT`; inserimos nele um texto que descreve a imagem;
Todas as img devem ter esse atributo configurado;
Importante para acessibilidade e rankeamento do site pelo Google;
É uma descrição da img e, mesmo que a img não apareça (tenha sumido do servidor) a descrição `alt` aparecerá;

- **Lista não ordenadas**:
Pode-se até criar um menu a partir de uma lista;
Criadas pela Tag `ul` (unordered list); cada item representado pela tag `li` (list item);

- **Lista ordenadas**:
Utilizadas para procedimentos ou passos (receitas, algoritmos de programação);
Criadas pela tag `ol`, itens tag `li`;

- **Tabelas**:
Categorizadas em colunas, são complexas, não tão utilizadas;
Tag `table` cria a tabela, um cabeçalho (coluna e nomes delas) e um corpo (dados);
Cada linha criada em uma tag `tr`, dados em um `td`;
No cabeçalho a tag `th`;
Ordem das `tr` de cima para baixo;

- **DIV**:
Cria divisões ou seções no site;
Criar elementos menores como cards;
Propósito: encapsular elementos conectados entre si (cria um componente);
Não tem valor semântico, é um contêiner, delimita elementos dentro dela para controlar CSS daquela divisão mais fácil;

- **Estrutura base**:
Iniciar VSCode, digitar `!` e apertar `Tab`;
Cria automaticamente uma estrutura `html`;

- **CSS**:
-Maneira de adicionar o CSS ao HTML:
1. Inline: estilos adicionados por um atributo;
2. Internal: CSS adicionado na tag head; consegue atingir mais elementos de uma vez só;
3. External: CSS adicionado através de um arquivo externo e depois importado ao HTML.

- **Anatomia do CSS**:
Aplicamos CSS a um elemento; seleciona o elemento primeiro, através da tag, depois colocar propriedades e valores;
1. Propriedades: tudo que podemos mudar no elemento (cor, tamanho de fonte, altura, largura, borda);
2. Valor: valor que vai alterar a propriedade, como ela vai ficar após alteração;
color: red; (propriedade: valor;).

- **Inline CSS**:
Pode ser adicionado sem selecionar elemento;
Atributo `style` nos permite escrever as regras do CSS;
Exemplo: `style="color: red;"`

- **Múltiplas regras no CSS**:
Podemos adicionar várias regras separadas por ponto e vírgula, gerando união de estilos;

- **Internal CSS**:
Técnica melhor que inline; colocar todos os estilos na tag `head`; `<style></style>` no head, colocar a tag no lugar dela `<p></p>` ou `<h1></h1>` ou outra, depois chamar (como apontado abaixo no texto) lá no head;
Regras também precisam estar entre a tag `style`;
Desta maneira, é necessário selecionar o elemento alvo:
```
 p {
      color: red;
 }
```
 
- **External CSS**:
Para adicionar CSS nesse formato é necessário criar um arquivo `.css`, numa pasta chamada `css`;
Deve ser importada por nós com a tag `link`;
 
- **Ordem do CSS**:
Inline > Internal = External > padrão do navegador; isso vale para um mesmo elemento, para elementos diferentes, carrega todas normalmente;
Entre Internal e External, a última aplicada será a carregada; verificar a ordem da chamada no `index.html`;

- **Múltiplos arquivos do CSS**:
É possível ter mais de uma folha de estilo no mesmo projeto;
Todas precisam ser importadas na tag `head`;
Os importados por último tem prioridade;
Boa prática: possibilita a divisão de CSS por páginas;

- **Desafio 2 do CSS**:
crie arquivo css titles.css
importe para o html
estilize os h4
crie h4 no html

- **Classes e Ids**:
São atributos de tags do HTML, relacionadas ao CSS;
Ids são usados para elementos únicos; classes servem para um ou mais; Id único na página;

- **Classes**:
Inseridas por atributo de HTML;
Valor do atributo é o nome da classe; [ex.: classe btn para botão que aparece x vezes no projeto]
Para elementos que se repetem;

- **Ids**:
Atributos do HTML;
Para elemento único, não repete o nome para a mesma página; pode ter dois IDs diferentes;

- **Ordem dos seletores**:
Se a tag tiver vários atributos, ordem: `id > class > seletor de tag`;

- **Cores no CSS**:
Nomes, RGB, Hexadecimal, HSL;
HEX: consiste em inserir 6 dígitos ; vermelho, verde, azul; 0 a 9, A a F; 
RGBA: A vem de alpha; muda opacidade da cor; valores do A de 0 (transparente) a 1 (totalmente visível); sintaxe = rgba(34, 207, 153, 0.67)
HSL: Hue, Saturation, Lightness;
BACKGROUND COLOR: sintaxe = `background-color: "cor";`
BACKGROUND OPACITY = valores de 0(invisível) a 1 (totalmente visível) `opacity`;
__Dica__ = alterando o "a" do RGBA tem-se a opacidade apenas na cor de fundo, não em todo o conteúdo;

- **BG Images**:
Regra = `background-image: url("pasta/imagem.jpg")`;
Centralizar img no bg = `background-position: center` ou `background-size: cover`;

- **Box Model**:
__Quatro partes__:
1. Altura e Largura = conteúdo do elemento, muda tamanho do elemento na tela, alguns elementos tem largura block `block elements` em 100%;
2. Padding (espaçamento interno do elemento, para letras não ficarem muito próximas da extremidade do elemento p. ex.) = espaço entre conteúdo e borda do elemento, distância entre conteúdo (texto) e extremidade do elemento;
Padding individual = `padding-top` (left, right, bottom);
3. Border (elemento decorativo, pode ou não ser adicionado);
4. Margin (espaçamento externo, distância de um elemento a outro);

- **Shorthand Properties**:
Adicionar paddings a todas as direções com uma regra (top, right, bottom, left);
Regra = `padding: 10px 5px 12px 20px`;
Shorthand também pode ser aplicada a `margin`;

- **Padding e Width**:
Padding é adicionada a largura do elemento, que pode ser um problema;
Se um elemento tem 200px de width e 25px de padding, tamanho horizontal total seria 250px;
Resolve-se com a regra `box-sizing` e o valor de `border-box` = elemento vai respeitar o tamanho que está em width!
Padding é incluído dentro do valor da largura;

- **Bordas**:
Elemento central entre padding e margin; decorativo;
Regra definida em = tamanho; aspecto; cor da borda;
Borda arredondada = `border-radius: 5px`;

- **Margin**:
Espaçamento externo do elemento; lados individuais e shorthand também são possíveis;

- **Alinhamento de texto**:
Padrão = à esquerda;
Regra = `text-align` podemos configurar `center` ou `right`;

- **Text Decoration**:
Efeitos ao texto;
Underline, linha que corta o texto;
A tag `a` tem um `underline` por padrão; pode ser removida com text decoration;

- **Text Transform**:
Altera como o texto é exibido; uppercase / lowercase;
Cuidado: **O CSS deve ser aplicado quando queremos texto `uppercase`, nunca escreva o texto com `CAPSLOCK` no HTML;

- **Espaçamento de letras**:
Regra = `letter-spacing: 5px`;

- **Fontes**:
Regra = `font-family`;
Opções = `Serif, Sans-serif, Monospace, Cursive, Fantasy`;
É possível adicionar fontes externas, por exemplo com Google Fonts;
Propriedade = `font-style` para mudar o aspecto das letras; 
Valores = `normal`, `italic` e `oblique`;

- **Font weight**:
Deixa mais fina ou grossa a fonte; valores de 100 a 900; bold = 600;

- **Font size**:
Base em `16px`;

- **Display**:
Elementos são `block` ou `inline`; `block` ocupa a linha toda, `inline` ficam os elementos um do lado do outro;
Tag `div` é `BLOCK` e a tag `span` é `INLINE`;
Com a regra `display` podemos mudar este comportamento;

- **Escondendo elemento**:
Ocultar = regra `display: none`;
Ainda consta no html, mas fica oculto;
A principal diferença é que `display: none` remove o elemento completamente do fluxo do documento, sem ocupar espaço, enquanto `visibility: hidden` o esconde visualmente, mas mantém o espaço que ele ocuparia na página. O `display: none` é usado quando você quer que outros elementos ocupem o espaço do elemento oculto, já `visibility: hidden` é útil se você precisa esconder o conteúdo, mas preservar a estrutura da página.

- **Positions dos elementos**:
Possibilidades: relative, fixed, absolute, sticky e mais;
Padrão = `static`;

- **Position static**:
Por ser padrão, não altera o elemento;
Se for `static`, não se alterará com valores `top, left, right, bottom`;

- **Position relative**:
Valores `top, left, right, bottom` movem o elemento pela tela; segue o fluxo do HTML ainda;
Não usamos esses valores de position com `relative` normalmente;

- **Position absolute**:
Valores `top, left, right, bottom` movem o elemento pela tela TODA;
QUEBRA o fluxo do HTML;
Não usamos esses valores de position com `relative` normalmente;

- **Position relative com absolute**:
Elemento com position `absolute` se liga ao elemento mais próximo com position `relative`, se não ele se liga ao `body`;
Usando container com posição `relative` podemos controlar melhor a área de ação do `absolute`;

- **Position fixed**:
Elemento permanece na mesma posição, mesmo após `scroll`;

- **Position sticky**:
Também fixa na tela;
Mas quando elemento volta à sua posição original ele se comporta como `relative`;
A posição original é onde ele foi inserido no HTML;

- **Z-index**:
Se dois elementos ocuparem a mesma posição ou colidirem, podemos escolher qual será exibido;
Elemento com MAIOR VALOR permanece;
Padrão = prevalece acima dos outros elementos quem está mais abaixo do HTML;
