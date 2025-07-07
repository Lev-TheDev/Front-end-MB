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



