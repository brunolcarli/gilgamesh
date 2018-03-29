<h1 align="center">Gilgamesh: Um conto épico</h1>
<br/>
<h2 align="center"> Game Design Document</h2>
<br/>
<h3 align="center"> Versão 0.9</h3>
<br/>
<br/>
<h4 align="center">Autor:</h4>

<h6 align="center">Bruno Luvizotto Carli</h6>

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

<h5 style="color:#ff0000;" align="center"><b><i>Documento em construção</i></b></h5>

<br/>
<hr>
<br/>

# Sumário

- Prefácio
- Escopo do Projeto
- Objetivos
- Requisitos
- História
- Gameplay
- Personagens
- Universo do jogo
- Inimigos
- Interface
- Cutscenes
- Cronograma
- Anexos
- Referências






## Prefácio:

Este documento descreve as características relativas ao desenvolvimento do jogo digital A Aventura de Gilgamesh como produto de software. Desta forma pretende-se elucidar os aspectos técnicos do processo comum de desenvolvimento e software. Esta primeira versão (1.0) é um esboço do projeto que deve ser seguido como orientação no processo de desenvolvimento. Também é objetivo deste documento servir como registro do processo de desenvolvimento do produto e descrição das características do software.

## Escopo e Descrição do Processo:

Gilgamesh: um conto épico é um Software de Computador Pessoal (PRESSMAN, 2010), mais especificamente um jogo digital, descrevendo acontecimentos da Epopéia de Gilgamesh, e incrementada com novas aventuras e novos personagens, como Alfr, um caçador  que  ajuda Gilgamesh, o rei da cidade de Uruk, em sua jornada, e Skulda, uma misteriosa Feiticeira que se diz designada a ajudar Gilgamesh em suas empreitadas. O game mistura a trama da saga com a fantasia que permeia o universo do RPG, enaltecendo o caráter old school do game. 
Na escolha de um modelo de desenvolvimento optou-se pela prototipação, pois Segundo Pressman (2010):

 >A prototipação é um processo que capacita o desenvolvedor a criar um modelo do software que será implementado. O modelo pode assumir uma das três formas: (1) um protótipo em papel ou modelo baseado em PC que retrata a interação  homem-máquina de uma forma que capacita o usuário a entender quanta interação ocorrerá; (2) um protótipo de trabalho  que implementa algum subconjunto da função exigida do software desejado; ou (3) um programa existente que executa parte ou toda a função desejada, mas que tem outras características que serão melhoradas em um novo esforço de desenvolvimento.

O mesmo autor ainda apresenta um gráfico demonstrativo das etapas do processo de prototipagem:

