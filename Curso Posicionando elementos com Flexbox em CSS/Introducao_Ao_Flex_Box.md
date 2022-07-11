# Flex Box
Foi projetado como um modelo de layout unidimencional e como um método que pode oferecer didtribuição de espaço entre itens em uma interface e recursos de alinhamento.

# Flex Container
É a tag que envolve os itens, será nela que iremos aplicar a propriedade **"display: flex"**. Transforma todos os seus itens filhos em flex itens.

# Flex Item 
São os elementos filhos diretos do flex Container. E também podem se torna Flex Container.

# Display: flex;
Torna a tag um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos desta tag, tornam-se em flex itens.

# Flex-direction
É a propriedade que estabelece o eixo principal do container, definindo assim a direção que o flex itens são colocados no flex container.

# Flex-wrap
É a propriedade que define se os itens devem ou não quebrar a linha.
Por padrão eles não quebram linhas, isso faz com que os flex itens sejam compactados além do limite do conteúdo.
- **nowrap:** é o padrão, não permite a quebra de linha.

- **wrap:** permite a quebra de linha assim que um dos flex itens não puder mais ser compactado.

- **wrap-reverse** permite a quebra de linha assim que um dos flex itens não puder mais ser compactado, porém na direção contrária da linha, acima.

# Flex-flow
É um atalho para as propriedades **flex-direction** e **flex-wrap.**
Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

# Justify Content
Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.

**OBS:** caso seus itens esteja ocupando 100% de todo o container, ela não se aplica.

##                                   As variações

- **flex-start:** início do container.
- **flex-end:** final do container.
- **center:** ao centro do container.
- **space-between:** cria um espaçamento igual entre os elementos.
- **space-around:** os espaçamentos do meio são duas vezes maiores que o inicial e final.

# Align-items
Trata do alinhamento dos flex itens de acordo com eixo do container.
O alinhamento é diferente para quando os itens estão em colunas ou linhas.
Permite o alinhamento central no eixo vertical.

##                                  Tipos de Alinhamento
- **center:** alinhamento dos itens ao centro
- **stretch:** padrão, e os flex intens creçam igualmente 
- **flex-start:** alinhamento dos itens no início
- **flex-end:** alinhamento dos itens no final
- **baseline:** alinhamento de acordo com a linha base da tipografia dos itens

# Align-content
É a propriedade responsável por tratar o alimhamento das linhas do container em relação ao eixo vertical do container.
Precosamos que:

- O container utilize quebra de linhas
- A altura do container seja maior que a soma das linhas dos itens

##                                  Tipos de Alinhamento
- **center** alinhamento dos itens ao centro
- **stretch:** é o padrão e os flex itens crescem igualmente
- **flex-start:** alinhamento dos itens no início
- **flex-end:** alinhamento dos itens no final
- **space-between:** cria um espaçamento igual entre os elementos
- **space-around:** os espaçamentos do meio são duas vezes maiores que o inicial e final

# flex-grow
Define a proporcionalidade de crescimento dos itens, respeitando o tamanho de seus conteúdos internos.
**OBS:** não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.

# Flex-basis
É a propriedade que estabelece o tamanho inicial do item antes das distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

##                                  Valores possíveis
- **Auto:** caso o item não tenha tamanho, este será prporcional ao conteúdo do item.
- **px, %, em, ...:** são valores exatos previamente definidos
- **0(zero):** terá relação com a definição do flex-grow.

# Flex-shrink
É a propriedade que estabelecer a capacidade de redução ou compressão do tamanho de um item.

# FLex
Esta propriedade é um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis.

# Align-self
É a propriedade que estabelece o alinhamento de modo individual sobre um determinado item.

##                                  Valores possíveis
- **auto:** valor padrão,irá respeitar a definição de align-items do container
- **flex-start:** ao início do container
- **flex-end:** ao final do container
- **center:** relativo ao centro de acordo com o eixo
- **stretch:** ocupa todo o espaço relativo
- **baseline:** utiliza a linha base da tipografia