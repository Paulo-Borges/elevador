Bem-vindo(a) ao projeto Elevador Divertido! Uma simulação simples, mas charmosa, de um elevador em um prédio de 6 andares mais o térreo. Prepare-se para ver o seu elevador subir e descer (assim que o código JavaScript de movimentação estiver completo, é claro 😉)!

🛠️ Tecnologias Usadas
Este projeto é um clássico "três mosqueteiros" do desenvolvimento web:

HTML5: A espinha dorsal da nossa estrutura, definindo o prédio, a calçada, a rua e, claro, os botões de controle do elevador.

CSS3: O toque de mágica visual! Usamos CSS para dar cor, forma e vida a todos os elementos. Variáveis CSS (:root) foram usadas para facilitar a customização de cores, e o flexbox (com certeza!) está ajudando a organizar a bagunça!

JavaScript (Puro!): O cérebro da operação. Por enquanto, ele já está fazendo a parte chata de gerar as faixas da rua automaticamente usando o atributo faixas no HTML. A próxima missão dele é fazer o elevador se mover de verdade!

🏗️ Como a Mágica Acontece (Por Dentro)
Dê uma olhada na estrutura básica do nosso prédio, rua e controles:

🧱 Estrutura HTML
O HTML é organizado para que o JavaScript possa facilmente manipular e gerar elementos:

Controles: A área superior (div.controles) tem o mostrador (div.mostrador) e os botões de andar (<button>).

Prédio: A calçada (div.calcada) abriga o prédio (div.predio), que tem duas colunas laterais (div.coluna) com o atributo andares="6". Essas colunas esperam que o JavaScript (futuramente) crie os andares e as portas dinamicamente. O poço do elevador (div.poco) fica no meio.

Rua: O elemento (div.rua) usa o atributo faixas="15" que é lido pelo nosso script JS inicial.

🎨 Estilização CSS
A estilização atual já nos dá um look noturno e tecnológico, com uma fonte de terminal (VT323) para o mostrador.

Variáveis: Definimos as cores principais no :root para um tema noturno (--color-rua, --color-predio, etc.).

Flexbox: O div.calcada usa display: flex para posicionar as árvores e o prédio. O body também usa flex para organizar a calçada e a rua verticalmente.

🧠 JavaScript Inicial
O arquivo script.js já tem um módulo inicial com uma função super útil:

JavaScript

export default function criarFaixas() {
// ... pega todos os elementos que têm o atributo 'faixas'
// ... e cria a quantidade correta de div's (as faixas da rua)!
}
Isso nos mostra que o código já está pronto para automatizar a criação de elementos com base em atributos no HTML, um ótimo ponto de partida para gerar os andares e a cabine do elevador no futuro!

🔜 Próximos Passos (Onde a Diversão Começa!)
Este é apenas o esqueleto. A verdadeira diversão está por vir!

Criar Andares: Usar JavaScript para gerar os andares (div.andar, div.porta) e a cabine do elevador (div.cabine) dentro do div.poco, lendo o atributo andares="6" da coluna.

Movimentação: Adicionar event listeners aos botões para que o elevador se mova (usando transformações CSS como translateY) e atualizar o mostrador com o andar atual.

Animação: Fazer as portas abrirem e fecharem de forma animada.

Quer dar uma força? Sinta-se à vontade para clonar o projeto e fazer o elevador finalmente andar! 🆙