|￼Imagem 1: Prototipação. Fonte: Pressman (2010)|
|----------------------------------------------|
|![prototipacao](http://s3.amazonaws.com/magoo/ABAAABiVMAA-99.png)|



Sustentando a adoção deste método, em artigo publicado, Sato (2010) destaca alguns motivos relevantes para o uso de protótipos ao longo do processo de desenvolvimento de jogos: 

- Permitem uma maior interação do game design e das ideias da equipe ampliando o alcance da comunicação entre os membros da equipe; 
- Permitem maior visualização e estudos de possibilidades para o jogo;
- Permitem testar ideias, conceitos e suas viabilidades; 
- Possibilitam o estudo de todas as ações pretendidas no jogo; 
- Permitem estudos dos limites físicos/espaciais do jogo; 
- Permitem verificar os pontos de interação e as formas de interação do jogador com o jogo e/ou outros jogadores; - Permitem estudos no balanceamento do sistema do jogo;
- Permitem estudos da progressão do jogo; 
- Possibilitam observar e definir as possíveis escolhas do jogador para cada ponto de interação e ações a serem realizadas; 
- Possibilitam estabelecer e verificar os feedbacks para o jogador, conforme este realiza uma ação dentro do jogo; 
- Oferecem redução de tempo e custo; 
- Permitem balanceamento entre a visão criativa e as condições técnicas e tecnológicas. 

A utilização da Game Engine (Motor de Jogo) RPG Maker MV facilitará o processo de prototipação e os testes do jogo, permitindo um deploy ágil de um protótipo experimental jogável.

## Objetivos:
	- Deste Documento:
		+ Tabelar as etapas do desenvolvimento do software;
		+ Mapear as atividades realizadas durante o processo;
		+ Descrever as funcionalidades do produto;
		+ Firmar Registro do desenvolvimento;
		+ Orientar o desenvolvimento;
	- Do sistema:
		+ Dar vida ao conto milenar em questão;
		+ Fornecer entretenimento através de mídia digital;
		+ Produzir mídia intelectual-cultural de qualidade;
	- A quem se destina este documento:
		+ Dono do produto a ser desenvolvido;
		+ Desenvolvedores do produto;
		+ Usuários em busca de conhecimento técnico sobre o produto;
		+ Demais stakeholders envolvidos no projeto;



## Requisitos de Sistema:
- O jogo deve ser  no formato RPG 2D, ao estilo Final Fantasy, Legend of Mana, Chrono trigger, etc;
- O sistema de batalhas é Lateral turn based;
- O enredo deve ser incrementado dando final alternativo ao jogo;
- O jogo deve ser disponibilizado para as plataformas Windows, Linux, MacOSX, IOS e Android;

## História

### EPOPEIA DE GILGAMESH

###### Original:
###### Translated by Maureen Gallery Kovacs Electronic Edition by Wolf Carnahan, I998

<h6 align="right">Tradução e adaptação:
Bruno L. Carli, 2017</h6>



	 CAPITULO I

	Aquele que já viu tudo, eu o anunciarei às terras. Eu ensinarei sobre aquele que experimentou todas as coisas,
	Anu concedeu-lhe a totalidade do conhecimento de todos. Ele viu o Segredo, descobriu o Oculto. Ele trouxe
	informações do tempo antes da grande enchente. Ele foi em uma viagem distante, empurrando-se até a exaustão, mas
	depois foi trazido à paz. Ele esculpiu em uma parede de pedra todos os seus trabalhos. E construiu as muralhas de
	Uruk, a parede do templos sagrados e santuários sagrados.Tal como nenhum rei ou homem posterior jamais igualou,
	Gilgamesh passou por todas as dificuldades.

	Supremo sobre outros reis, senhor na aparência, ele é o herói, nascido de Uruk, o bravo touro selvagem. Ele sai na 
	frente, o líder, e na retaguarda é confiado por seus companheiros. Foi ele que abriu as passagens da montanha, que 
	cavou poços no flanco da montanha.  Foi ele quem cruzou o oceano, os mares vastos, para o sol nascente, que 
	explorou as regiões do mundo, buscando a vida.

	Dois terços dele são deus, um terço dele é homem. A Grande Deusa Aruru projetou o modelo para seu corpo, ela 
	preparou sua forma o mai bonito dos homens, Perfeito. Ele vive na cidade de Uruk, É poderoso como um touro selvagem 
	e anda cabeça erguida. Não há rival que possa levantar uma arma contra ele. Gilgamesh é o rei de Uruk, Corajoso, 
	eminente, belo e sábio!

	Porém o povo de Uruk murmuravam aos deuses: "Vocês realmente trouxeram-no para ser um poderoso touro selvagem!”, 
	“Não há nenhum rival que possa levantar uma arma contra ele.”, “Seus companheiros estão atentos aos seus comandos”, 
	"Gilgamesh não deixa um filho para sua mãe, pois desafia a todos, inclusive os jovens”,”Ele é o rei de Uruk e 
	deveria ser seu pastor, não este arrogante”, "Em sua luxúria Gilgamesh não deixa uma moça para sua mãe! Nem a filha 
	do guerreiro, nem a noiva do jovem, primeiro o rei, depois o marido”


	Anu ouviu suas queixas, e os deuses clamaram a Aruru: "Foi você, Aruru, que criou a humanidade, agora crie um zikru 
	para ele. Que ele seja igual ao seu coração tempestuoso e deixe-os ser um atraídos de modo que Uruk possa encontrar 
	a paz!”. Quando Aruru ouviu isso, ela criou dentro de si o zikru de Anu. Aruru lavou as mãos, arrancou um pouco de 
	argila e jogou-a na terra. Ela criou o valente Enkidu. 

	Seu corpo inteiro era coberto de pelos, Ele tinha uma cabeça cheia de cabelos longos e cheios, ele não conhecia o 
	povo e vivia com as feras das colinas, um caçador notório veio face-a-face com ele próximo ao riacho que corta o 
	bosque. Um primeiro, um segundo e um terceiro dia. Ele veio cara a cara com ele em frente ao riacho. Ao vê-lo, o 
	rosto do caçador ficou duro de medo, e Enkidu e seus animais recuaram para casa. O coração do caçador bateu e seu 
	rosto estava falido.Voltou rapidamente para sua casa.

	O caçador dirigiu-se a seu pai dizendo:  "Pai, há um homem-fera vivendo nas montanhas. Ele parece ser o mais 
	poderoso da terra, sua força é tão poderosa quanto o meteorito De Anu! Ele vai continuamente sobre as colinas, ele 
	desce ao riacho para beber água com os animais, Eu estava com medo, então eu não fui até ele. Ele encheu com terra 
	os poços que eu tinha cavado, arrancou minhas armadilhas que havia espalhado, liberando do meu alcance os animais 
	selvagens. Ele não me deixa fazer minhas rondas no bosque! "

	O pai do caçador falou com ele dizendo: “Meu filho, vive em Uruk um certo Gilgamesh. Não há ninguém mais forte do 
	que ele, Ele é tão forte quanto o meteorito de Anu. Vá para Uruk, diga a Gilgamesh sobre este Homem-fera. Ele te 
	dará a prostituta, leva-a contigo. A mulher vencerá o selvagem como se fosse forte. Quando os animais estão bebendo 
	no riacho manda-a tirar o roupa e expor o corpo dela. Quando ele a vir, ele se aproximará, e os seus amigos 
	animais, que cresceram em sua companhia, lhe serão estranhos.”

	Ele deu ouvidos ao conselho de seu pai. O caçador foi para Uruk, ele fez a viagem, ficou dentro de Uruk, no palácio 
	declarou a Gilgamesh: "Há um certo selvagem que veio das montanhas. Ele parece ser o mais poderoso da terra, sua 
	força é tão poderosa quanto o meteorito de Anu! Ele vai continuamente ás colinas, ele desce ao rio beber água com 
	os animais, eu estava com medo, então eu não fui até ele. Ele encheu com terra os poços que eu tinha cavado, 
	Arrancou minhas armadilhas que havia espalhado, liberando do meu alcance os animais selvagens. Ele não me deixa 
	fazer minhas rondas no bosque! "

	Gilgamesh disse ao caçador: "Vá, caçador, e leva esta rameira com você. Quando os animais descerem ao riacho manda-
	a se entregar ao selvagem. Quando ele a vir, ele se aproximará dela, e os seus amigos animais, que cresceram em sua 
	companhia, lhe serão estranhos.”

	O caçador foi, levando a prostituta com ele. Eles partiram na viagem, fazendo o caminho direto. No terceiro dia 
	chegaram ao lugar designado, e o caçador e a prostituta sentaram-se em seus postos. Os animais chegaram e bebiam 
	água no riacho, as bestas selvagens chegaram e mataram a sede com água. Então ele, Enkidu, descendente das 
	montanhas, que come gramas com as gazelas, veio para beber no riacho com os animais, com os animais selvagens ele 
	abafou sua sede com água. Então a rameira o viu, um homem selvagem das profundezas da selva!

	O caçador diz: “Esse é ele! Agora vá até ele, exponha o seu corpo para que ele possa tomá-la em sua voluptuosidade. 
	Não se contenha, tome toda sua energia! Quando ele o vir, ele se aproximará de você. Espalhe seu manto para que ele 
	possa por os olhos sobre ti, E ensina este selvagem a ser como os homens, seus animais, que cresceram com ele, se 
	tornarão estranhos a ele, e sua luxúria gemerá sobre ti ".

	Ela desabotoou seu peito, expôs seus seios, e ele tomou-a em sua voluptuosidade. Por seis dias e sete noites Enkidu 
	ficou excitado, E teve relações sexuais com a prostituta até que ele estava saciado com seus encantos. Mas quando 
	ele voltou sua atenção para seus animais, as gazelas viram Enkidu e saíram, os animais selvagens distanciaram-se de 
	seu corpo. Enkidu viu seu corpo completamente esgotado, seus joelhos que queriam sair com seus animais ficaram 
	rígidos. Enkidu estava acabado, ja não corria como antes. Mas então ele se ergueu, pois seu entendimento se 
	ampliou. E seguiu prostituta em direção ás luzes que vinham da cabana nas colinas.

	A prostituta disse a Enkidu: “Agora você é como os homens Enkidu por que quer correr no mato com os animais 
	selvagens? Venha, deixe-me trazê-lo para Uruk, para o Templo Sagrado, a residência de Anu e Ishtar, o lugar de 
	Gilgamesh, que é sábio à perfeição, mas que domina seu poder sobre o povo como um touro selvagem.
	Tornando-se consciente de si mesmo, ele procurou um amigo. Enkidu falou à prostituta: "me leve para o Templo 
	Sagrado, a residência de Anu e Ishtar, e para Uruk, o lugar de Gilgamesh, que é sábio à perfeição, mas que domina 
	seu poder sobre o povo como um touro selvagem. Vou desafiá-lo. Deixe-me gritar em Uruk: Eu sou o poderoso!:

	A rameira fala para Enkidu: "Vou levá-lo a Gilgamesh, eu sei onde ele estará. Ele é mais poderoso do que você, não 
	o subestime. Gilgamesh ja sabe sobre você, ele sonhou com sua chegada“

	Gilgamesh levantou-se e revelou o sonho, dizendo a sua mãe: “Mãe, tive um sonho ontem à noite. Estrelas do céu 
	apareceram, e algum tipo de meteorito de Anu caiu ao meu lado. Eu tentei levantá-lo, mas era muito poderoso para 
	mim, Eu tentei transformá-lo, mas eu não podia movê-lo.  A Terra de Uruk estava de pé à sua volta, toda a terra se 
	tinha reunido em torno dele, os homens aglomeraram-se sobre ele, adorei-o e abracei-o como esposa. Eu o coloquei 
	aos seus pés"

	A mãe de Gilgamesh, a sábia, disse a Gilgamesh: "Quanto às estrelas do céu que apareceram e o meteorito de Anu que 
	caiu ao seu lado, você tentou levantar, mas foi muito poderoso para você, você tentou transformá-lo, mas foram 
	incapazes de movê-lo, você colocou-a aos meus pés, e você a amou e abraçou como uma esposa. Chegará a você um homem 
	poderoso, um camarada que será seu amigo, ele é o mais poderoso da terra, ele é o mais forte, sua força é poderosa 
	como o meteorito de Anu! Você o amará e abraçará como uma esposa. E é ele quem repetidamente salvará você. Seu 
	sonho é bom e propício! "

	Uma segunda vez Gilgamesh disse para sua mãe: "Mãe, eu tive outro sonho: "No portão da minha câmara matrimonial 
	havia um machado. Toda a terra tinha se reunido sobre ele, e eu coloquei a seus pés, eu amei e abracei como uma 
	esposa”. A mãe de Gilgamesh, disse a Gilgamesh: "O machado que você viu é um homem. Aquele a quem você amará e 
	abraçará como uma esposa”. Gilgamesh falou com sua mãe dizendo: "Posso ter um amigo e conselheiro, um amigo e 
	conselheiro que eu possa ter! "Você interpretou para mim os sonhos sobre ele!"

	Enkidu perseguiu leões para que os pastores pudessem comer. Ele derrotou os lobos e perseguiu os leões. Com Enkidu 
	como guarda, os pastores podiam se deitar. Um homem desperto, um jovem singular, era duas vezes mais alto que 
	homens normais.
	E Enkidu andou pela rua de Uruk, poderoso. Ele bloqueou o caminho através do mercado de Uruk. A terra de Uruk 
	estava ao seu redor. Toda a cidadela se reuniu a seu redor, o povo estava se aglomerando, os homens estavam 
	agrupados em torno dele. E comentavam “E é enviado de Anu”, “Ele é como Gilgamesh”, “Ele é mais baixo”, “Agora 
	Gilgamesh tem com quem combater”.

	De noite quando Gilgamesh ia para um noivado usurpar a noiva, Enkidu bloqueou a entrada para a câmara da noiva, E 
	não permitiria que Gilgamesh fosse trazido dentro. Eles lutaram um com o outro na entrada para a câmara da noiva. 
	Na rua se atacaram em praça pública da terra. Os batentes da porta tremiam e as paredes tremiam. Gilgamesh deixou 
	seus oponentes no chão, sua raiva diminuiu e ele virou o peito dele. Enkidu disse para Gilgamesh: “Você é mesmo 
	muito poderoso, o mais poderoso do mundo Gilgamesh. E Gilgamesh disse: “Venha meu amigo, esse é o começo de uma 
	grande amizade”

	CAPITULO II

	Gilgamesh conta a seus amigos que decide descer à floresta dos cedros para caçar Humbaba, o Terrível! Enkidu diz: 
	“Ja estive nessa floresta. A fim proteger a floresta do cedro Enlil atribuíu Humbaba como um terror para os seres 
	humanos, o rugido de Humbaba é uma tormenta, sua boca é Fogo, e sua respiração é Morte! Ele pode ouvir a 100 léguas 
	de distância qualquer sussurro em sua floresta! Quem iria descer à sua floresta!

	Gilgamesh falou com Enkidu dizendo: "O que você diz? Agora você tem medo da morte? O que se tornou de sua força 
	ousada? Eu vou na frente de você, então eu gritarei de dentro do calabouço: “Venha é seguro! Se eu cair, eu 
	estabelecerei minha fama. Outros homens dirão: 'Foi Gilgamesh que travou em batalha com Humbaba, o Terrível!’”

	Foram então ao templo de Shamash pedir sua benção e quando retornou a cidade, disse ao povo: “Vocês, homens de 
	Uruk, sabem que eu quero me tornar mais poderoso, e irei em uma viagem distante! Eu lutarei como eu nunca soube, eu 
	partirei em uma estrada que eu nunca viajei! Dê-me suas bênçãos!”

	Os homens de Uruk disseram: “não deve ir para a Floresta de Cedro, a viagem não é para ser feita!”, “Você esta 
	maluco Gilgamesh, o guardião da floresta do cedro irá tirar sua vida”, ”Você é jovem, Gilgamesh, você não sabe o 
	que você está falando!”, “O rugido de Humbaba é uma inundação, seu hálito chamusca, sua respiração é o som da 
	própria Morte! Ele pode ouvir qualquer sussurro em sua floresta em100 léguas de distância!

	Gilgamesh ouviu a declaração de seus nobres conselheiros. Gilgamesh falou com Enkidu, dizendo: "Vamos, meu amigo, 
	vamos ao Templo de Egalmah, la vive Ninsun e ela nos dará sua benção”, tomando um ao outro pela mão, Gilgamesh e 
	Enkidu caminharam até o Egalmah onde fica o Grande Palácio.

	Para Ninsun, a Grande Rainha. Gilgamesh se levantou, foi até ela e disse: "Ninsun, minha mãe, eu sou 
	extraordinariamente forte, Eu devo agora viajar um longo caminho para onde Humbaba vive, eu devo enfrentar lutas 
	como nunca enfrentei,  e devo viajar em uma estrada que nunca viajei! Até chegar à Floresta de Cedro, até que mate 
	Humbaba, o Terrível, e erradicar da terra algo abominável que Shamash odeia, se eu matar Humbaba e cortar seu cedro 
	que haja regozijo em toda a terra, e eu erigirei um monumento em homenagem aos deuses! "

	As  palavras de Gilgamesh, tocaram a rainha Ninsun. Ela entrou em seus aposentos. Lavou-se com a planta da pureza, 
	ela vestiu um manto digno de seu corpo, ela vestiu jóias dignas de seu peito, ela vestiu sua faixa, e colocou em 
	sua coroa. Ela borrifou água de uma tigela no chão. Ela subiu ao telhado e colocou incenso na frente de Shamash, e 
	ela ofereceu incensos, e levantou seus braços para Shamash e disse: "Por que você impôs um coração inquieto sobre 
	meu filho, Gilgamesh! Agora você o tocou para que ele quisesse viajar um longo caminho para onde Humbaba vive! Ele 
	vai enfrentar lutas como nunca lutou, e vai viajar em uma estradas desconhecidas! Até chegar à Floresta de Cedro, 
	até matar Humbaba, o Terrível, e erradicar da terra algo abominável que você odeia, guia seu caminho para que 
	retorne em segurança.”

	Ela voltou e disse para Enkidu: "Poderoso Enkidu, tu não és do meu ventre, mas agora eu falo com você junto com os 
	devotos sagrados de Gilgamesh, as sacerdotisas, as mulheres santas, e os servidores do templo ". Ela colocou um 
	pingente no pescoço de Enkidu, “este pingente” - Disse Ninsun -  “abençoado pelas sacerdotisas do templo, Irá 
	proteger-te contra os inimigos em sua jornada, e eu lhe imploro Enkidu, proteja Gilgamesh, traga-o de volta em 
	segurança. Nós confiamos o rei de Uruk a sua proteção.”
	A vinte léguas pararam para uma refeição e descanso, Haviam andado cinquenta léguas em um dia inteiro, uma 
	caminhada de um mês e meio. No terceiro dia aproximaram-se dos cedros.

	Gilgamesh subiu no pico da montanha, Acendeu um incenso  e disse: "Montanha, traz-me um sonho, uma mensagem 
	favorável de Shamash.”, Enkidu preparou um lugar de dormir para ele durante a noite, um vento violento passou por 
	isso ele anexou uma cobertura. Eles se deitaram próximo ao circulo de fogo. Enquanto Gilgamesh descansava o queixo 
	sobre os joelhos, o sono que derrama sobre a humanidade o alcançou. No meio da noite seu sono chegou ao fim. Assim 
	que levantou-se, disse a seus amigos: "Meus amigos, vocês não me chamaram? Por que eu acordei? Você não me tocou? 
	Por que estou tão perturbado? Um deus passou? Por que meus músculos estão tremendo? Enkidu, meu amigo, eu tive um 
	sonho e o sonho que eu tinha era profundamente perturbador. Nos desfiladeiros da montanha, a montanha caiu sobre 
	nós e fomos esmagados como moscas.”

	Enkidu, interpretou o sonho de seu amigo: "Meu amigo, seu sonho é favorável. O sonho é extremamente importante. Meu 
	amigo, a montanha que você viu no sonho é Humbaba. Significa que vamos capturar Humbaba, e matá-lo e lançar seu 
	cadáver ao chão. Pela manhã haverá uma mensagem favorável de Shamash.”

	Na entrada da floresta dos cedros ressoou um som de advertência do céu. “Humbaba está floresta adentro, escondido 
	em seu covil, no templo perante as árvores” disse Gilgamesh e Enkidu falou com Gilgamesh, dizendo: "Assim que 
	descermos para a Floresta de Cedro, vamos abrir caminho entre as árvores, haverão inimigos mas nós passaremos por 
	eles, até que cheguemos às Ruínas da Floresta de Cedro. " e continuou “ Atravessamos montanhas e terras distantes 
	para chegar até aqui, ganhamos experiência na batalha e agora, deixem que o medo parta, não temam a morte, vamos 
	meus amigos, o Terrível Humbaba nos aguarda.”

	Eles estão na beira da floresta, olhando para o topo da árvore de cedro, olhando para uma entrada da floresta. Esta 
	entrada levava para as Ruínas. Sabiam que estavam no caminho certo pois onde Humbaba caminhava, tinha uma trilha, 
	em seu caminho começaram a aparecer restos de ossos e corpos em decomposição.
	Quando encontraram Humbaba, ele falou a Gilgamesh dizendo: "Eu sabia que você viria Gilgamesh, Enlil me avisou de 
	sua vinda, és tolo Gilgamesh, você se acha um Deus mas esqueces que sua única herança dos Homens é a mortalidade, 
	um Deus não pode morrer, mas eu matarei você semideus”

	Enkidu falou com Humbaba, dizendo: "Humbaba  um sozinho não é capaz de vence-lo, mas nós não estamos sozinhos.” E 
	Humbaba fala a Enkidu: “Enkidu você que corria com os bichos do mato, eu podia ter comido sua carne quando te via a 
	solta pela selva seu cretino, agora pensas que é como os homens, eu vou te matar miserável!!!”, Humbaba falou a 
	Gilgamesh, dizendo: “Um idiota é um idiota e devem dar conselhos uns aos outros, você, Gilgamesh, veio a mim e 
	agora vou moer os seus ossos e joga-los aos abutres!”

	Depois da batalha, Humbaba implorou por sua vida, a espada de Gilgamesh estava por sobre o pescoço de Humbaba e 
	poderia corta-la fora a qualquer instante, “Humbaba implorou por sua vida, dizendo a Gilgamesh: "Você ainda é 
	jovem, Gilgamesh, sua mãe deu à luz a você, você foi persuadido pela palavra de Shamash,  foi ele quem despertou o 
	desejo por esta expedição em ti. Gilgamesh, deixe-me ir, vou morar com você como seu servo, eu cortarei para você 
	todas as árvores que quiser, haverá tanta madeira fina o suficiente para o seu palácio! " Enkidu se dirigiu a 
	Gilgamesh, dizendo: "Meu amigo, não ouça Humbaba, ele quer persuadi-lo eternamente o trairá.”, aparentemente 
	Humbaba vê que Gilgamesh é influenciado por Enkidu, e se move para dissuadir Enkidu. "Você entende as regras da 
	minha floresta. Além disso, você está ciente de todas as coisas assim ordenadas por Enlil. Eu deveria ter te matado 
	quando tive a chance animal Na própria entrada dos ramos da minha floresta. Eu deveria ter alimentado sua carne com 
	o urubu, a águia, e o abutre. Então agora, Enkidu, a clemência depende de você. Fale com Gilgamesh para poupar 
	minha vida! "

	Enkidu se dirigiu a Gilgamesh, dizendo: “Meu amigo, Humbaba, Guardião da Floresta de Cedro, foi enviado por Enlil 
	da Montanha, foi enviado para destruir os homens, nós devemos mato-lo.” Humbaba, Guardião da Floresta, disse: “Os 
	deuses se encherão de raiva contra vocês.”, Enkidu fala a Gilgamesh: “Não caias na maldição de Humbaba Gilgamesh, 
	vamos” então Gilgamesh corta a cabeça de Humbaba.

	O silêncio caiu sobre a montanha, e sobre o céu. Eles atravessam o cedro, Enkidu disse para Gilgamesh ao fim da 
	floresta: “Gilgamesh, nós vencemos o mal da floresta, agora deves erigir um monumento aos deuses. Também, Enlil da 
	Montanha deve estar muito furioso, vamos ter cautela para nano ferir o orgulho dos deuses.” Enquanto Gilgamesh 
	segurava a cabeça de Humbaba eles voltaram a Uruk.

	CAPITULO III

	Gilgamesh lavou seus cabelos arranhados e limpou seu equipamento, sacudindo sua capa por sobre suas costas, jogando 
	fora suas roupas sujas e vestindo roupas limpas. Calçou novas botas e apertou seu cinto. Quando Gilgamesh colocou 
	sua coroa em sua cabeça, Ishtar, a deusa do amor e da beleza ergueu os olhos para a beleza de Gilgamesh, dizendo: 
	"Venha, Gilgamesh, seja você meu marido, para conceder-te teus herdeiros. Seja você meu marido, e eu serei sua 
	esposa. Eu vou dar a ti uma carruagem de lápis-lazúli e ouro, Entre em nossa casa, com a fragrância de cedro. E 
	quando você entrar em nossa casa, o batente da porta e o estrado do trono 'Beijarão seus pés’. O povo Lullubu vai 
	lhe trazer o produto das montanhas e do campo como tributo. E também, outros senhores e reis de outras terras se 
	curvarão a ti, Gilgamesh.”

	Gilgamesh dirigiu-se à princesa Ishtar dizendo: "O que eu teria que lhe dar se eu me casasse com você? Você precisa 
	de óleo ou roupas para o seu corpo! Você não tem nada para comer ou beber? Gostaria de bom grado alimentá-la com 
	comida adequada para um deus, gostaria de lhe dar vinho apto para um rei, qualquer homem em sua luxuria faria tudo 
	para casar-se contigo!” - respirou e prosseguiu - “Contudo onde estão seus noivos que você guarda e ama para 
	sempre? Posso ser jovem, mas compreendo que nem tudo que reluz é ouro. Veja aqui agora, vou recitar a lista de seus 
	amantes lady Ishtar. Tammuz, o amante de sua juventude mais antiga, para ele você ordenou lamentações ano após ano! 
	Você amou o pássaro colorido do jovem pastor e bateu nele, quebrando sua asa, então agora ele está na floresta 
	vivendo sem poder voar! Você amou o leão supremamente poderoso, mas você cavou para ele sete palmos abaixo da 
	terra. Você amou o garanhão, famoso na batalha, contudo ordenaste para ele o chicote, ordenou para ele galopar por 
	setenta e sete horas e então ordenado para ele beber de águas confusas. Você amava o pastor dos pastores, Mestre 
	Herder, que carinhosamente vos apresentava pão cozido em brasas, e que diariamente lhe trouxe a caça para o jantar. 
	Contudo, você o atingiu e transformou-o num lobo, Então seus próprios pastores agora o perseguem com seus próprios 
	cães. Você também amava Ishullanu, jardineiro da casa de seu pai, Que continuamente trouxe-lhe cestas de 
	guloseimas, e iluminado sua mesa diariamente. Você o transformou em um anão, e o fez viver no meio de seu jardim. E 
	agora eu! Sou eu que você ama, e você vai ordenar para mim como ordenou o fim para eles!"

	Quando Ishtar ouviu isto, em uma fúria ela subiu ao céu, Indo para Anu, seu pai, e chorando, Indo para Anu, seu 
	pai, e chorando: "Pai, Gilgamesh me insultou repetidamente, Gilgamesh relatou atos desprezíveis sobre mim, 
	Desprezíveis atos e maldições! " Anu dirigiu-se à princesa Ishtar, dizendo: "Qual é o problema? Não foi você que 
	provocou o rei Gilgamesh? Então Gilgamesh relatou ações desprezíveis sobre você, Desprezíveis atos e maldições?" 
	Ishtar falou com seu pai, Anu, dizendo: "Pai, dá-me o Touro do Céu, para que ele possa matar Gilgamesh em sua 
	habitação. Se você não me der o Touro do Céu, Eu derrubarei as Portas do Netherworld, vou esmagar os postes da 
	porta, e deixar as portas para baixo, e vai deixar os mortos subir para comer os vivos! E os mortos superarão os 
	vivos!

	Anu dirigiu-se à princesa Ishtar, dizendo: "Se você exigir o Coice do Céu de mim, Haverá sete anos de trevas para a 
	terra de Uruk. Você já colecionou grãos para o povo? Você fez grama crescer para os animais? " e Ishtar dirigiu-se 
	a Anu, seu pai, dizendo: "Eu tenho amontoado grãos nos celeiros para o povo, Eu fiz gramas crescer para os animais, 
	Suficiente para poderem comer nos sete anos de trevas.”. Quando Anu ouviu suas palavras, colocou a nariz do Touro 
	do Céu na mão de Ishtar e ela levou o Touro do Céu até a terra. Quando chegou a Uruk Ele subiu para o Eufrates e ao 
	resmungo do Touro do Céu abriu-se um enorme poço, muitos cidadãos daquelas terras cairam, Enkidu que estava por 
	perto quase caiu, se não tivesse se agarrado a uma raiz e saltado para fora da fenda que engolia a terra. Ao 
	salvar-se Enkidu viu o grande Touro que vomitava raiva perante Enkidu, que voltou correndo a Uruk para contar a 
	Gilgamesh.

	Enkidu se dirigiu a Gilgamesh, dizendo: "Meu amigo, o Touro de Céu abriu uma fenda que engoliu parte do vale, 
	muitos morreram, devemos ser ousados” e Gilgamesh diz: “Vou arrancar os chifres deste maldito” 
	Depois de terem matado o Touro do Céu, arrancaram seu coração e apresentaram-no a Shamash.  Então os deuses se 
	sentaram juntos para uma reunião. Ishtar subiu para o topo do Muro de Uruk, lançou-se na pose de luto, e lançou sua 
	maldição lamentável: “Maldito Gilgamesh que me difamou e matou o Coice do Céu, vai pagar por isso!”

	Gilgamesh também trouxe os chifres do touro, que brilhavam os olhos dos artesãos que ofereciam até 30 lapislazuli 
	pelos chifres. Eles lavaram as mãos no Eufrates, e procedeu de mãos dadas, caminhando pelas ruas de Uruk. Gilgamesh 
	disse aos guardas do palácio: "Quem é o mais corajoso dos homens? Quem é o mais ousado dos guerreiros? Gilgamesh é 
	o mais bravo dos homens, o mais ousado dos guerreiros! Aquele que enviou o touro para trazer desgraça em nossa 
	terra esta furiosa, Ishtar não tem ninguém que lhe veja com bons olhos na rua agora. Vamos festejar” Gilgamesh 
	realizou uma celebração em seu palácio. Os Rapazes cochilaram, dormindo nos sofás da noite. Enkidu estava dormindo, 
	e teve um sonho. Acordou e revelou seu sonho a seu amigo.

	"Meu amigo, por que os Grandes Deuses estão em conferência? Em meu sonho Anu, Enlil e Shamash realizaram um 
	conselho, e Anu falou a Enlil: "Porque eles mataram o Touro do Céu e também mataram Humbaba?, O rei deles que 
	profanou o cedro da montanha na selva deve morrer!” Enlil disse: "Que Enkidu morra, mas Gilgamesh não deve morrer!" 
	Shamash, Deus do Céu respondeu a valente Enlil: "Não foi a meu comando que eles mataram o Touro do Céu e Humbaba! 
	Deveria agora o inocente Enkidu morrer? Então Enlil ficou zangado com Shamash, dizendo: “É você quem é responsável 
	porque você viajou diariamente com eles como seu amigo! "

	Enkidu estava deitado na frente de Gilgamesh. Suas lágrimas fluindo como canais, e disse: "Ó irmão, querido irmão, 
	por que eles estão absolvendo-me em vez de meu irmão?” e Enkidu disse : "Então agora eu devo me tornar um fantasma, 
	para sentar com os fantasmas dos mortos, para nunca mais ver meu querido irmão! Na Floresta de Cedro, onde o 
	emboscamos Humbaba, eu não matei o Cedro." E Gilgamesh disse para seu companheiro: "Amigo, os deuses lhe deram uma 
	mente ampla e embora seja bom para você ser sensato, você continua pronunciando coisas impróprias! Por que, meu 
	amigo, sua mente expressa coisas impróprias? O sonho é importante, mas muito assustador, seus lábios estão zumbindo 
	como moscas. Embora haja muito medo, o sonho é muito importante. Para os vivos, os deuses deixam tristeza, vou 
	rezar e suplicar os Grandes Deuses, o que Enlil diz não pode ser verdade, e se for nos tornaremos inimigos dos 
	deuses para proteger-te de qualquer desgraça.” 

	As entranhas de Enkidu estavam agitando-se, deitado lá tão sozinho. Falou tudo o que sentia, dizendo ao amigo: 
	“Ouça, meu amigo, o sonho que tive ontem à noite. Os céus clamaram e a terra respondeu e eu estava de pé entre 
	eles. Apareceu um homem de rosto negro, seu rosto parecia o Anzu. Suas mãos eram as patas de um leão, suas unhas as 
	garras de uma águia! Ele me pegou pelo cabelo e me dominou. Golpeei-o com um golpe, mas ele saltou como uma corda, 
	e então ele me golpeou e paralisou-me como uma cobra, e pisoteou-me como um touro selvagem. ‘Ajude-me, meu amigo’ 
	eu gritava, mas você não me resgatou, você estava com medo e não pode fazer nada". "Então ele me transformou em uma 
	pomba, de modo que meus braços estavam emplumados como um pássaro. Segurando-me, ele me levou até a Casa das 
	Trevas, a habitação de Irkalla, para a casa onde os que entram não saem, ao longo da estrada de não retorno, para a 
	casa onde os que habitam sem luz clamam em desespero, onde a sujidade é a sua bebida, a sua comida é de barro, onde 
	como um pássaro, eles usam roupas de penas, e a luz não pode ser vista, eles habitam no escuro. Ao entrar na Casa 
	da Poeira, em toda parte eu olhei havia coroas reais reunidas em montões, em todo lugar que eu ouvia, era os 
	portadores de coroas, que, no passado, tinha governado a terra, mas que agora servem a Anu e Enlil carnes cozidas. 
	Ali estava o sumo sacerdote e acólito, ali estava o padre da purificação e extasiado, ali estavam os sacerdotes 
	ungidos dos Grandes Deuses. Ali estava Etana, lá estava Sumukan, lá se sentou Ereshkigal, a rainha do Netherworld. 
	Beletseri, o escriba do Netherworld, ela estava segurava um papiro e estava lendo para o Ereshkigal, a rainha do 
	Netherworld”

	E por sete noites Enkidu dormiu e sonhou com o momento de sua morte, gemia em sua cama e sua frio. Em seus últimos 
	suspiros, Enkidu disse para Gilgamesh: “A. Deusa me amaldiçoou amigo, estou fadado a partir para o submundo, 
	gostaria de ter caído em batalha com herói a teu lado, mas morrerei vergonhosamente em uma cama, nas sombras.” 
	Gilgamesh ao sentir que o coração de Enkidu ja não batia mais ele caiu em prantos, fechou os olhos do amigo e o 
	recobriu com um véu.

	CAPITULO IV

	Quatro anos haviam se passado, Gilgamesh nunca mais vira Alfr, o caçador nem Skulda a feiticeira, cujos lhe haviam 
	ajudado em suas tarefas na floresta do cedro e na luta contra o touro do céu. Gilgamesh havia abandonado Uruk para 
	realizar uma peregrinação em busca dos segredos da vida. Se pegou andando pelas ruas da Babilônia cuja possuía uma 
	torre incrivelmente alta, alcançava os céus e la em cima imaginava enxergar palácios nas nuvens, perguntava-se 
	constantemente se poderia estar delirando. Quanto recobrou sua consciência continuou seu caminho para a grande 
	Biblioteca, onde procurou por pergaminhos antigos.

	Descobriu que poderia entrar no Netherworld se obtivesse um artefato chamado Talismã da Fenda, que permite um ser 
	mortal atravessar a fenda que conecta os planos da existência. Porém os deuses haviam fragmentado em três partes 
	este talismã, escondendo suas partes em diferentes regiões, e que seriam guardadas por terríveis bestas.

	Gilgamesh sabia de lendas antigas que contavam sobre uma fera mais terrível do que o Humbaba que havia cortado a 
	cabeça, uma fera que vivia para guardar seu segredo. Gilgamesh supunha agora que o segredo da fera poderia ser uma 
	das partes do talismã que procura. A fera vivia nas profundezas do calabouço de Gormet, um antigo templo tombado em 
	ruínas, selado pelos deuses e proibido pelos homens. Agora Gilgamesh pretendia profanar os selos mágicos das portas 
	do templo em busca de seu tesouro.

	Para quebrar o encantamento que sela a entrada do calabouço, Gilgamesh precisou ir até Egalmah falar sua mãe e 
	pedir que lhe ensinasse como desfazer o encantamento. “Mãe, ensina-me como desfazer encantamentos, assim poderei 
	desfazer a magica que sela as portas mágicas que existem neste mundo.”, e a deusa respondeu: “Meu filho, por que 
	queres abrir as portas mágicas que existem nesse mundo? Se o fizeres coisas terríveis que   os deuses e os homens 
	de outrora ali aprisionaram, sairão da escuridão para a luz da superfície, trazendo a desgraça para o homem 
	novamente.” e Gilgamesh disse: “Eu Gilgamesh, me responsabilizo por isso, que os deuses me julguem me acusem se eu 
	falhar. Não deixarei uma coisa viva para escapar de qualquer túmulo trancado que faça mal à este mundo.” Sua mãe 
	então lhe disse: “Que seja, Gilgamesh. Eu lhe ensinarei como desfazer a mágica. Mas saiba, Gilgamesh, que os deuses 
	tem falado de ti, tem observado você. Enlil das montanhas tem tentado corromper os outros deuses. Tome cuidado, meu 
	filho!”. E adeusa ensinou Gilgamesh a decantar.

	Gilgamesh partiu em direção ao calabouço, muitos dias de caminhada, subiu pelas colinas, e desceu novamente 
	atravessando um lugar deserto e sombrio entre as paredes de pedra. Quando chegou na porta selada, usou o 
	decantamento ensinado por sua mãe, quebrando o selo mágico. Ao romper o selo um enorme demônio surge em seu caminho 
	gritando: “Uhaaaaa... GILGAMEEEESHHHHH EU VOU ARRANCAR A SUA CABEÇA!” O demônio atacou furiosamente Gilgamesh. 
	Durante a batalha, uma explosão de chamas atinge o monstro. Gilgamesh viu que era a feiticeira Skulda que chegava 
	para seu axílio. Os dois mataram o demônio. “Esse era somente o porteiro” - disse Skulda. Esclareceram algumas 
	ideias e entraram no calabouço.

	Era escuro e sujo, e haviam criaturas estranhas la dentro que saiam das sombras, passaram por varias câmaras até 
	chegar a sala da criatura que guardava o tesouro. Eles lutaram ferozmente com o demônio, e quando ele sucumbiu 
	murmurava palavras como: “Enlil da montanha, matar Gilgamesh” entre outros gemidos e rosnados esquisitos.

//TODO continuar historia


## Gameplay - Mecânicas

Gilgamesh: An Epic Tale é um jogo de RPG de mundo semi-aberto não-linear que permite o jogador explorar o cenário a vontade dentro dos limites da história (o que quer dizer que para entrar em determinados mapas será preciso concluir determinada parte da história). Sua mecânica é similar à clássicos da série Final Fantasy, com batalhas laterais e um enredo envolvente. O jogo apresentará cenários originais com diferentes climas, de dia ou de noite, chuva ou sol e certos tipos de inimigo que aparecem somente ema certas condições proporcionando uma diversidade de eventos ampla e abrangente. 
As batalhas serão Side Battles (batalhas laterais)  onde o jogador é levado a uma tela onde seus heróis estão de um lado da tela e o inimigo de outro, o jogador receberá as opções disponíveis para batalha, que são: 

| Ação | Descrição |
|------|-----------|
|Atacar|O personagem ataca com golpe fisico utilizando a arma que está na sua mão;|
|Feitiço/Habilidade|Um menu com a lista de habilidades ou mágicas que o personagem souber será exibido e o jogador poderá escolher, se disponível, a habilidade que quiser e puder utilizar, ou voltar ao menu anterior;|
|Proteger|O personagem tomará posição defensiva recebendo menos dano caso seja atingido;|
|Item  |Um menu com a lista de itens disponíveis será exibido ao jogador para que possa escolher um item para ser usado. O efeito e descrição do item aparecerá ao selecionar o item desejado. O jogador poderá retornar ao menu anterior caso não deseje mais utilizar um item;|
|Fugir |Os personagens tentarão fugir da luta, se obtiverem êxito, o jogador voltará a tela do cenário. Em batalhas contra chefe é impossível a  fuga.|


A batalha acontecerá quando:
	- O jogador tocar em um inimigo no cenário;
	- Um evento no decorrer da história acontecer (geralmente um chefe).


O jogador encontrará diversos desafios na história, como a jornada para terras distantes, busca por artefatos perdidos, explorar calabouços, batalhar com fantásticas criaturas das mais diferentes espécies e tamanhos.
O progresso no jogo acontece por meio da realização dos principais eventos da história que levarão o jogador a desafios mais complicados, calabouços mais profundos e inimigos mais poderosos, exigindo maior fortalecimento dos heróis. O jogador encontrará áreas especiais no jogo, chamadas de área segura, onde os inimigos não podem entrar e o jogador poderá salvar seu progresso. O progresso poderá ser salvo fazendo com que o personagem toque no Cristal Mágico. Certas tarefas devem ser cumpridas para que o progresso no jogo aconteça, e certas tarefas opcionais estarão acessíveis ao jogador para que possa conquistar novos itens e equipamentos.
O jogador irá se deparar com uma gama de possibilidades de recompensas. Poderá encontrar tesouros em lugares inóspitos, recebe itens, dinheiro e experiência após vencer uma batalha, poderá cumprir tarefas e receber algum tipo de recompensa por isso.
O jogo termina quando o jogador completar todos os eventos principais. Os eventos principais estão relacionados ao enredo da história, quando o jogador cumprir todos os desafios da história o jogo se dará por finalizado.
Se todos os heróis do grupo morrerem (Deixar o HP chegar a zero) o jogo acaba e o jogador voltará a tela de inicio, podendo carregar algum de seus jogos salvos na memória.
As habilidades dos personagens terão um custo de energia, que pode ser recuperado através de itens, tocando no cristal ou dormindo em locais de repouso. As feitiçarias além do custo de atp (energia) poderão requerer a utilização de ítens para serem conjuradas.

//TODO inserir e descrever menu

## Personagens 

A imagem dos personagens foi elaborada no criador de imagens do RPG Maker MV, plataforma principal de desenvolvimento deste projeto.

### Personagens Jogáveis:

|Nome|Altura|Local de Nascimento|Ocupação|Classe|Descrição|Sprites|Face|
|----|------|--------------------|--------|------|---------|-------|-----|
|Gilgamesh|1,90|Uruk|Rei de Uruk|Herói|O rei de Uruk e protagonista da epopéia, Filho da Deusa Ninsun com o pastor mortal Lugalbanda, por estes motivos Gilgamesh é dois terços deus e um terço homem. O herói da história passa por várias aventuras  e perigos desafiando os deuses de sua terra. É Bravo, porém sincero. É também o mais belo e poderoso de Uruk.|![Gigamesh Sprites](https://uploaddeimagens.com.br/images/001/350/718/original/Gilgamesh.png?1522301761)|![Gilgamesh Face](https://uploaddeimagens.com.br/images/001/350/720/full/Gilgamesh.png?1522301893)|
|Enkidu|1,90|Floresta do Cedro|Escudeiro de Gilgamesh|Fera|Enkidu foi criado pelos deuses à pedido do povo de Uruk, ele é um zikru (um semelhante) de Gilgamesh, enviado para que pudesse acalmar distrair Gilgamesh. Somente assim o rei aprenderia seu verdadeiro oficio.|-|-|
|Alfr|1,75|Colinas do vale de Uruk|Caçador|Arqueiro|Alfr é um personagem fictício representando o papel do caçador que identifica Enkidu no bosque. Passa então a ajudar Gilgamesh em suas jornadas. Alfr é um pouco covarde mas um exímio atirador de arco e flecha. Leal e sincero, mora com seu velho pai em uma pequena casa nas colinas do vale, próximo ao bosque.|-|-|
|Skulda|1,63|Desconhecido|Serva e Protetora de Gilgamesh|Feiticeira|Uma feiticeira que diz ser designada pelos deuses para empenhar-se em ajudar Gilgamesh à cumprir seu destino. Misteriosa e sarcástica, porém extremamente sábia. Possui feitiços mágicos destruidores capazes de causar um estrago enorme em seus inimigos.|sprite skulda|face skulda|


## Personagens Não Jogáveis da história (NPC):

|Nome|Altura|Local de Nascimento|Ocupação|Classe|Descrição|
|----|------|-------------------|--------|------|---------|
|Pai do Alfr|1,70 metros|Uruk|Fazendeiro|NPC|O velho pai do caçador Alfr, aparece na história para dar conselhos à seu filho. Manda-o para Uruk conhecer Gilgamesh, nunca recusa ceder o espaço de seu lar para que você aventureiro possa descansar.|
|Shamat|1,59|Uruk|Rameira|Item Chave|Shamat é uma prostituta entregue por Gilgamesh para que Alfr leve-a até onde Enkidu se encontra nas colinas para que seduza a fera. Shamat ensina Enkidu os segredos dos homens.|
|Ninsun|Desconhecido|Desconhecido|Deusa|NPC|A mãe de Gilgamesh, sábia Deusa dos homens e guia iluminada do herói da lenda, responsável pelas duas partes deus de Gilgamesh, concedendo-lhe a força de um touro indomável.|
|Ishtar|Desconhecido|Desconhecido|Deusa|NPC|A belíssima Deusa Ishtar, da qual aqueles cujo lançam o olhar caem em um eterno e profundo amor. Senhora da fertilidade, do amor, do sexo e da guerra, deleita-se no prazer dos homens porém seu orgulho é ferido ao ser rejeitada por Gilgamesh, jurando destruir a vida do herói.|
|Anu|Desconhecido|Desconhecido|Deus|NPC|Anu é o senhor dos céus, dos espíritos e das constelações, sábio dentre os deuses, pai de Ninsun e Ishtar, é furioso e capaz de mudar a ordem das coisas com uma simples piscadela sendo o mais forte dentre todos os deuses.|
|Shamash|Desconhecido|Desconhecido|Grande Deus|NPC|Shamash é o Deus dos Deuses perante a Terra, o glorioso Sol que resplandece e enche o universo de luz e força. Shamash é o supremo Deus sumério a qual todos clamam.|
|Enlil|Desconhecido|Desconhecido|Deus|NPC|Enlil o senhor sobre a montanha, tem agido de maneira impetuosa e estranha por motivos desconhecidos, enviando diversas dificuldades no caminho de Gilgamesh e tentando corromper os outros deuses.|
|Ereshkigal|Desconhecido|Desconhecido|Rainha do Netherworld|NPC|Ereshkigal é a rainha do submundo, sentada sob seu trono ela cuida para que a alma dos que morreram permaneçam em paz nos salões do Netherworld.|

### Outros NPC’s:

|Nome|Descrição|
|----|---------|
|Vendedor de Item|Comerciante responsável pela venda de itens consumíveis. Localizado nas lojas das cidades.|
|Comerciante|Comerciante de itens consumíveis que pode aparecer em áreas do jogo como acampamentos, bosques e entradas de calabouços.|
￼|Atendente do INN|Recepcionista localizado nas pousadas do jogo, responsável por acomodar os heróis e cobrar a taxa da pousada.|
|Ferreiro|O ferreiro é o comerciante responsável pela venda de Armas, Equipamentos e Acessórios, localizado nas Lojas de Armas e Equipe nas cidades e vilas.|
|Herbalista|Comerciante de ervas, incensos e óleos utilizados por feiticeiros em seus experimentos mágicos. Localizado no Covenstead das cidades do jogo.|
|Macerador|Responsável por realizar as sínteses de ítens. Localizado nos Covensteads das cidades.|


￼￼

### NPCs com função unicamente de exibir mensagens ao jogador:

//TODO colocar o sprite dos NPCs variados

## Universo do Jogo

Os cenários do jogo devem descrever uma imagem digna de um ambiente mágico com uma história de fantasia. Os mapas utilizarão a técnica de parallax evidenciando os efeitos de sombreamento, luz e overlays.

￼
Imagem 2 - Colinas do Bosque

Os cenários serão conectados através de eventos de transferência, sempre que o jogador chegar ao final da estrada e houver este evento, automaticamente o herói será transferido para a continuação do mapa. Em geral as áreas do jogo estarão dispostas em um grande mapa do mundo em que o jogador poderá ter a liberdade de explorar, podendo este entrar nas florestas, bosques, cidades, vilarejos, calabouços, etc. que estiverem por sobre o mapa. Ao tocar em um destes o evento de transferência será ativado, levando o herói para a localização daquela área.
O mundo será semi-aberto dando liberdade ao jogador para explorar áreas inóspitas do game, desde que possua condições de sobreviver nestas áreas e tenha cumprido determinada parte da história que permita sua passagem nesta área. Por não possuir limites (exceto por poucos bloqueios que somente serão liberados após a conclusão de um determinado evento da história) o jogador poderá, por exemplo, entrar em um calabouço ou região onde os inimigos sejam extremamente fortes, obrigando-o a retornar mais tarde quando ja tiver fortalecido seus heróis.
O ambiente deverá passar uma sensação de nostalgia e fantasia, além de tornar a imersão do jogador na história mais envolvente, fazendo-o sentir como se realmente fosse o herói. Os cenários devem ser belos, originais e únicos.
Cada cenário deve ter musicalidade com efeitos sonoros característicos à sua situação. Músicas temáticas serão utilizadas para dar vida aos ambientes nostálgicos característicos de tempos passados, ressaltando o caráter fantasioso do jogo. Músicas de ação para momentos de batalha e guitarras distorcidas em chefes poderosos passando a sensação de um momento decisivo na vida do herói.

//TODO incluir imagens dos mapas e fases do jogo;

## Mapas:

Os mapas serão representados neste documento através de diagramas de Caso de Uso, onde cada caso de uso representa um mapa e suas associações.

	//=========================
	// Locais do capitulo 1
	//=========================

	//=========================
	// Bosque das Colinas
	// Casa do caçador
	// Cidade de Uruk
	//	 Palácio de Uruk
	//=========================	

O primeiro mapa do jogo é o Bosque das Colinas, nele acontecerá a cena de Alfr se deparando com Enkidu no riacho, então o jogador tomará posse do controle sobre Alfr para guiá-lo pelo bosque até a saída para o mapa, em direção a sua casa.

￼
Imagem 3 - Modelo do mapa da região do Bosque das Colinas

Imagem 4 - Bosque 1				   
Imagem 5 - Bosque 2
Imagem 6 - Riacho das Colinas                              
Imagem 7 - Colinas 1
Imagem 8 - Colinas 2
Imagem 9 - Modelo do mapa da Casa do Caçador
Imagem 10 - Casa do Caçador Fora
Imagem 11 - Casa do Cacador Dentro
Imagem 11 - Modelo do mapa da Cidade de Uruk
Imagem 12 - Cidade de Uruk
Imagem 13 - Loja de Itens, Loja de armas e Equips, Covenstead
Imagem 14 - PUB, INN
￼Imagem 15 - Entrada do Palácio de Uruk, Palácio de Uruk
￼Imagem 16 - Camara Real, Quarto de Gilgamesh

	//=========================
	// Locais do capitulo 2
	//=========================
	//=========================
	// Templos de Uruk
	// Montanha do Egalmah
	// Palácio de Egalmah
	// Trilha do Vale
	// Montanha do Vale
	// Chalé da Montanha
	// Acampamento do Pico do Vale
	// Rota do Cedro
	// Montanha do Cedro
	// Floresta do Cedro
	//	Ruínas do Cedro
	//	Gruta das Aranhas
	//========================

￼
Imagem 17 - Modelo do mapa Templos de Uruk
Imagem 18 - Entrada dos Templos de Uruk
Imagem 19 - Templos de Shamash e Templo de Ishtar
Imagem 20 - Templo de Anu
Imagem 21 - Montanha do Egalmah 
Imagem 22 - Montanha do Egalmah - Area 1
Imagem 23 - Montanha do Egalmah - Area 2
Imagem 24 - Montanha do Egalmah - Area 3
Imagem 24 - Montanha do Egalmah - Area 4
￼Imagem 25 - Montanha do Egalmah - Area 5( Esquerda) e Area 6 (Direita)
magem 26 - Montanha do Egalmah - Area 7( Esquerda) e Area 8 (Direita)
magem 27 - Montanha do Egalmah - Area 9( Esquerda) e Area 10 (Direita)
Imagem 28 - Palácio do Egalmah
Imagem 30 - Entrada do palácio(esquerda), Sala 1 (Direita)
Imagem 31 - Salão principal (Esquerda), INN (Direita)
Imagem 32 - Loja de Itens (Esquerda), Camara Real (Direita)
Imagem 33 - Escadaria 1 (Esquerda), Escadaria 2 (Direita)
Imagem 34 - Escadaria 3 (Esquerda), Topo da Torre (Direita)
Imagem 35 - Trilha do vale
Imagem 36 - Area1
Imagem 37 - Area2 (esquerda), Area3 (direita)
Imagem 38 - Area4 (esquerda), Area5 (direita)
Imagem 39 - Area6 (esquerda), Area7 (direita)
￼

	//=========================
	// Locais do capitulo 3
	//=========================

	//=========================
	// Palácio de Anu
	// Fenda do Vale
	// Eufrates
	// Netherworld
	//	Palácio de Ereshkigal
	//=========================

	￼

	//=========================
	// Locais do capitulo 4
	//=========================


	//=========================
	// Babilônia
	// 	Torre do Céu
	// 	A Biblioteca
	// Gormet
	//	Calabouço Selado
	// Prisão de Troma
	// Rota de Troma
	// Fossos Basílicos
	//=========================

	//=========================
	// Locais do capitulo 5
	//=========================

	//=========================
	// Saqqara
	// 	Djoser
	// 		Complexo de Djoser
	// 		Calabouço de Imhotep
	// Cairo
	// 	Gizé
	//		Complexo de Gizé
	//	Quéops 
	// 		Complexo de Quéops
	//=========================

	//=========================
	// Locais do capitulo 6
	//=========================

	//=========================
	// Cemitério de Toga
	// 	Trilha do Netherworld
	// Netherworld
	//	Palácio de Ereshkigal
	//	Vale das Sombras
	//	Salão dos mortos
	//=========================

	//=========================
	// Locais do capitulo 7
	//=========================

	//=========================
	// Pico do Paraíso
	// 	Palácio Divino
	// Cidadela
	// Trilha sagrada
	// O Bortumenal
	//=========================

	//=========================
	// Locais do capitulo 8
	//=========================

	//=========================
	// Torre do Céu
	// 	Topo do Mundo
	// 	Casa de Shamash
	//=========================

## Itens

### Itens de Cura

|Nome|Tipo|Valor|Descrição|Imagem|
|----|----|-----|---------|------|
|Pão Sírio|Consumível fora de batalha|20|Pão integral com sementes ricas em Omega3. Restaura 250 pontos de vida de um personagem.|imagem|
|Queijo|Consumível fora de batalha|50|Queijo de ovelha com sementes ricas em Omega3. Restaura 500 pontos de vida de um personagem.|
|Elixir Pequeno|Consumível|150|Restaura 500 pontos de vida de um personagem|imagem|
|Elixir Médio|Consumível|800|Restaura 2500 pontos de vida de um personagem|imagem|
|Elixir Grande|Consumível|1500|Restaura 5000 pontos de vida de um personagem|imagem|
￼|Ultralixir|Consumível|5000|Restaura o máximo de vida de um personagem|imagem|
|Salmão|Consumível fora de batalha|250|Restaura 1500 pontos de vida de um personagem|imagem|
￼|Maçã da Deusa|Consumível fora de batalha|1000|Restaura 5000 pontos de vida de um personagem|imagem|
|Pão do Céu|Consumível fora de batalha|5000|Restaura completamente a vida de um personagem|imagem|
|Suco de laranja|Consumível fora de batalha|50|Restaura 50 pontos de energia de um personagem|imagem|
|Pote de Mel|Consumível fora de batalha|250|Restaura 150 pontos de energia de um personagem|imagem|
|Cerveja|Consumível fora de batalha|500|Restaura 500 pontos de energia de um personagem|imagem|
￼|Gota Divina|Consumível fora de batalha|1500|Restaura completamento os pontos de energia de um personagem|imagem|
|Cesta de pães|Consumível fora de batalha|120|Restaura 250 pontos de vida de todos os personagens.|imagem|
|Cesta de maçãs|Consumível fora de batalha|500|Restaura 500 pontos de vida de todos os personagens.|imagem|
￼|Bolo de Carne|Consumível fora de batalha|2000|Restaura 1500 pontos de vida de todos os personagens.|imagem|
|Frutapão Divino|Consumível fora de batalha|6000|Restaura 5000 pontos de vida de todos os personagens.|imagem|
|Jarra de Suco|Consumível fora de batalha|200|Restaura 50 pontos de energia de todos os personagens.|imagem|
|Vinho|Consumível fora de batalha|500|Restaura 150 pontos de energia de todos os personagens.|imagem|
￼
Hidromel
Consumível fora de batalha
 2000
Restaura 500 pontos de energia de todos   os personagens.
￼
Lágrimas de Aruru
Consumível fora de batalha
6000
Restaura completamente os pontos de energia de todos   os personagens.
￼
Ambrosia
Consumível fora de batalha
10000
Restaura completamente os pontos de vida e  energia de um personagem.
￼
Manjar
Consumível fora de batalha
25000
Restaura completamente os pontos de vida e  energia de todos  os personagens.
￼
Chá de Losna
Consumível
50
Cura confusão
￼
Chá de Canela
Consumível
50
Cura paralisia 

Maçã
Consumível fora de batalha
10
Restaura 50 pontos de vida de um personagem
￼
Mel de Abelha
Consumível fora de batalha
 25
Restaura 10 pontos de energia de um personagem
￼
Óleo Solar
Consumível em batalha
1000
Invoca as forças masculinas aumentando a força física do personagem
￼
Óleo Lunar
Consumível em batalha
1000
Invoca as forças femininas aumentando a força magica do personagem
￼
Óleo de Proteção
Consumível em batalha
1000
Aumenta temporariamente a defesa física do personagem
￼
Óleo de Patchuli
Consumível em batalha
1000
Aumenta temporariamente a defesa magica do personagem
￼
Óleo de Anis
Consumível em batalha
5000
Aumenta temporariamente a sorte do personagem
￼
Óleo de Madressilva
Consumível
50
Cura envenenamento
￼
Damiana
Consumível
50
Cura miopia
￼
Estoraque
Consumível
250
Cura TDAH 
￼
Pedra vital
Consumível
1000
Cura Nocaute
￼

Itens Mágicos
Nome
Valor
Descrição
Imagem
Lavanda
100
Planta possuidora dos elementos do Ar
￼
Mirra
100
Planta possuidora dos elementos da Água
￼
Almíscar
100
Planta possuidora dos elementos do Fogo
￼
Narciso
100
Planta possuidora dos elementos da Terra
￼
Cravos-da-índia
150
Planta possuidora de poderes curativos
￼



Itens de síntese e comercializáveis
Nome
Valor
Descrição
Imagem
Visco
100
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Algália
100
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Olíbano
100
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Cipreste
100
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Noz-moscada
150
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Benjoim
250
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Cânfora
250
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Sangue-de-dragão
250
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Orégano-de-Creta
250
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Cedro
300
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Ametista
400
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Agua-Marinha
500
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Jade
600
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Lapis-Lazuli
1000
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Presas Afiadas
200
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Garras Afiadas
400
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Raizes de Cedro
300
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Raizes de Carvalho
500
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Bolotas de Carvalho
400
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Madeira de Cipreste
300
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Mythril
5000
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Ferro Puro
400
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼
Madeira de Carvalho
1000
Especiaria que pode ser utilizada em receitas ou vendida no mercado
￼

Armas e Equipamentos
Nome
Valor
Descrição
Tipo
Imagem
Arco de madeira
500
Arco de madeira de pinos, usado por caçadores do vale.
Arma
￼
Espada de Ferro
600
Espada de Ferro típica da terra de Uruk.
Arma
￼
Cajado de madeira
400
Cajado de madeira de pinos.
Arma
￼
Garras Selvagens
400
Garras afiadas como as de uma fera do mato.
Arma
￼
Arco Recurvo
700
Arco de eucalipto recurvo, consegue atingir 56 libras.
Arma
￼
Espada Majestosa
1200
Espada refinada cuja lâmina 120 libras
Arma
￼
Força dos Heróis
1200
Machado reforçado  cujas lâminas possuem 180 libras
Arma
￼
Anshan
1200
Arco feito para ajudar na empreitada contra o monstro Humbaba.
Arma
￼
Arco de Ossos
2400
Arco longo feito de ossos reforçados, consegue atingir até 78 libras.
Arma
￼
Cajado de Ossos
2400
Cajado de ossos enfeitiçados.
Arma
￼
Espada de Ossos
2400
Lâmina feita a partir do ossos de alguma criatura muito grande.
Arma
￼
Garras de Ossos
2400
Garras arrancadas de alguma fera extremamente feroz.
Arma
￼
Plifortigita
4000
Arco Recurvo reforçado com potência de 102 libras.
Arma
￼
Sabro
4000
Espada que pertenceu a um grande herói de outros tempos.
Arma
￼
Duklingoj
4000
Machado Simples capaz de abrir um buraco em uma parede.
Arma
￼
Magiisto
4000
Cajado cujas lendas dizem possuir um grande poder.
Arma
￼
Arco Dourado
8000
Arco dourado feito pelos ferreiros dos deuses.
Arma
￼
Espada Divina
8000
Espada feita de ouro maciço, forjada pelos ferreiros dos deuses.
Arma
￼
Cajado Dourado
8000
Cajado feito de ouro maciço, forjado pelos ferreiros dos deuses
Arma
￼
Machado Divino
8000
Machado feito de ouro puro, forjado pelos ferreiros dos deuses
Arma
￼
Escudo de Madeira
500
Escudo comum feito de madeira de pinos.
Escudo
￼
Escudo de Ferro
1500
Escudo de ferro padrão.
Escudo
￼
Escudo Reforçado
3500
Escudo Reforçado em camadas de ferro e madeira.
Escudo
￼
Jadar
5000
Diz-se que esse escudo é como se fosse uma parede.
Escudo
￼
Escudo Divino
9000
Escudo de Ouro feito pelos ferreiros dos deuses.
Escudo
￼
Cota de Couro
500
Roupa feita de couro animal.
Armadura Leve
￼
Cota de Malha
1500
Proteção feita de anéis de ferro.
Armadura Leve
￼
Roupão
500
Roupão extenso que cobre praticamente o corpo inteiro.
Armadura Mágica
￼
Armadura de Ferro
600
Armadura feita de ferro fundido.
Armadura Pesada
￼
Manto Encantado
1500
Manto comprido encantado com bruxarias.
Armadura Mágica
￼
Armadura Temperada
1550
Armadura de aço temperado com materiais resistentes.
Armadura Pesada
￼
Cota temperada
1500
Cota feita com argolas de aço temperado.
Armadura Leve
￼
Vestes do Conjurador
4000
Vestes sagradas que aumentam a força de espirito.
Armadura Mágica
￼
Armadura Reforcada
4000
Armadura reforçada 
Armadura Pesada
￼
Cota Negra
3550
Cota feita de malha temperada com dupla camada de anéis forjados sob magia negra
Armadura Leve
￼
Manto de Aruru
8000
Manto Sagrado confeccionado pela própria Deusa Aruru.
Armadura Mágica
￼
Cota de Ouro
8000
Cota feita com  três camadas de argolas de ouro maciço.
Armadura Leve
￼
Armadura de Ouro
8000
Armadura feita de ouro puro, forjada pelos ferreiros dos Deuses.
Armadura Pesada
￼
Adagas de Caçador
1000
Adagas utilizadas por caçadores em substituição do escudo.
Escudo/arma secundaria
￼
Athame 
1000
Athame utilizado por feiticeiros em substituição de um escudo
Escudo/arma secundaria
￼
Shoto
1000
Lâmina secundária de um guerreiro, pode ser utilizada em substituição de um escudo.
Escudo/arma secundaria
￼
Garras Embutidas
1000
Garras Selvagens afiadas como espadas, pode ser utilizadas em substituição do escudo.
Escudo/ arma secundaria
￼
Chapéu
500
Chapéu pequeno de tecido
Cabeça Leve
￼
Bandana
1000
Bandana de tecido comum
Cabeça Leve
￼
Chapéu de Seda
2000
Chapéu de seda oriunda dos povos orientais
Cabeça Leve
￼
Chapéu de Pena
4000
Chapéu artesanal com uma pena de adorno
Cabeça Leve
￼
Chapéu pontudo
500
Chapéu pontiagudo utilizado pelos bruxos
Cabeça Magico
￼
Capuz
1000
Capuz que recobre toda cabeça e oculta a face
Cabeça Magico
￼
Chapéu de Feiticeira
2500
Chapéu característico dos feiticeiros
Cabeça Magico
￼
Ornamento divino
5000
Ornamento prateado que lembra muito uma coroa
Cabeça Magico
￼
Elmo de Ferro
600
Elmo feito de ferro fundido
Cabeça Pesado
￼

Elmo de Ossos

1200
Elmo feito de ossos resistentes de animais
Cabeça Pesado
￼
Elmo de Aço
2400
Elmo feito de Aço temperado
Cabeça Pesado
￼
Elmo de Ouro
5000
Elmo forjado pelos ferreiros dos Deuses, feito de ouro puro.
Cabeça Pesado
￼

Itens Sintéticos
Nome
Valor
Descrição
Requisitos
Imagem
Incenso de Lavanda
1000
Incenso possuidor do elemento Ar
10x Lavanda
10x Visco
10x Benjoim
500x Gold
￼
Incenso de Mirra
1000
Incenso possuidor do elemento Água
10x Mirra
10x Algália
10x Cânfora
500x Gold
￼
Incenso de Almíscar
1000
Incenso possuidor do elemento Fogo
10x Almíscar
10x Olíbano
10x Sangue-de-Dragão
500x Gold
￼
Incenso de Narciso
1000
Incenso possuidor do elemento Terra
10x Narciso
10x Cipreste
10x Orégano-de-creta
500x Gold
￼
Incenso de Cravos-da-índia
1500
Incenso possuidor de poderes curativos
10x Cravos-da-índia
10x Noz-mocada
10x Cedro
500x Gold
￼
Arco de Cipreste
2000
Arco longo feito de madeira de Cipreste
10x Madeira de Cipreste
15x Cipreste
1x Arco de ossos
1x Anshan
15000x Gold
￼
Arco de Mythril
15000
Arco recurvo reforçado feito de ouro e mythril
25x Lapislazuli
25x Mythril
1x Arco Dourado
1x Arco de Cipreste
50000x Gold
￼
Espada Púrpura
3500
Espada reluzente adornada com Ametistas
99x Ametista
25x Agua-marinha
2x Sabro
15000x Gold
￼
Espada de Mythril
20000
Espada longa feita de ouro e mythril
25x Lapislazuli
25x Mythril
1x Espada Divina
1x Espada Púrpura
50000x Gold
￼
Machado do Cedro
2000
Machado poderoso feito de Aço e madeira de Cedro
70x Cedro
99x Ferro Puro
1x Forca dos Heróis
1x Duklingoj
15000x Gold
￼
Machado de Mythril
14000
Grande machado cujas láminas são feitas de Mythril e sua empunhadura é feita de ouro
25x Mythril
25x Lapislazuli
1x Machado do Cedro
1x Machado Divino
50000x Gold
￼
Cajado de Carvalho
4000
Cajado feito com madeira de carvalho
50x Jade
50x Bolotas de Carvalho
25x madeira de Carvalho
1x Magiisto
15000x Gold
￼
Cajado de Mythril
16000
Lendário cajado construído a partir de ouro e mythril
25x Mythril
25x Lapislazuli
1x Cajado Dourado
1x Cajado de Carvalho
50000x Gold
￼
Essência de Lavanda
5000
Essência capaz de invocar os poderes do Ar
1x Ametista
5x Bolotas de Carvalho
10x Incenso de Lavanda
10x Benjoim
3000x Gold
￼
Essência de Mirra
5000
Essência capaz de invocar os poderes da água
1x Ametista
5x Raizes de Cedro
10x Incenso de Mirra
10x Algália
3000x Gold
￼
Essência de Almíscar
5000
Essência capaz de invocar os poderes do fogo
1x Ametista
5x Raizes de carvalho
10x Incenso de Almiscar
3000x Gold
￼
Essência de Narciso
5000
Essência capaz de invocar os poderes da terra
1x Jade
5x Ametista
10x Incenso de Narciso
10x Madeira de Cipreste
3000x Gold
￼
Essência de Cravos-da-índia
6000
Essência curativa
5x Ametista
5x Agua-Marinha
5x Jade
10x Incenso de Cravos-da-índia
3000x Gold
￼

Acessórios
Nome
Valor
Descrição
Imagem
Anel
100
Anel comum feito de bronze
￼
Luvas de Couro
150
Luvas feitas de couro animal
￼
Pulseira de Bronze
200
Pulseira feita a partir da ligação de elos de bronze 
￼
Colar de Ametista
500
Colar adornado em ametistas lapidadas
￼
Pé de Coelho
8000
Dizem que traz boa sorte
￼
Anel de prata
1200
Anel feito de prata pura adornado com rubis
￼
Amuleto
1400
Dizem que protege o espirito
￼
Sandálias
500
Ajuda a proteger da areia quente do deserto
￼
Botas
1000
Botas de couro resistentes para longas jornadas
￼
Luvas de Aço
2000
Luvas de cavaleiro feitas de aço fundido
￼
Botas de Aço
2000
Botas de Cavaleiro feitas de Aço fundido
￼
Anel rúnico
3000
Anel com misteriosas inscrições entalhadas adornado com esmeraldas
￼
Colar de Prata
3000
Colar feito em prata pura
￼
Anel de Ouro
5000
Anel adornado com ouro maciço
￼
Lenço de Seda
6000
Lenço feito de seda do oriente médio.
￼
Amuleto de Rubi
10000
Uma jóia forjada pelos ferreiros dos deuses
￼
Pulseira de Ouro
10000
Pulseira feira de ouro puro
￼
Colar de Pérola
10000
Colar adornado em pérolas reluzentes
￼
Jóia Divina
20000
Jóia do Cajado de Anu
￼

Itens de Receita
Nome
Valor
Descrição
Imagem
Grimório do Ar I
1000
Grimório com instruções para sintetização de incensos
￼
Grimório da Agua I
1000
Grimório com instruções para sintetização de incensos
￼
Grimório do Fogo I
1000
Grimório com instruções para sintetização de incensos
￼
Grimório da Terra I
1000
Grimório com instruções para sintetização de incensos
￼
Grimório do Curandeiro I
1000
Grimório com instruções para sintetização de incensos
￼
Projetos do Marceneiro
-
Projetos para um tipo de arco de madeira
￼
O Arco Azul
-
Antiga receita quase ilegível
￼
Livro do Ferreiro
-
Passo-a-passo do ferreiro iniciante
￼
A Espada Lendária
-
Antiga receita quase ilegível
￼
Machado de Humbaba
-
Rascunhos deixados por Humbaba na floresta
￼
Retrato do Herói
-
Antiga receita quase ilegível
￼
Bengala Druida
-
Como fazer uma típica bengala druida
￼
Cetro de Yaweh
-
Antiga receita quase ilegível
￼
Grimório do Ar II
10000
Grimório com instruções para sintetização de essências
￼
Grimório da Água II
10000
Grimório com instruções para sintetização de essências
￼
Grimório do Fogo II
10000
Grimório com instruções para sintetização de essências
￼
Grimório da Terra II
10000
Grimório com instruções para sintetização de essências
￼
Grimório do Curandeiro II
10000
Grimório com instruções para sintetização de essências
￼


Itens Chave
Nome
Descrição
Imagem
Shamat
Rameira entregue-lhe por Gilgamesh para que leve-a para seduzir a Fera das colinas.
￼
Cordeiro branco
Cordeiro branco para ser levado em  sacrificio á Shamash ns Templos de Uruk
￼


￼


￼


￼



Inimigos 
 //TODO elaborar mais inimigos

￼
Nome: Gob
HP: 100
MP: 20
Ataque: 10
Defesa:7
Agi: 5
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 10
Ouro: 5
Drop: maçã (50%)
Habilidades: Ataque

￼
Nome: Lobo das Colinas
HP: 200
MP: 20
Ataque: 16
Defesa:7
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 15
Ouro: 8
Drop: maçã (100%)
Habilidades: Ataque


￼
Nome: Serpente das Colinas
Hp: 180
Mp: 50
Ataque: 15
Defesa:8
Agi: 7
Ataque M: 7
Defesa M: 7
Sorte: 5
Exp: 15
Ouro: 8
Drop: maçã (50%);
Óleo de Madressilva(75%)
Habilidades: Ataque; Picada Venenosa

￼
Nome: Ladrão
HP: 600
MP: 20
Ataque: 23
Defesa:13
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 122
Ouro: 45
Drop: Pão sirio (50%); (Elixir P.(50%)
Habilidades: Ataque

￼
Nome: Urso das Colinas
HP: 1500
MP: 20
Ataque: 33
Defesa:15
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 45
Ouro: 14
Drop: Mel de Abelha (50%)
Habilidades: Ataque


Nome: Falcão das Colinas
HP: 1200
MP: 20
Ataque: 30
Defesa:15
Agi: 15
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 40
Ouro: 20
Drop: Salmão(1%)
Maçã x3 (100%)
Habilidades: Ataque


￼
Nome: Escorpião do Deserto
HP: 700
MP: 20
Ataque: 17
Defesa:10
Agi: 6
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 30
Ouro: 18
Drop: Óleo de Madressilva(100%)

Habilidades: Ataque; Picada Venenosa


￼
Nome: Gob do Deserto
HP: 800
MP: 20
Ataque: 20
Defesa:15
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 30
Ouro: 22
Drop: 
Maçã x2 (100%)
Habilidades: Ataque



Nome: Leão
HP: 00
MP: 20
Ataque: 20
Defesa:15
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 5
Exp: 30
Ouro: 22
Drop: 
Maçã x2 (100%)
Habilidades: Ataque



￼
Nome: Gilgamesh
HP: 2000
MP: 20
Ataque: 20
Defesa:15
Agi: 8
Ataque M: 2
Defesa M: 3
Sorte: 10
Exp: 300
Ouro: 22
Drop: 
Maçã x2 (100%)
Habilidades: Ataque


Habilidades
//TODO: adicionar tabela de habilidades de cada personagem principal
Subquests

O jogo apresentará um sistema de subquests, que serão missões alternativas de caráter não obrigatório, o que implica que o cumprimento ou não cumprimento destes eventos não influenciarão no enredo do jogo.
O sistema de caçador de recompensas será definido como principal sistema de subquests, tendo como objetivo caçar um alvo determinado e após eliminá-lo receber a recompensa pelo serviço. Nos PUBs das cidades, vilas e condados haverá um quadro de procurados listando os alvos disponíveis para o jogador escolher. Tendo escolhido o alvo, o jogador deverá conversar com o postador do cartaz para descobrir a localização do alvo, que somente estará disponível para caçada após confirmá-la com o postador. Após eliminar o alvo, o jogador deverá retornar até o postador para receber sua recompensa.


￼
Nome: Ratatosk
HP: 3000
MP: 200
Ataque: 24
Defesa:17
Agi: 8
Ataque M: 10
Defesa M: 10
Sorte: 10
Exp: 150
Ouro: 100
Drop: 
Maçã x2 (100%)
Habilidades: Ataque
Local: Bosque das Colinas[colinas_2]
Horario: Tempo todo
Capitulo I
Requisitos: Nenhum




￼
Nome: Mandíbula
HP: 5000
MP: 200
Ataque: 33
Defesa:17
Agi: 18
Ataque M: 10
Defesa M: 10
Sorte: 10
Exp: 190
Ouro: 100
Drop: 
Maçã x2 (100%)
Habilidades: Ataque
Local: Bosque das Colinas[Riacho do bosque]
Horario: Noite
Capitulo I
Requisitos: Nenhum

//TODO elaborar mais  junta 


Interface 
//TODO
- Design e ilustração do HUD (head-up display);
- Posicionamento dos elementos do HUD;
- Design e ilustração das interfaces do jogo: tela inicial, menu de opções, tela de pause, menu de itens, tela de loading, etc...


Cutscenes 
//TODO
- Descrição dos filmes que serão incluídos no jogo;
- Descrição dos roteiros;
- Qual método será usado para a criação dos filmes?
- Em quais momentos eles serão exibidos?
















Cronograma

//TODO reelaborar o cronograma

Anexos

Creditos

Stephen “Redshrike” Challener, William Thompsonj (LPC Wolf Sprite, Golem Sprite, Spider Sprite) <https://opengameart.org/users/williamthompsonj>

Avery resources and sprites (https://forums.rpgmakerweb.com/index.php?threads/avys-mv-stuff.53317/)

SumRndmDde <http://sumrndm.site>

(Referências)

Literatura:

LIMA, E. S. Modelo de Game Design Document. Web, 2014. Disponível em: <http://edirlei.3dgb.com.br/aulas/intro-eng_2014_1/Modelo_Game_Design_Document.docx>;

KOVACS, M. G; CARNAHAN, W. The Epic of Gilgamesh. Web, 1998. Disponível em: <http://www.ancienttexts.org/library/mesopotamian/gilgamesh/> ;

PRESSMAN, R. S. Engenharia de Software. Tradução de José Carlos Barbosa dos Santos. 3˚ed. Pearson - São Paulo, 2010;

SATO, A. K. O. Game Design e Prototipagem: Conceitos e Aplicações ao Longo do Processo Projetual. IX SBGames [pg. 74 - 84] - Florianópolis - SC, 8 a 10 de Novembro de 2010. Disponível em: <http://www.sbgames.org/papers/sbgames10/artanddesign/Full_A&D_10.pdf>

OJIMA, Y. RPG Maker MV. Kadokawa Corporation. 2015;

Resources:
//TODO: Atribuir corretamente os nomes aos autores.

Moghunter (Atelier RGSS)
<https://atelierrgss.wordpress.com/> (GUI and Window Design)

Yanfly Engine Plugins. Disponível em: <http://yanfly.moe/yep/>

Frascos - https://opengameart.org/content/more-flacons

Swords - https://opengameart.org/content/32x-sword-icon

aneis - https://opengameart.org/content/anti-poison-rings


Necklaces and amulets - https://opengameart.org/content/loyalty-lies-equipment-amulets-necklaces

Key icons -https://opengameart.org/content/key-icons

Axes - https://opengameart.org/content/axe-icons-from-pixeltime-videos

Bows - https://opengameart.org/content/bow-icons-from-pixeltime-videos

Archer and bows set - https://opengameart.org/content/archer-job-set

Food set - https://henrysoftware.itch.io/pixel-food

Daggers - https://opengameart.org/content/loyalty-lies-equipment-daggers

Hands and gloves - https://opengameart.org/content/loyalty-lies-equipment-gauntlets-brass-knuckles

Head equipment - https://opengameart.org/content/loyalty-lies-equipment-masks-hats

Helmets - https://opengameart.org/content/loyalty-lies-equipment-helmets

Staffs 1 - https://opengameart.org/content/loyalty-lies-equipment-staffs-wands

Staffs 2 - https://opengameart.org/content/staff-icons-from-pixeltime-videos

Frascos - https://opengameart.org/content/more-flacons

Armor - https://opengameart.org/content/24-armor-icons

Items - https://opengameart.org/content/items

Shield - https://opengameart.org/content/shield-0

Shields - https://opengameart.org/content/shield-icons-from-pixeltime-videos

Potions and berryes - https://raventale.itch.io/daily-doodles-pixelart-asset-pack

Treasure - https://opengameart.org/content/golden-treasures
