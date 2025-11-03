<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guia Portage de Educação Pré-Escolar - Documento Completo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f7f6;
            color: #333;
        }
        .container {
            max-width: 1200px;
            margin: auto;
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #007bff;
            border-bottom: 3px solid #007bff;
            padding-bottom: 15px;
            margin-top: 0;
            text-align: center;
        }
        h2 {
            color: #28a745;
            border-bottom: 2px solid #28a745;
            padding-bottom: 8px;
            margin-top: 30px;
        }
        h3 {
            color: #17a2b8;
            margin-top: 15px;
        }
        .identification-fields div {
            margin-bottom: 15px;
        }
        .identification-fields label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }
        .identification-fields input[type="text"], 
        .identification-fields input[type="date"] {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }
        .legend {
            margin-bottom: 20px;
            padding: 15px;
            background-color: #f8f9fa;
            border: 1px dashed #ced4da;
            border-radius: 4px;
        }
        .legend p {
            margin: 5px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            font-size: 0.9em;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #007bff;
            color: white;
            position: sticky;
            top: 0;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        .age-range-header {
            background-color: #17a2b8;
            color: white;
            font-weight: bold;
            text-align: center;
            padding: 10px;
            font-size: 1.1em;
        }
        .result-cell {
            white-space: nowrap;
            width: 150px; 
            text-align: center;
        }
        .result-cell label {
            margin-right: 10px;
        }
        textarea {
            width: 100%;
            min-height: 100px;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            margin-top: 10px;
        }
        .dicas li {
            margin-bottom: 8px;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Guia Portage de Educação Pré-Escolar</h1>
    <p style="text-align: center;">A escala para avaliação e cálculo da idade de desenvolvimento — Documento Completo e Interativo.</p>

    <section>
        <h2>I. Dados do Educando e da Avaliação</h2>
        <div class="identification-fields">
            <div>
                <label for="nome">Nome do educando:</label>
                <input type="text" id="nome">
            </div>
            <div>
                <label for="nascimento">Data de Nascimento:</label>
                <input type="date" id="nascimento">
            </div>
            <div>
                <label for="diagnostico">Diagnóstico:</label>
                <input type="text" id="diagnostico">
            </div>
            <div>
                <label for="avaliacao">Data da avaliação:</label>
                <input type="date" id="avaliacao">
            </div>
        </div>

        <div class="legend">
            <h3>Legendas para Preenchimento dos Resultados:</h3>
            <p><strong>S:</strong> Sim (alcançou)</p>
            <p><strong>N:</strong> Não (ainda não alcançou)</p>
            <p><strong>AV:</strong> Às vezes</p>
            <p><strong>Obs:</strong> Marque utilizando as legendas acima, baseado no Manual do Inventário Operacionalizado Portage.</p>
        </div>
    </section>

    <div id="scales-container">
        </div>

    <section>
        <h2>III. Observações e Dicas</h2>
        <label for="observacoes" style="font-weight: bold;">Observações Adicionais e Metas:</label>
        <textarea id="observacoes" placeholder="Registre aqui observações, pontos fortes, desafios e os objetivos prioritários (não alcançados) para o aluno."></textarea>
        
        <div class="legend">
            <h3>Dicas do Guia Original:</h3>
            <ul class="dicas">
                <li>Devem ser selecionados para trabalho os objetivos que são prioritários para o aluno, ou seja, os não alcançados.</li>
                <li>Os objetivos em que o aluno obteve <strong>AV</strong> (às vezes) devem ser trabalhados para reforço até que sejam alcançados.</li>
                <li>À medida que cada objetivo for alcançado, ele deverá ser substituído por outro da mesma área na mesma folha.</li>
                <li>O professor não deve restringir-se apenas aos objetivos do Portage. Deve haver dinamismo para trabalhar as dificuldades que forem surgindo.</li>
                <li>Sempre considere a individualidade de cada aluno. Ninguém é igual a ninguém.</li>
            </ul>
        </div>
        
        <p style="margin-top: 20px; font-style: italic;">Para dicas e a tabela de cálculo automático da idade de desenvolvimento, consulte o e-book do Instituto Itard (mencionado no documento original): [E-book Instituto Itard](https://institutoitard.com.br/categoria/livros/)</p>
    </section>

</div>

<script>
    // JSON COMPLETO COM TODOS OS 540+ ITENS DO GUIA PORTAGE
    const escalas = {
        "Socialização": {
            "0 a 1 ano": [
                { num: "01", item: "Observa uma pessoa movimentando-se em seu campo visual." },
                { num: "02", item: "Sorri em resposta à atenção do adulto." },
                { num: "03", item: "Vocaliza em resposta à atenção." },
                { num: "04", item: "Olha para sua própria mão, sorrindo ou vocalizando." },
                { num: "05", item: "Responde a seu círculo familiar, sorrindo, vocalizando ou parando de chorar." },
                { num: "06", item: "Sorri em resposta à expressão facial dos outros." },
                { num: "07", item: "Sorri e vocaliza ao ver sua imagem no espelho" },
                { num: "08", item: "Acaricia ou toca no rosto de adultos (puxa cabelo, nariz, óculos, etc.)." },
                { num: "09", item: "Estende a mão em direção a um objeto oferecido." },
                { num: "10", item: "Estende os braços em direção a pessoas familiares." },
                { num: "11", item: "Estende a mão e toca sua imagem refletida no espelho." },
                { num: "12", item: "Segura e examina por 1 minuto um objeto que lhe foi dado." },
                { num: "13", item: "Sacode ou aperta um objeto colocado em sua mão, produzindo sons involuntários." },
                { num: "14", item: "Brinca sozinho por 10 minutos." },
                { num: "15", item: "Procura contato visual quando alguém lhe dá atenção por 2 a 3 minutos." },
                { num: "16", item: "Brinca sozinho sem reclamar por 15 a 20 minutos, próximo de um adulto." },
                { num: "17", item: "Vocaliza para obter atenção." },
                { num: "18", item: "Imita adulto em brincadeiras de esconde-esconde." },
                { num: "19", item: "Bate palmas, imitando um adulto." },
                { num: "20", item: "Acena a mão, imitando um adulto." },
                { num: "21", item: "Ergue os braços para expressar 'grande', imitando um adulto." },
                { num: "22", item: "Oferece algo, mas nem sempre entrega." },
                { num: "23", item: "Abraça, acaricia e beija familiares." },
                { num: "24", item: "Responde ao próprio nome, olhando ou estendendo o braço para ser pego." },
                { num: "25", item: "Aperta ou sacode um brinquedo para produzir sons, em imitação." },
                { num: "26", item: "Manipula brinquedo ou objeto." },
                { num: "27", item: "Estende um brinquedo ou objeto a um adulto e o entrega." },
                { num: "28", item: "Imita movimentos de outras crianças ao brincar." }
            ],
            "1 a 2 anos": [
                { num: "29", item: "Imita um adulto em uma tarefa simples." },
                { num: "30", item: "Brinca ao lado de outra criança, cada uma realizando tarefas diferentes." },
                { num: "31", item: "Toma parte em uma brincadeira com outra criança por 2 a 5 minutos." },
                { num: "32", item: "Aceita a ausência dos pais, embora possa reclamar." },
                { num: "33", item: "Explora ativamente seu meio ambiente." },
                { num: "34", item: "Realiza atividade manipulativa com outra pessoa." },
                { num: "35", item: "Abraça e carrega uma boneca ou brinquedo macio." },
                { num: "36", item: "Repete ações que produzem risos e atenção." },
                { num: "37", item: "Dá um livro para que um adulto o leia ou para que ambos o compartilhem." },
                { num: "38", item: "Puxa uma pessoa a mostrar-lhe algo." },
                { num: "39", item: "Retira a mão ou diz 'não' quando está próximo de um objeto não permitido e alguém o lembra disto." },
                { num: "40", item: "Quando colocado em sua cadeira ou trocador espera ser atendido." },
                { num: "41", item: "Brinca com 2 ou 3 crianças da sua idade." },
                { num: "42", item: "Compartilha um objeto ou alimento com outra criança." },
                { num: "43", item: "Cumprimenta colegas ou adultos quando lembrado." }
            ],
            "2 a 3 anos": [
                { num: "44", item: "Obedece às ordens dos pais pelo menos 1½ das vezes." },
                { num: "45", item: "Busca / leva um objeto ou pessoa, quando solicitado." },
                { num: "46", item: "Presta atenção à estória ou música por 5 a 10 min." },
                { num: "47", item: "Diz 'Por favor' ou 'Obrigado' quando lembrado." },
                { num: "48", item: "Tenta ajudar os pais a executarem tarefas realizando parte da mesma." },
                { num: "49", item: "Brinca de usar roupas de adultos." },
                { num: "50", item: "Faz uma escolha quando indagado." },
                { num: "51", item: "Demonstra entender sentimentos, expressando-os." }
            ],
            "3 a 4 anos": [
                { num: "52", item: "Canta e dança ao ouvir músicas." },
                { num: "53", item: "Segue regras de um jogo imitando ações de outras crianças." },
                { num: "54", item: "Cumprimenta pessoas familiares sem ser lembrado." },
                { num: "55", item: "Seguem regras em jogos de grupos dirigidos por adultos." },
                { num: "56", item: "Pede permissão para brincar com um brinquedo que está sendo usado por outra criança." },
                { num: "57", item: "Diz 'Por favor' e 'Obrigado' sem ser lembrado 1½ das vezes." },
                { num: "58", item: "Atende ao telefone, chamando um adulto e falando com pessoas familiares." },
                { num: "59", item: "Espera a sua vez." },
                { num: "60", item: "Segue regras em jogos dirigidos por uma criança mais velha." },
                { num: "61", item: "Obedece às ordens de um adulto 75% das vezes. (3 vezes a cada 4 tentativas)" },
                { num: "62", item: "Permanece em seu próprio quintal ou jardim." },
                { num: "63", item: "Brinca perto de outras crianças conversando com elas enquanto trabalha em um projeto próprio (30 min.)." }
            ],
            "4 a 5 anos": [
                { num: "64", item: "Pede ajuda quando está tendo dificuldades." },
                { num: "65", item: "Contribui para a conversa de adultos." },
                { num: "66", item: "Repete rimas, canções ou dança para os outros." },
                { num: "67", item: "Faz uma tarefa sozinha por 20 a 30 minutos." },
                { num: "68", item: "Pede desculpas sem ser lembrado 75% das vezes." },
                { num: "69", item: "Espera sua vez em brincadeiras que envolvam de 8 a 9 crianças." },
                { num: "70", item: "Brinca com 2 a 3 crianças por 20 min. em uma atividade que envolva cooperação." },
                { num: "71", item: "Quando em público, apresenta um comportamento socialmente aceitável." },
                { num: "72", item: "Pede permissão para usar objetos dos outros em 75% das vezes." }
            ],
            "5 a 6 anos": [
                { num: "73", item: "Manifesta seus sentimentos." },
                { num: "74", item: "Brinca com 4 a 5 crianças em atividade de cooperação por 20 minutos, sem supervisão." },
                { num: "75", item: "Explica aos outros as regras do jogo ou atividade." },
                { num: "76", item: "Imita papéis de adulto." },
                { num: "77", item: "Colabora para a conversa durante as refeições." },
                { num: "78", item: "Segue regras de jogo que envolva raciocínio verbal." },
                { num: "79", item: "Conforta colegas quando estes estão tristes." },
                { num: "80", item: "Escolhe seus próprios amigos." },
                { num: "81", item: "Planeja e constrói, usando ferramentas simples." },
                { num: "82", item: "Estabelece metas para si próprio e executa atividade para atingi-las." },
                { num: "83", item: "Dramatiza trechos de histórias, desempenhando um papel ou utilizando fantoches." }
            ]
        },
        "Linguagem": {
            "0 a 1 anos": [
                { num: "01", item: "Repete sons emitidos por outras pessoas." },
                { num: "02", item: "Repete a mesma sílaba 2 a 3 vezes." },
                { num: "03", item: "Responde a gestos com gestos." },
                { num: "04", item: "Obedece a uma ordem simples, quando acompanhada de gestos indicativos." },
                { num: "05", item: "Interrompe a atividade quando lhe dizem 'Não' 75% das vezes." },
                { num: "06", item: "Responde a perguntas simples com respostas não verbais." },
                { num: "07", item: "Combina 2 sílabas diferentes quando tenta verbalizar." },
                { num: "08", item: "Imita padrões de entonação da voz de outras pessoas." },
                { num: "09", item: "Usa uma palavra funcionalmente para indicar objetos ou pessoas." },
                { num: "10", item: "Vocaliza em resposta à fala de outras pessoas." }
            ],
            "1 a 2 anos": [
                { num: "11", item: "Diz 5 palavras diferentes." },
                { num: "12", item: "Pede 'mais'." },
                { num: "13", item: "Diz 'acabou'." },
                { num: "14", item: "Obedece a 3 ordens diferentes que não são acompanhadas de gestos indicativos." },
                { num: "15", item: "Consegue 'dar' ou 'mostrar' quando solicitado." },
                { num: "16", item: "Aponta para 12 objetos quando nomeados." },
                { num: "17", item: "Aponta para 3 a 5 figuras em um livro." },
                { num: "18", item: "Aponta para 3 partes de seu próprio corpo." },
                { num: "19", item: "Diz seu nome ou apelido quando solicitado." },
                { num: "20", item: "Responde à pergunta 'O que é isto?'" },
                { num: "21", item: "Combina palavras e gestos para expressar desejos." },
                { num: "22", item: "Nomeia 5 membros da família, incluindo animais." },
                { num: "23", item: "Nomeia 4 brinquedos." },
                { num: "24", item: "Produz sons de animais, ou os nomeia pelo som." },
                { num: "25", item: "Pede alimentos conhecidos pelo nome, quando mostrados." },
                { num: "26", item: "Faz perguntas variando a entonação da voz." },
                { num: "27", item: "Nomeia 3 partes do corpo em uma boneca ou outra pessoa." },
                { num: "28", item: "Responde a perguntas de sim / não." }
            ],
            "2 a 3 anos": [
                { num: "29", item: "Combina substantivos ou adjetivos e substantivos em frases de 2 palavras." },
                { num: "30", item: "Combina substantivo e verbo em frases de 2 palavras" },
                { num: "31", item: "Usa uma palavra para indicar que quer ir ao banheiro" },
                { num: "32", item: "Combina verbo ou substantivo com 'lá' e 'aqui' em frases de 2 palavras." },
                { num: "33", item: "Combina 2 palavras para expressar posse." },
                { num: "34", item: "Emprega 'não' na fala." },
                { num: "35", item: "Responde à pergunta 'O que está fazendo?' para atividade habituais." },
                { num: "36", item: "Responde a perguntas tipo 'Onde está objeto?'" },
                { num: "37", item: "Nomeia sons ambientais familiares." },
                { num: "38", item: "Dá mais de um objeto quando se usa a forma plural na solicitação." },
                { num: "39", item: "Ao falar, refere-se a si próprio pelo nome." },
                { num: "40", item: "Aponta para figuras de objetos comuns descritos pelo uso (até 10) ('O que se usa pra comer? = colher')" },
                { num: "41", item: "Mostra a idade pelos dedos." },
                { num: "42", item: "Diz seu sexo quando solicitado." },
                { num: "43", item: "Obedece à seqüência de duas ordens relacionadas." },
                { num: "44", item: "Usa a forma do verbo no gerúndio." },
                { num: "45", item: "Emprega formas regulares no plural." },
                { num: "46", item: "Emprega algumas formas irregulares de verbos no passado de forma sistemática." },
                { num: "47", item: "Faz perguntas do tipo 'O que é isso?'" },
                { num: "48", item: "Controla o volume da voz 90% das vezes." },
                { num: "49", item: "Usa 'este / esta' e 'aquele / aquela' na fala." },
                { num: "50", item: "Emprega 'é' e 'está' em frases simples." },
                { num: "51", item: "Diz 'eu', 'mim', 'meu' ao invés do próprio nome." },
                { num: "52", item: "Aponta objetos e diz que eles não são outras coisas." },
                { num: "53", item: "Responde à pergunta 'Quem?' dando um nome." },
                { num: "54", item: "Emprega as formas possessivas dos substantivos." },
                { num: "55", item: "Usa artigos ao falar." },
                { num: "56", item: "Usa substantivos que indicam grupo ou categoria." },
                { num: "57", item: "Usa os verbos 'ser', 'estar' e 'ter' no presente com poucos erros." },
                { num: "58", item: "Diz se os objetos estão abertos ou fechados." }
            ],
            "3 a 4 anos": [
                { num: "59", item: "Expressa diminutivos e aumentativos quando fala." },
                { num: "60", item: "Presta atenção por 5 minutos a uma estória lida." },
                { num: "61", item: "Obedece à sequência de 2 ordens não relacionadas." },
                { num: "62", item: "Diz seu nome completo quando solicitado." },
                { num: "63", item: "Responde perguntas simples envolvendo 'Como'." },
                { num: "64", item: "Emprega verbos regulares, no passado." },
                { num: "65", item: "Relata experiências imediatas." },
                { num: "66", item: "Diz como são usados objetos comuns." },
                { num: "67", item: "Expressa ações futuras empregando os verbos 'ir', 'ter' e 'querer'." },
                { num: "68", item: "Utiliza adequadamente masculino e feminino na fala." },
                { num: "69", item: "Usa formas imperativas de verbos ao pedir favores." },
                { num: "70", item: "Conta 2 fatos na ordem de ocorrência." }
            ],
            "4 a 5 anos": [
                { num: "71", item: "Obedece a uma sequência envolvendo 3 ordens." },
                { num: "72", item: "Demonstra compreensão de verbos reflexivos, usando-os ocasionalmente (ex. ele se machucou)." },
                { num: "73", item: "Consegue identificar objetos/figuras que formem par, sob solicitação." },
                { num: "74", item: "Emprega o futuro ao falar." },
                { num: "75", item: "Usa orações compostas por coordenação." },
                { num: "76", item: "Consegue identificar a parte de cima e de baixo de objetos, quando solicitado." },
                { num: "77", item: "Emprega ocasionalmente o condicional ao falar (poderia, pudesse, iria, seria, faria)." },
                { num: "78", item: "Consegue identificar absurdos em figuras." },
                { num: "79", item: "Emprega as seguintes palavras: irmã(o), avó, avô." },
                { num: "80", item: "Completa frases com antônimos." },
                { num: "81", item: "Relata uma estória conhecida sem ajuda de figuras." },
                { num: "82", item: "Em uma figura, nomeia o objeto que não pertence a uma determinada categoria." },
                { num: "83", item: "Diz se duas palavras rimam ou não." },
                { num: "84", item: "Usa frases complexas, compostas por subordinação." },
                { num: "85", item: "Diz se um som é forte ou fraco." }
            ],
            "5 a 6 anos": [
                { num: "86", item: "Consegue indicar alguns, muitos e vários elementos." },
                { num: "87", item: "Diz seu endereço." },
                { num: "88", item: "Diz o número de seu telefone." },
                { num: "89", item: "Aponta para o conjunto que tem mais, menos ou poucos elementos." },
                { num: "90", item: "Conta piadas simples." },
                { num: "91", item: "Relata experiências diárias." },
                { num: "92", item: "Descreve um local ou movimento: através ou entre, longe de, de / desde..., para, por cima de, até." },
                { num: "93", item: "Responde à pergunta 'Porque' com uma explicação." },
                { num: "94", item: "Ordena e conta uma estória de 2 a 5 episódios na sequência correta." },
                { num: "95", item: "Define palavras." },
                { num: "96", item: "Responde adequadamente a pergunta 'Qual o contrário de ...'." },
                { num: "97", item: "Responde a pergunta 'O que acontece se...'." },
                { num: "98", item: "Usa 'ontem' e 'amanhã, corretamente'." },
                { num: "99", item: "Pergunta o significado de perguntas novas ou conhecidas." }
            ]
        },
        "Cognição": {
            "0 a 1 anos": [
                { num: "01", item: "Remove um pano do rosto que obscureça sua visão." },
                { num: "02", item: "Procura com o olhar um objeto que foi tirado de seu campo visual." },
                { num: "03", item: "Remove um objeto de um recipiente colocando a mão dentro do mesmo." },
                { num: "04", item: "Coloca um objeto em um recipiente imitando um adulto." },
                { num: "05", item: "Coloca um objeto em um recipiente quando recebe instruções." },
                { num: "06", item: "Balança um brinquedo que produz som, pendurado em um barbante." },
                { num: "07", item: "Coloca três objetos em um recipiente e o esvazia." },
                { num: "08", item: "Transfere um objeto de uma mão à outra para apanhar outro objeto." },
                { num: "09", item: "Deixa cair e apanha um brinquedo." },
                { num: "10", item: "Descobre um objeto escondido sob um recipiente." },
                { num: "11", item: "Empurra 3 blocos como se fosse um comboio." },
                { num: "12", item: "Remove um círculo de uma prancha, por imitação." },
                { num: "13", item: "Coloca um pino redondo em uma prancha de pinos, quando solicitado." },
                { num: "14", item: "Executa gestos simples quando requisitado." }
            ],
            "1 a 2 anos": [
                { num: "15", item: "Retira 6 objetos de um recipiente, um por vez." },
                { num: "16", item: "Aponta para uma parte do corpo." },
                { num: "17", item: "Empilha 3 blocos, dada a ordem." },
                { num: "18", item: "Emparelha objetos semelhantes." },
                { num: "19", item: "Faz rabiscos no papel." },
                { num: "20", item: "Aponta para si quando perguntam 'Cadê o Fulano?'" },
                { num: "21", item: "Coloca 5 pinos redondos, dada a ordem." },
                { num: "22", item: "Emparelha objetos com a figura do mesmo nome." },
                { num: "23", item: "Aponta para a figura nomeada." },
                { num: "24", item: "Vira as páginas de um livro (2/3 por vez) para encontrar a figura nomeada." }
            ],
            "2 a 3 anos": [
                { num: "25", item: "Encontra determinado livro quando solicitado." },
                { num: "26", item: "Completa um quebra-cabeça de encaixe de 3 peças." },
                { num: "27", item: "Nomeia 4 objetos comuns em figuras." },
                { num: "28", item: "Desenha uma linha vertical imitando um adulto." },
                { num: "29", item: "Desenha uma linha horizontal imitando um adulto." },
                { num: "30", item: "Copia um círculo." },
                { num: "31", item: "Emparelha objetos com a mesma textura." },
                { num: "32", item: "Aponta o 'pequeno' e o 'grande' quando solicitado." },
                { num: "33", item: "Desenha (+) imitando um adulto." },
                { num: "34", item: "Emparelha 3 cores." },
                { num: "35", item: "Coloca objetos dentro, em cima e em baixo de um recipiente, dada a ordem." },
                { num: "36", item: "Nomeia objetos quando ouve o barulho que fazem." },
                { num: "37", item: "Monta um brinquedo de encaixe de 4 peças." },
                { num: "38", item: "Nomeia ações em figuras ('O que ... está fazendo?')." },
                { num: "39", item: "Emparelha forma geométrica com a figura da mesma." },
                { num: "40", item: "Empilha 5 ou mais argolas em uma vara na ordem." }
            ],
            "3 a 4 anos": [
                { num: "41", item: "Nomeia objetos como sendo grandes ou pequenos." },
                { num: "42", item: "Aponta para 10 partes do corpo quando requisitado." },
                { num: "43", item: "Aponta para menino e menina, dada a ordem." },
                { num: "44", item: "Diz se um objeto é pesado ou leve." },
                { num: "45", item: "Une 2 partes de uma figura para formar o todo." },
                { num: "46", item: "Descreve 2 eventos ou personagens de uma estória familiar ou programa de televisão." },
                { num: "47", item: "Repete brincadeiras (rimas ou canções) que envolvam movimentos coordenados." },
                { num: "48", item: "Emparelha 3 ou mais objetos." },
                { num: "49", item: "Aponta para objetos compridos ou curtos." },
                { num: "50", item: "Associa objetos correspondentes. Ex: meia/sapato." },
                { num: "51", item: "Conta até 3 imitando um adulto." },
                { num: "52", item: "Agrupa objetos em categorias." },
                { num: "53", item: "Traça um (V) em imitação." },
                { num: "54", item: "Traça uma linha diagonal dado o exemplo." },
                { num: "55", item: "Conta até 10 objetos, imitando um adulto." },
                { num: "56", item: "Constrói uma ponte com 3 blocos por imitação." },
                { num: "57", item: "Emparelha uma sequência ou padrão (tamanho, cor) de blocos ou contas." },
                { num: "58", item: "Copia uma série de (V) interligados." },
                { num: "59", item: "Acrescenta perna ou braço em um desenho incompleto da figura humana." },
                { num: "60", item: "Completa um quebra-cabeças de 6 peças." },
                { num: "61", item: "Indica se os objetos são iguais ou diferentes." },
                { num: "62", item: "Desenha um quadrado imitando um adulto." },
                { num: "63", item: "Nomeia 3 cores sendo requisitado." },
                { num: "64", item: "Nomeia 3 formas geométricas (quadrado, triângulo e círculo)." }
            ],
            "4 a 5 anos": [
                { num: "65", item: "Apanha de 1 a 5 objetos quando solicitado." },
                { num: "66", item: "Nomeia 5 texturas diferentes." },
                { num: "67", item: "Copia um triângulo ao ser requisitado." },
                { num: "68", item: "Recorda-se de 4 objetos que haviam sido vistos em uma figura." },
                { num: "69", item: "Diz o momento do dia associado a cada atividade." },
                { num: "70", item: "Repete rimas familiares." },
                { num: "71", item: "Diz se um objeto é mais pesado ou mais leve (objetos com diferença de 0,5 quilo)." },
                { num: "72", item: "Diz o que está faltando quando um objeto é retirado de um grupo de 3 objetos." },
                { num: "73", item: "Nomeia 8 cores." },
                { num: "74", item: "Identifica o valor de 3 moedas." },
                { num: "75", item: "Emparelha símbolos (letras e números)." },
                { num: "76", item: "Diz a cor de objetos nomeados." },
                { num: "77", item: "Relata 5 principais fatos de uma história contada 3x." },
                { num: "78", item: "Desenha figura humana (cabeça, tronco e 4 membros)" },
                { num: "79", item: "Canta 5 estrofes de uma canção." },
                { num: "80", item: "Constrói uma pirâmide de 10 blocos por imitação." },
                { num: "81", item: "Nomeia objetos como sendo compridos ou curtos." },
                { num: "82", item: "Coloca objetos 'atrás', 'ao lado' ou 'junto' a outros." },
                { num: "83", item: "Faz conjuntos iguais de 10 objetos, segundo modelo." },
                { num: "84", item: "Nomeia ou aponta para a parte ausente da figura." },
                { num: "85", item: "Conta de 1 a 20." },
                { num: "86", item: "Identifica o objeto que está colocado no meio, em primeiro e em último lugar." }
            ],
            "5 a 6 anos": [
                { num: "87", item: "Conta até 20 objetos e responde adequadamente à pergunta: 'Quantos ... você contou?'" },
                { num: "88", item: "Nomeia 10 numerais." },
                { num: "89", item: "Identifica qual a sua esquerda e qual a sua direita." },
                { num: "90", item: "Diz as vogais em ordem." },
                { num: "91", item: "Escreve seu nome com letras de forma." },
                { num: "92", item: "Nomeia 5 letras do alfabeto." },
                { num: "93", item: "Ordena objetos em sequência de comprimento e largura." },
                { num: "94", item: "Nomeia as letras maiúsculas do alfabeto." },
                { num: "95", item: "Coloca numerais de 1 a 10 na sequência correta." },
                { num: "96", item: "Identifica a posição de objetos em 1º, 2º e 3º lugar." },
                { num: "97", item: "Nomeia as letras minúsculas do alfabeto." },
                { num: "98", item: "Emparelha letras maiúsculas com minúsculas." },
                { num: "99", item: "Aponta para numerais de 1 a 25." },
                { num: "100", item: "Copia um losango." },
                { num: "101", item: "Completa um labirinto simples." },
                { num: "102", item: "Diz os dias da semana na ordem." },
                { num: "103", item: "Soma e subtrai combinações de até 3 elementos." },
                { num: "104", item: "Diz o mês e o dia de seu aniversário." },
                { num: "105", item: "Lê 10 palavras impressas." },
                { num: "106", item: "Prediz o que vai ocorrer." },
                { num: "107", item: "Aponta para objetos inteiros e partidos ao meio." },
                { num: "108", item: "Conta de memória de 1 a 100 (pedir que pare no 40, e continue no 80, caso não erre até o 40)." }
            ]
        },
        "Auto Cuidados": {
            "0 a 1 anos": [
                { num: "01", item: "Suga e deglute líquidos." },
                { num: "02", item: "Toma mingau / sopinha." },
                { num: "03", item: "Estende as mãos em direção a mamadeira, tentando pegá-la." },
                { num: "04", item: "Come alimentos liquidificados dados pelos pais." },
                { num: "05", item: "Segura a mamadeira sem ajuda enquanto bebe." },
                { num: "06", item: "Leva a mamadeira até a boca ou a recusa, empurrando-a." },
                { num: "07", item: "Come alimentos amassados dados pelos pais." },
                { num: "08", item: "Bebe em uma caneca, segurada pelos pais." },
                { num: "09", item: "Come alimentos semissólidos dados pelos pais." },
                { num: "10", item: "Alimenta-se sozinho usando os dedos." },
                { num: "11", item: "Segura a caneca com ambas as mãos e bebe." },
                { num: "12", item: "Leva a colher cheia de comida até a boca com ajuda." },
                { num: "13", item: "Estica braços e pernas ao ser vestido." }
            ],
            "1 a 2 anos": [
                { num: "14", item: "Come com colher de modo independente." },
                { num: "15", item: "Segura a caneca com uma só mão e bebe." },
                { num: "16", item: "Coloca a mão na água e dá tapinhas no rosto com as mãos molhadas, imitando alguém." },
                { num: "17", item: "Senta-se em um piniquinho ou sanitário infantil por 5 min." },
                { num: "18", item: "Coloca um chapéu na cabeça e o remove." },
                { num: "19", item: "Tira as meias." },
                { num: "20", item: "Empurra os braços pelas mangas e os pés pelas pernas da calça." },
                { num: "21", item: "Tira os sapatos quando os cordões estiverem desamarrados" },
                { num: "22", item: "Tira o casaco quando desabotoado." },
                { num: "23", item: "Tira a calça quando desabotoada." },
                { num: "24", item: "Puxa um fecho grande para cima e para baixo." },
                { num: "25", item: "Utiliza palavras ou gestos indicando necessidade de ir ao banheiro." }
            ],
            "2 a 3 anos": [
                { num: "26", item: "Alimenta-se sozinho usando colher ou caneca, derrubando um pouco de comida ou derramando pouco líquido." },
                { num: "27", item: "Quando recebe uma toalha enxuga as mãos e o rosto com ajuda." },
                { num: "28", item: "Suga líquido do copo ou caneca usando canudinho." },
                { num: "29", item: "Dá garfadas." },
                { num: "30", item: "Mastiga e engole apenas substâncias comestíveis." },
                { num: "31", item: "Enxuga as mãos sem ajuda ao lhe darem uma toalha." },
                { num: "32", item: "Avisa que quer ir ao banheiro, mesmo sendo tarde demais." },
                { num: "33", item: "Controla sua baba." },
                { num: "34", item: "Urina ou defeca quando colocado no piniquinho pelo menos 3 vezes por semana." },
                { num: "35", item: "Calça os sapatos." },
                { num: "36", item: "Escova os dentes imitando um adulto." },
                { num: "37", item: "Retira roupas simples que foram desabotoadas." },
                { num: "38", item: "Usa o banheiro para defecar (falha apenas 1x por semana)." },
                { num: "39", item: "Obtém água de uma torneira sem ajuda." },
                { num: "40", item: "Lava as mãos e o rosto com um sabonete." },
                { num: "41", item: "Avisa que quer ir ao banheiro durante o dia a tempo." },
                { num: "42", item: "Pendura o casaco em um gancho da sua altura." },
                { num: "43", item: "Permanece seco ao dormir durante o dia." },
                { num: "44", item: "Evita riscos, por ex: pontas em móveis e escadas sem corrimão." },
                { num: "45", item: "Usa guardanapo quando recomendado." },
                { num: "46", item: "Espeta o garfo na comida, levando-a a boca." },
                { num: "47", item: "Despeja líquido de uma peq. jarra para o copo sem ajuda." },
                { num: "48", item: "Desprende roupas presas com o feixe de pressão." },
                { num: "49", item: "Lava seus braços e pernas ao lhe darem banho." },
                { num: "50", item: "Coloca meias." },
                { num: "51", item: "Veste casaco, malha ou camisa." },
                { num: "52", item: "Identifica a parte dianteira da roupa." }
            ],
            "3 a 4 anos": [
                { num: "53", item: "Alimenta-se sozinho por toda a refeição." },
                { num: "54", item: "Veste-se só, precisando de ajuda apenas quanto há malhas ou camisetas com golas fechadas ou botões e fechos." },
                { num: "55", item: "Enxuga o nariz quando lembrado." },
                { num: "56", item: "Acorda seco 2 manhãs por semana." },
                { num: "57", item: "Se menino, urina no sanitário, em pé." },
                { num: "58", item: "Veste-se e despe-se sozinho, exceto quanto à botões e fechos em 75% das vezes." },
                { num: "59", item: "Fecha a roupa com fechos de pressão ou de gancho." },
                { num: "60", item: "Assoa o nariz quando lembrado." },
                { num: "61", item: "Evita perigos corriqueiros, por ex: caco de vidro." },
                { num: "62", item: "Pendura roupa no cabide e põe no armário quando pedem." },
                { num: "63", item: "Escova os dentes quando recebe instrução." },
                { num: "64", item: "Coloca luvas." },
                { num: "65", item: "Desabotoa botões grandes." },
                { num: "66", item: "Abotoa botões grandes." },
                { num: "67", item: "Calça botas." }
            ],
            "4 a 5 anos": [
                { num: "68", item: "Limpa o que derramou por conta própria." },
                { num: "69", item: "Evita veneno e todas as substâncias prejudiciais." },
                { num: "70", item: "Desabotoa sua roupa." },
                { num: "71", item: "Abotoa sua roupa." },
                { num: "72", item: "Retira prato e talheres da mesa." },
                { num: "73", item: "Encaixa fecho em sua terminação." },
                { num: "74", item: "Lava as mãos e o rosto." },
                { num: "75", item: "Usa talher apropriado para alimentar-se." },
                { num: "76", item: "Acorda de noite para ir ao banheiro, ou acorda seco." },
                { num: "77", item: "Limpa e assua o nariz em 75% das vezes sem ser lembrado" },
                { num: "78", item: "Toma banho só, precisando de ajuda apenas para lavar as costas, pescoço e orelhas." },
                { num: "79", item: "Usa faca para espalhar manteiga no pão." },
                { num: "80", item: "Aperta e afrouxa cintos ou fivelas." },
                { num: "81", item: "Veste-se sozinho, mas não dá laços." },
                { num: "82", item: "Serve-se à mesa enquanto seguram a travessa de comida." },
                { num: "83", item: "Ajuda a pôr a mesa corretamente quando recebe instruções." },
                { num: "84", item: "Escova os dentes." },
                { num: "85", item: "Vai ao banheiro a tempo, retira a roupa, usa papel higiênico, dá descarga e veste-se sem ajuda." },
                { num: "86", item: "Penteia ou escova cabelos." },
                { num: "87", item: "Pendura roupas em cabides." },
                { num: "88", item: "Anda pela vizinhança sem constante supervisão." },
                { num: "89", item: "Enfia cordões em sapatos." },
                { num: "90", item: "Amarra ou dá laços nos cordões dos sapatos." }
            ],
            "5 a 6 anos": [
                { num: "91", item: "É responsável por uma tarefa semanal e a executa ao ser lembrado." },
                { num: "92", item: "Seleciona roupas apropriadas ao clima e ocasião." },
                { num: "93", item: "Pára no passeio, olha para ambos os lados, e atravessa a rua sem precisar ser lembrado." },
                { num: "94", item: "Serve-se à mesa e passa aos demais a panela de comida." },
                { num: "95", item: "Prepara sua própria caneca de café com leite." },
                { num: "96", item: "É responsável por uma tarefa diária em casa." },
                { num: "97", item: "Ajusta a temperatura da água para o banho." },
                { num: "98", item: "Prepara seu próprio lanche." },
                { num: "99", item: "Anda sozinho até a distância de 2 quadras de casa." },
                { num: "100", item: "Corta alimentos tenros com faca." },
                { num: "101", item: "Encontra o banheiro em local público, corretamente." },
                { num: "102", item: "Abre a embalagem de leite." },
                { num: "103", item: "Apanha uma bandeja com comida, levando-a e pondo sobre a mesa." },
                { num: "104", item: "Amarra os cordões em casacos com capuz." },
                { num: "105", item: "Aperta o cinto de segurança do automóvel." }
            ]
        },
        "Desenvolvimento Motor": {
            "0 a 1 anos": [
                { num: "01", item: "Alcança um objeto colocado à sua frente (15 a 20 cm.)." },
                { num: "02", item: "Apanha um objeto colocado à sua frente (8 cm.)." },
                { num: "03", item: "Estende os braços em direção a um objeto à sua frente e o apanha." },
                { num: "04", item: "Alcança um objeto preferido." },
                { num: "05", item: "Coloca objetos na boca." },
                { num: "06", item: "Eleva a cabeça e o tronco apoiando-se nos braços, ao estar deitado de barriga para baixo." },
                { num: "07", item: "Levanta a cabeça e o tronco apoiando-se em um só braço." },
                { num: "08", item: "Toca e explora objetos com a boca." },
                { num: "09", item: "Em DV (decúbito ventral, de bruços), vira de lado e mantém esta posição 1/2 das vezes." },
                { num: "10", item: "Em DV, vira de costas." },
                { num: "11", item: "Em DV, move-se para frente o equivalente à sua altura." },
                { num: "12", item: "Em DD (decúbito dorsal), rola para o lado." },
                { num: "13", item: "Em DD, vira de barriga para baixo." },
                { num: "14", item: "Faz esforço para sentar-se, segurando nos dedos do adulto." },
                { num: "15", item: "Vira a cabeça com facilidade quando o corpo está apoiado." },
                { num: "16", item: "Mantém-se sentado por 2 minutos." },
                { num: "17", item: "Solta um objeto para apanhar outro." },
                { num: "18", item: "Apanha e deixa cair um objeto propositalmente." },
                { num: "19", item: "Fica em pé com o máximo de apoio." },
                { num: "20", item: "Estando em pé com apoio, pula para cima e para baixo." },
                { num: "21", item: "Engatinha para apanhar um objeto (distante a sua altura)." },
                { num: "22", item: "Senta-se apoiando-se sozinho." },
                { num: "23", item: "Estando sentado, vira de gatinhas." },
                { num: "24", item: "Estando em DV consegue sentar-se." },
                { num: "25", item: "Senta-se sem o apoio das mãos." },
                { num: "26", item: "Atira objetos ao acaso." },
                { num: "27", item: "Balança para frente e para trás quando de gatinhas." },
                { num: "28", item: "Transfere objetos de uma mão para outra quando sentado." },
                { num: "29", item: "Retém em uma das mãos 2 cubos de 2,5 cm." },
                { num: "30", item: "Fica de joelhos." },
                { num: "31", item: "Fica em pé, apoiando-se em algo." },
                { num: "32", item: "Usa preensão de pinça para pegar objetos." },
                { num: "33", item: "Engatinha." },
                { num: "34", item: "Estando de gatinhas, estende uma das mãos para o alto." },
                { num: "35", item: "Fica em pé com o mínimo de apoio." },
                { num: "36", item: "Lambe a comida ao redor da boca." },
                { num: "37", item: "Mantém-se em pé sozinho por um minuto." },
                { num: "38", item: "Derruba um objeto que está dentro de um recipiente." },
                { num: "39", item: "Vira várias páginas de um livro ao mesmo tempo." },
                { num: "40", item: "Escava com uma colher ou pá." },
                { num: "41", item: "Coloca pequenos objetos dentro do recipiente." },
                { num: "42", item: "Estando de pé, abaixa-se e senta." },
                { num: "43", item: "Bate palmas." },
                { num: "44", item: "Anda com um mínimo de apoio." },
                { num: "45", item: "Dá alguns passos sem apoio." }
            ],
            "1 a 2 anos": [
                { num: "46", item: "Sobe escadas engatinhando." },
                { num: "47", item: "Coloca-se em pé, estando sentado." },
                { num: "48", item: "Rola uma bola imitando um adulto." },
                { num: "49", item: "Sobe em uma cadeira de adulto, vira-se e senta." },
                { num: "50", item: "Coloca 4 aros em uma pequena estaca." },
                { num: "51", item: "Retira pinos de 2,5 cm de uma prancha ou tabuleiro." },
                { num: "52", item: "Encaixa pinos de 2,5 cm em uma prancha de encaixe." },
                { num: "53", item: "Constrói uma torre de 3 blocos." },
                { num: "54", item: "Faz traços no papel com lápis ou lápis de cera." },
                { num: "55", item: "Anda sozinho." },
                { num: "56", item: "Desce escadas sentado, colocando primeiro os pés." },
                { num: "57", item: "Senta-se em uma cadeirinha." },
                { num: "58", item: "Agacha-se e volta a ficar em pé." },
                { num: "59", item: "Empurra e puxa brinquedos ao andar." },
                { num: "60", item: "Usa cadeira ou cavalo de balanço." },
                { num: "61", item: "Sobe escadas com ajuda." },
                { num: "62", item: "Dobra o corpo sem cair para apanhar objetos no chão." },
                { num: "63", item: "Imita um movimento circular." }
            ],
            "2 a 3 anos": [
                { num: "64", item: "Enfia 4 contas grandes em um cordão em 2 minutos." },
                { num: "65", item: "Vira trincos ou maçanetas em portas." },
                { num: "66", item: "Salta no mesmo local com ambos os pés." },
                { num: "67", item: "Anda de costas." },
                { num: "68", item: "Desce escadas sem ajuda." },
                { num: "69", item: "Atira uma bola a um adulto à 1 ½ de distância." },
                { num: "70", item: "Constrói uma torre de 5 a 6 blocos." },
                { num: "71", item: "Vira páginas de um livro, uma por vez." },
                { num: "72", item: "Desembrulha um pequeno objeto." },
                { num: "73", item: "Dobrar um papel ao meio, imitando um adulto." },
                { num: "74", item: "Desmancha e reconstrói brinquedos de encaixe por pressão." },
                { num: "75", item: "Desenrosca brinquedos que se encaixam por roscas." },
                { num: "76", item: "Chuta uma bola grande que está imóvel." },
                { num: "77", item: "Faz bolas de argila, barro ou massinha." },
                { num: "78", item: "Segura o lápis entre o polegar e o indicador, apoiando-o sobre o dedo médio." },
                { num: "79", item: "Dá cambalhota para frente com ajuda." },
                { num: "80", item: "Dá marteladas para encaixar 5 pinos em seus orifícios." }
            ],
            "3 a 4 anos": [
                { num: "81", item: "Faz um quebra cabeça de 3 peças." },
                { num: "82", item: "Corta algo em pedaços com tesoura." },
                { num: "83", item: "Pula de uma altura de 20 cm." },
                { num: "84", item: "Chuta uma bola grande quando enviada para si." },
                { num: "85", item: "Anda na ponta dos pés." },
                { num: "86", item: "Corre 10 passos coordenando e alternando o movimento dos braços e pés." },
                { num: "87", item: "Pedala com triciclo a distância de 1 metro e ½." },
                { num: "88", item: "Balança em um balanço quando este está em movimento." },
                { num: "89", item: "Sobe em um escorregador de 1,20m a 1,80m e escorrega." },
                { num: "90", item: "Dá cambalhotas para frente." },
                { num: "91", item: "Sobe escadas alternando os pés." },
                { num: "92", item: "Marcha (anda de forma ritmada)." },
                { num: "93", item: "Apara a bola com ambas as mãos." },
                { num: "94", item: "Desenha figuras seguindo contornos ou pontilhados." },
                { num: "95", item: "Recorta ao longo de uma linha reta 20 cm, afastando-se pouco da linha." }
            ],
            "4 a 5 anos": [
                { num: "96", item: "Fica em um só pé sem apoio por 4 a 8 segundos." },
                { num: "97", item: "Muda de direção ao correr." },
                { num: "98", item: "Anda sobre uma viga ou tábua, mantendo o equilíbrio." },
                { num: "99", item: "Pula para frente 10 vezes sem cair." },
                { num: "100", item: "Salta sobre uma corda suspensa a 5 cm do solo." },
                { num: "101", item: "Pula de costas 6 vezes." },
                { num: "102", item: "Rebate e apanha uma bola grande." },
                { num: "103", item: "Une 2 a 3 pedaços de massa de modelar." },
                { num: "104", item: "Recorta em torno de linhas curvas." },
                { num: "105", item: "Encaixa objetos de rosca." },
                { num: "106", item: "Desce escadas alternando os pés." },
                { num: "107", item: "Pedala um triciclo fazendo curvas." },
                { num: "108", item: "Salta em um só pé 5 vezes consecutivas." },
                { num: "109", item: "Recorta um círculo em 5 cm." },
                { num: "110", item: "Desenha figuras simples facilmente identificáveis (por ex: casa)." },
                { num: "111", item: "Recorta e cola formas simples." }
            ],
            "5 a 6 anos": [
                { num: "112", item: "Escreve letras de imprensa maiúsculas, isoladas e grandes em qualquer lugar do papel." },
                { num: "113", item: "Anda sobre uma tábua para trás, para frente e para os lados, mantendo o equilíbrio." },
                { num: "114", item: "Caminha saltitando." },
                { num: "115", item: "Balança em um balanço iniciando e mantendo o movimento." },
                { num: "116", item: "Estica os dedos tocando o polegar em cada um deles." },
                { num: "117", item: "Copia letras maiúsculas." },
                { num: "118", item: "Sobe em escadas de mão ou de escorregador de 3 m." },
                { num: "119", item: "Bate em um prego com martelo." },
                { num: "120", item: "Rebate a bola à medida que anda com direção." },
                { num: "121", item: "Consegue colorir sem sair da margem em 95% das vezes." },
                { num: "122", item: "Recorta figuras sem sair mais que 6 mm da margem." },
                { num: "123", item: "Usa apontador de lápis." },
                { num: "124", item: "Copia desenhos complexos (escola, navio)." },
                { num: "125", item: "Rasga figuras simples de um papel." },
                { num: "126", item: "Dobrar um papel quadrado 2x em diagonal por imitação." },
                { num: "127", item: "Apanha uma bola leve com uma só mão." },
                { num: "128", item: "Pula corda sozinho." },
                { num: "129", item: "Golpeia uma bola com um bastão ou pedaço de pau." },
                { num: "130", item: "Apanha um objeto no chão enquanto corre." },
                { num: "131", item: "Patina uma distância de 3 m, ou usa skate." },
                { num: "132", item: "Anda de bicicleta." },
                { num: "133", item: "Escorrega descendo um monte de areia ou terra." },
                { num: "134", item: "Anda ou brinca em piscina tendo água até a cintura." },
                { num: "135", item: "Conduz um patinete dando impulso com um só pé." },
                { num: "136", item: "Salta e gira em um só pé." },
                { num: "137", item: "Escreve seu nome com letras de forma em caderno pautado." },
                { num: "138", item: "Salta de uma altura de 30 cm e cai na ponta dos pés." },
                { num: "139", item: "Pára em um só pé sem apoio com olhos fechados por 10 segundos." },
                { num: "140", item: "Dependura-se por 10 segundos em uma barra horizontal." }
            ]
        }
    };

    function generateScaleHTML(scaleName, scaleData) {
        let html = `
            <section>
                <h2>II. Escalas de Desenvolvimento: ${scaleName}</h2>
                <table>
                    <thead>
                        <tr>
                            <th>N.º</th>
                            <th>Verificar se:</th>
                            <th class="result-cell">Resultado (S / N / AV)</th>
                        </tr>
                    </thead>
                    <tbody>
        `;

        for (const ageRange in scaleData) {
            html += `
                <tr>
                    <td colspan="3" class="age-range-header">${scaleName} — ${ageRange}</td>
                </tr>
            `;
            scaleData[ageRange].forEach(item => {
                // Cria um nome único para o grupo de botões de rádio (ex: Socializacao-01)
                const uniqueName = `${scaleName.replace(/\s/g, '')}-${item.num}`;
                html += `
                    <tr>
                        <td>${item.num}</td>
                        <td>${item.item}</td>
                        <td class="result-cell">
                            <label><input type="radio" name="${uniqueName}" value="S"> S</label>
                            <label><input type="radio" name="${uniqueName}" value="N"> N</label>
                            <label><input type="radio" name="${uniqueName}" value="AV"> AV</label>
                        </td>
                    </tr>
                `;
            });
        }

        html += `
                    </tbody>
                </table>
            </section>
        `;
        return html;
    }

    document.addEventListener('DOMContentLoaded', () => {
        const scalesContainer = document.getElementById('scales-container');
        let allScalesHTML = '';
        for (const scaleName in escalas) {
            allScalesHTML += generateScaleHTML(scaleName, escalas[scaleName]);
        }
        scalesContainer.innerHTML = allScalesHTML;
    });
</script>

</body>
</html>
