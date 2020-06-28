## Índice
- [Introdução](#introdução)
- [Capítulo 1: O Código Limpo](#capítulo-1:-o-código-limpo)
	- [O Código](#o-código)
	- [Código Ruim](#código-ruim)

## Introdução

"The only valid measurement of code quality: WTFs / minute."

A perfeição se encontra nos pequenos detalhes, mesmo no nome da mais isolada variável presente no código. Existe uma abordagem muito interessante, de origem japonesa, chamada Manutenção Produtiva Total (da sigla em inglês TPM ), onde o foco é a manutenção ao invés da produção em massa, baseada em um conjunto de princípios demoninado 5S:

- Seiri ("ordenar"): Saber onde estão as coisas, por exemplo, aplicar nomes significativos nas variáveis para facilitar sua localização e identificação mais tarde;

- Seiton ("sistematizar"): Um pedaço de código deve estar exatamente onde o autor ou quem está lendo espera encontrá-lo. Caso não esteja, é necessário que seja refatorado;

- Seiso ("polir"): Manter o local de trabalho limpo e organizado, não apenas os diretórios do projeto, mas o próprio local físico de trabalho, seja o quarto, o escritório, etc. No escopo de desenvolvimento, isso também significa deixar o código o mais limpo possível e livre de trechos desnecessários, como comentários com desejos futuros ou informações sobre o passado;

- Seiketsu ("padronização"): A concordância da equipe acerca da manutenção do workspace limpo e organizado;

- Shutsuke ("autodisciplina"): Disciplina para aceitar e seguir as práticas (e eventuais mudanças) e estar disposto à mudança.

	Existem duas "portas": a do good code e a do bad code. E atravessar uma
delas é reflexo da habilidade profissional, esteja ela presente ou ausente. Existem duas vertentes para se obter habilidade profissional: conhecimento e trabalho. É necessário não apenas adquirir o conhecimento teórico acerca de princípios, modelos, padrões, heurísticas, etc., mas também destrinchar esse conhecimento em um cenário prático, através do esforço e trabalho duro.
	É importante destacar que este livro não é trivial, como diz o próprio
autor, "não é um livro fácil e simples, que você pode ler num avião e terminar antes de aterrisar...". O caminho, como citado anteriormente, não é composto apenas da teoria, mas sim, de puro trabalho duro, por isso, é necessário muita prática acompanhada da leitura.
	O livro é dividido em três partes: na primeira, existem diversos
capítulos abordando a teoria sobre o código limpo, como princípios, padrões e práticas, além de muitas demonstrações de código; na segunda, o aprendizado será mais trabalhoso, pois serão abordados conceitos práticos de limpeza de código e o leitor será convidado a resolver diversos exercícios; a terceira, conforme descrita pelo autor como uma lista de "odores", abordará diversas heurísticas sobre identificação de focos para refatoração de código, ou seja, um "odor", em que tentaremos compreender nossas reações quando estivermos lendo ou alterando esse código.

## Capítulo 1: Código Limpo
	
### O Código

Algumas pessoas dizem que um dia a programação como conhecemos será extinta, ou seja, que todo código seria gerado automaticamente pelas máquinas de acordo com determinadas especificações e modelos, e não mais escrito manualmente. Confesso que eu mesmo também pensava assim até bem pouco tempo atrás, porém, nós nunca estaremos livre da programação em codificação, já que eles representam os detalhes dos requisitos. Especificar requisitos de modo que uma máquina consiga compreendê-los é programar, e a especificação é o código, e isso nunca irá mudar.

Esperar que, um dia, as máquinas alcancem um nível de comunicação com linguagem natural tão perfeita a ponto de uma simples especificação ser suficiente para gerar um programa executável perfeito e livre de inconsistências é como um matemático esperar que a matemática evolua tanto a ponto da formalidade da definição ser desnecessária. Isso jamais acontecerá, pois até mesmo os humanos, com toda sua criatividade e capacidade de adaptação e compreensão das "entrelinhas", não são capazes de criar sistemas de software que atendam de forma bem-sucedida aos requisitos confusos que os seus clientes por vezes definiram.

### Código Ruim

	
