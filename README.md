<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Atividade Avaliativa - Química Orgânica</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #121212; /* Fundo geral escuro */
            color: #ffffff;
            margin: 0;
            padding: 0;
        }
        .form-container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background-color: #1e1e1e; /* Fundo do contêiner principal */
            border-radius: 10px;
        }
        .header, .school-header {
            text-align: center;
        }
        .school-header h2 {
            margin: 0;
            color: #FFD700;
        }
        .header h1 {
            color: #ffffff;
        }
        .cabecalho {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 15px;
        }
        /* Estilização dos campos de seleção, data e textarea */
        select, input[type="date"], textarea {
            width: 100%;
            padding: 8px 10px; /* Reduzido o padding para tornar mais compacto */
            border-radius: 5px;
            border: 1px solid #ccc; /* Borda cinza clara */
            background-color: #ffffff; /* Fundo branco */
            color: #000000; /* Texto preto */
            box-sizing: border-box;
            font-size: 14px; /* Reduzido o tamanho da fonte */
        }
        /* Estilização específica para o select de nomes */
        #nome {
            appearance: none; /* Remove a seta padrão */
            background-image: url('data:image/svg+xml;charset=US-ASCII,<svg xmlns="http://www.w3.org/2000/svg" width="10" height="7" viewBox="0 0 10 7"><path fill="%23000000" d="M0 0l5 5 5-5H0z"/></svg>');
            background-repeat: no-repeat;
            background-position: right 10px center;
            background-size: 10px 7px;
            padding-right: 30px; /* Espaço para a seta personalizada */
            cursor: pointer;
        }
        /* Estilização para manter a aparência do select */
        select:focus {
            outline: none;
            border-color: #4CAF50;
            box-shadow: 0 0 5px rgba(76, 175, 80, 0.5);
        }
        /* Estilização do botão de envio */
        .submit-button {
            margin: 30px auto;
            display: block;
            width: 200px;
            background-color: #4CAF50;
            color: #ffffff;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            box-shadow: 0 5px #999; /* Efeito 3D */
            transition: all 0.2s;
        }
        .submit-button:active {
            box-shadow: 0 2px #666; /* Efeito de depressão */
            transform: translateY(4px); /* Desloca para baixo */
        }
        .feedback-container {
            display: none;
            margin-top: 20px;
            background-color: #fff;
            color: #333;
            padding: 20px;
            border-radius: 8px;
        }

        /* Estilização das questões */
        .questoes-container > div {
            margin-bottom: 30px; /* Espaçamento de 30px entre cada questão */
        }

        .questoes-container label {
            display: block;
            line-height: 1.6; /* Aumento do espaçamento entre linhas */
            background-color: #2f4f4f; /* Fundo cinza escuro */
            padding: 10px;
            border-radius: 5px;
            color: #ffffff; /* Texto branco */
            margin-bottom: 10px; /* Espaçamento entre o enunciado e a textarea */
            box-shadow: 3px 3px 5px rgba(0, 0, 0, 0.5); /* Efeito de borda 3D */
        }

        /* Ajuste nas textareas para melhor contraste */
        .questoes-container textarea {
            background-color: #ffffff; /* Fundo branco conforme solicitado */
            color: #000000; /* Texto preto */
            border: 1px solid #ccc; /* Borda */
        }

        /* Responsividade para telas menores */
        @media (max-width: 768px) {
            .cabecalho {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <div class="form-container">
        <div class="school-header">
            <h2>E.E. MARIA LEONI</h2>
        </div>
        <div class="header">
            <h1>Atividade Avaliativa - Química Orgânica</h1>
        </div>

        <form id="formulario">
            <div class="cabecalho">
                <div>
                    <label for="nome">Nome:</label>
                    <select id="nome" name="nome" required>
                        <option value="" disabled selected>Selecione seu nome</option>
                        <!-- Lista completa de nomes dos alunos -->
                        <option>ANA BEATRIZ DE BRITTO CERQUEIRA</option>
                        <option>BRUNA FREITAS DA SILVA</option>
                        <option>CAIO EDUARDO SILVA DE MORAES</option>
                        <option>CAUE CAPDEVILA KLEIN</option>
                        <option>DAFNE COSTA SANTANA</option>
                        <option>DANIEL GONCALVES MOLINA</option>
                        <option>ERICK THOMAS CONSOLO VALOSSI</option>
                        <option>GABRIEL FONSECA DA SILVA</option>
                        <option>GIOVANNA DOS SANTOS PONTES</option>
                        <option>GIOVANNA REGINA PEREIRA MACHADO</option>
                        <option>GUSTAVO HENRIQUE PEREIRA</option>
                        <option>ISABELA DE ARAUJO ANTONIO</option>
                        <option>ISABELLEY DE PAULA NASCIMENTO</option>
                        <option>JOAO VICTOR LIMA DE SOUSA</option>
                        <option>JONAS ELIAQUIM CARVALHO BIELLA</option>
                        <option>JULIA CRISTINI ASSUNCAO DA SILVA</option>
                        <option>KAUAN COSTA DOS SANTOS</option>
                        <option>LETICIA BORGES DE CASTRO</option>
                        <option>MARCELA ALCANTARA DA SILVA</option>
                        <option>MATHEUS ESTEVAM AGUIAR</option>
                        <option>MICHAEL PETTER SOARES DE SOUSA</option>
                        <option>MIGUEL VENANCIO DE BRITO</option>
                        <option>MIRIA NOBERTO DOS SANTOS</option>
                        <option>NICOLAS EMANUEL DE OLIVEIRA VILAR</option>
                        <option>PEDRO HENRIQUE BESSA DOS SANTOS</option>
                        <option>YAGO PEIXOTO RODRIGUES ORTEGA</option>
                        <option>LEANDRO HIROYUKI ROCHA TAGUTI</option>
                        <option>WESDLEY SENA PAULO JUNIOR</option>
                        <option>GUILHERME LUCAS FONTOLAN DOS SANTOS</option>
                        <option>JOAO VICTOR PAULINO DOS SANTOS</option>
                        <option>ANDRE SILVA BRAGA GONCALVES</option>
                        <option>QUEZIA ZAINE ALVES DA SILVA RAMOS</option>
                        <option>FLAVIA PALMA SOUZA</option>
                        <option>VITOR RODRIGUES DOS SANTOS ALVES</option>
                        <option>MARIA EDUARDA RODRIGUES VILLELA DA SILVA</option>
                        <option>ARTHUR FERNANDO DA SILVA MAIRINK</option>
                        <option>CARLOS HENRIQUE SILVA SOUSA</option>
                        <option>CRISTIAN FERNANDO DA SILVA</option>
                        <option>DANIEL BARBOSA CORREIA</option>
                        <option>GABRIEL ALMEIDA DA SILVA</option>
                        <option>JHENNIFER GOMES FRANCO</option>
                        <option>JOAO GABRIEL SANTOS ESTEVES</option>
                        <option>JOAO VICTOR BITO DOS SANTOS</option>
                        <option>JOSE HENRIQUE BARCELLOS DA SILVA</option>
                        <option>JULIA SILVA MAGALHAES</option>
                        <option>KAIO HENRIQUE CONCEICAO SILVA</option>
                        <option>KAIQUE DERICK MENDES DE CARVALHO</option>
                        <option>LECIVAN ALEXANDRE MENEZES DA SILVA</option>
                        <option>LUCAS MONTERO DE OLIVEIRA</option>
                        <option>LUCAS OLIVEIRA DE SOUZA</option>
                        <option>MAISHA MIKI ROCHA PEDRICO</option>
                        <option>MARIANA DA SILVA AZARIAS CANDIDO</option>
                        <option>MARINA ELAILIA DOS SANTOS BEZERRA</option>
                        <option>MATHEUS EDUARDO DOS SANTOS</option>
                        <option>NICOLLY SURIEL SANTOS</option>
                        <option>RAFAELA ROCHA VIEIRA</option>
                        <option>RAQUEL DE OLIVEIRA CARVALHO</option>
                        <option>SOPHIA RODRIGUES AMORIM</option>
                        <option>VICTOR EDUARDO OLIVEIRA DE ALMEIDA CARDOSO</option>
                        <option>VINÍCIUS MONTEIRO DAS NEVES</option>
                        <option>VITOR HUGO AMORIM PEREIRA</option>
                        <option>YAGO MARTINS REBECHI</option>
                        <option>YURI SILVA FIRMINO</option>
                        <option>SARA QUERINO DE OLIVEIRA</option>
                        <option>ELOIZA ALEXANDRE DOS SANTOS RODRIGUES</option>
                        <option>LARYSSA MARTINS DE SOUZA</option>
                        <option>EMILLY CRISTINA CARNEIRO</option>
                        <option>GABRIEL FERNANDES SILVEIRA</option>
                        <option>SAMUEL VINICIUS DOS SANTOS SILVA</option>
                        <option>ELISÂNGELA LUCIANO DA SILVA</option>
                        <option>MIQUEIAS CRUZ DOS SANTOS</option>
                        <option>EMANUEL VIEIRA DOS SANTOS</option>
                        <option>ALICE CRUZ BATISTA</option>
                        <option>ARTHUR RODRIGUES WRONSKI</option>
                        <option>MARIA EDUARDA DOMICIANO GOMES</option>
                        <option>ANA CAROLINA DE CASSIA CAVALCANTE</option>
                        <option>ANA MUCELIN BORGES PINHEIRO</option>
                        <option>ARIEL CARLOS AGUIAR DA SILVA</option>
                        <option>ARTHUR ALVES BRITO DA COSTA</option>
                        <option>BRUNO CESAR PEREIRA NETO BOSCATO</option>
                        <option>CRISTIANE FERNANDA DA SILVA</option>
                        <option>DANDARA SANTOS</option>
                        <option>DAYANE DOS SANTOS PEDROSO</option>
                        <option>DIEGO CARVALHO SANTOS</option>
                        <option>GABRIEL ROMERO SANTOS</option>
                        <option>GAEL RIQUELME FERREIRA</option>
                        <option>GUILHERME SILVA SARLO COSTA</option>
                        <option>GUSTAVO DE SOUZA FRANCA</option>
                        <option>GUSTAVO FRIAS DE OLIVEIRA TAVARES</option>
                        <option>ISABELLI FONSECA DA SILVA</option>
                        <option>ISABELLI MIRANDA NARVAES</option>
                        <option>JHONY PETTER MARQUES LUDWIG ROTH GRACIANO</option>
                        <option>JOAO VICTOR DE FRANCA SOARES</option>
                        <option>JOAQUIM HENRIQUE SANTOS AMORIM</option>
                        <option>KAUE LUCKA DA SILVA FACIOLI</option>
                        <option>LORENA GALVAN CESPEDES</option>
                        <option>LORRANY LIMA GONCALVES</option>
                        <option>LUCIA OLIVEIRA SOUTO</option>
                        <option>MURILO GABRIEL GOMES DA SILVA ALVES</option>
                        <option>NOEL CHRISTE PEREIRA NETO</option>
                        <option>REBEKA CAMILLY SILVA XAVIER</option>
                        <option>YASMIN LORENÇATO REBEQUI</option>
                        <option>YNGRID VERISSIMO WILCHES</option>
                        <option>ERIK GONELLI GARCIA</option>
                        <option>RAYSSA MANTA MULLER</option>
                        <option>NYCOLE GIMENES SILVA</option>
                        <option>OLÍVIA FERREIRA CANDIDO</option>
                        <option>MARIA EDUARDA RODRIGUES BARBOSA</option>
                        <option>IGOR SILVEIRA FERNANDES</option>
                        <option>LUISA CARVALHAES LARA</option>
                        <option>GUSTAVO CAMPOS DE OLIVEIRA</option>
                        <option>DAVI DE JESUS CARVALHO LIMA</option>
                        <option>TAYNA DE OLIVEIRA</option>
                        <option>EDUARDA GOMES BALTAZAR</option>
                        <option>FERNANDO DE SOUSA</option>
                        <option>MABILI CRISTINA LIMA DE CASTRO</option>
                        <option>PIETRO MOREIRA COMUNIAN</option>
                        <option>ANA CAROLINA DA SILVA RODRIGUES</option>
                        <option>CAMILA ANDRADE VENANCIO</option>
                        <option>DEBORAH VICTORIA PRADO DA CRUZ</option>
                        <option>EMILY CAROLINE RODRIGUES LIMA</option>
                        <option>EMILY SUENAGA ARAI</option>
                        <option>EVANDRO RAMOS GONCALVES</option>
                        <option>FELIPE BENÍCIO DOS SANTOS</option>
                        <option>GABRIEL VERONEZE BRITO</option>
                        <option>GABRIELLA LOPES NASCIMENTO</option>
                        <option>GABRIELLE FERNANDES SAMPAIO</option>
                        <option>ISADORA FLORES DE ALMEIDA</option>
                        <option>JULIA DOS SANTOS SILVA</option>
                        <option>JULIA LEANDRO DA SILVA ALMEIDA</option>
                        <option>JULIA NERIS COSTA DE JESUS</option>
                        <option>LAURA FEREZIN CHAVES</option>
                        <option>MARCOS VINICIUS MATOS OLIVEIRA</option>
                        <option>MATEUS DIAS NEVES</option>
                        <option>NICHOLAS ALMEIDA COSTA</option>
                        <option>NICOLE EDUARDA DE LIMA GAIA</option>
                        <option>VITORIA CRISTINA PEREIRA</option>
                        <option>ANA LIVIA DE LIMA ABEL</option>
                        <option>LUCAS SALES CARNEIRO</option>
                    </select>
                </div>

                <div>
                    <label for="serie">Série:</label>
                    <select id="serie" name="serie" required>
                        <option value="" disabled selected>Selecione a série</option>
                        <option>2ªSÉRIE A</option>
                        <option>2ªSÉRIE B</option>
                        <option>2ªSÉRIE C</option>
                        <option>2ºTÉCNICO</option> <!-- Nova opção adicionada -->
                    </select>
                </div>

                <div>
                    <label for="data">Data:</label>
                    <input type="date" id="data" name="data" required>
                </div>
            </div>

            <div class="questoes-container">
                <div>
                    <label for="resposta1">1. Imagine que você vai ao supermercado e encontra produtos como alimentos, produtos de limpeza e cosméticos. Muitos deles são feitos com compostos orgânicos. Com base no que você sabe, como a química orgânica está presente nesses produtos? De que maneira isso influencia nossas escolhas de consumo no dia a dia?</label>
                    <textarea id="resposta1" name="resposta1" required></textarea>
                </div>

                <div>
                    <label for="resposta2">2. Em diversas culturas, alimentos fermentados, como pães e iogurtes, fazem parte da dieta tradicional. Pense no impacto social e econômico desses produtos na vida moderna. Por que você acredita que a fermentação continua sendo importante hoje, mesmo com tantas tecnologias industriais disponíveis?</label>
                    <textarea id="resposta2" name="resposta2" required></textarea>
                </div>

                <div>
                    <label for="resposta3">3. Com as mudanças climáticas, há uma busca por substituir combustíveis fósseis por biocombustíveis. Analise os benefícios e desafios de adotar biocombustíveis em larga escala. O que poderia incentivar ou dificultar essa mudança no Brasil e no mundo?</label>
                    <textarea id="resposta3" name="resposta3" required></textarea>
                </div>

                <div>
                    <label for="resposta4">4. Substâncias orgânicas, como a ocitocina, influenciam nosso humor e relacionamentos. Pense em como momentos simples, como abraçar alguém ou conviver com amigos, podem ser explicados também pela química. Como você acredita que o conhecimento sobre esses processos pode ser útil para a saúde emocional das pessoas?</label>
                    <textarea id="resposta4" name="resposta4" required></textarea>
                </div>

                <div>
                    <label for="resposta5">5. Muitos tecidos usados na moda, como o poliéster, são produzidos a partir de compostos orgânicos derivados do petróleo. Sabendo que esses materiais demoram anos para se decompor, como você avalia a busca por materiais sustentáveis na moda? O que mais poderia ser feito para reduzir o impacto ambiental da indústria têxtil?</label>
                    <textarea id="resposta5" name="resposta5" required></textarea>
                </div>

                <div>
                    <label for="resposta6">6. A química é usada na fabricação de eletrônicos, como celulares e laptops, mas também causa resíduos prejudiciais ao meio ambiente. Como você avalia o desafio de equilibrar o avanço tecnológico com a preservação ambiental? O que a sociedade e as indústrias poderiam fazer para diminuir o impacto dos resíduos eletrônicos?</label>
                    <textarea id="resposta6" name="resposta6" required></textarea>
                </div>

                <div>
                    <label for="resposta7">7. A ciência foi fundamental na criação das vacinas contra a COVID-19, mas a desinformação gerou hesitação na vacinação. A confiança pode ser construída com campanhas educativas, maior transparência e envolvimento da comunidade científica para aproximar as pessoas da ciência e dos benefícios da vacinação.</label>
                    <textarea id="resposta7" name="resposta7" required></textarea>
                </div>

                <div>
                    <label for="resposta8">8. As reações químicas nos alimentos explicam mudanças de sabor, cor e textura, como o escurecimento do pão (reação de Maillard). Compreender esses processos ajuda a melhorar a qualidade da alimentação e permite o desenvolvimento de novos produtos, como alimentos mais saudáveis e funcionais.</label>
                    <textarea id="resposta8" name="resposta8" required></textarea>
                </div>

                <div>
                    <label for="resposta9">9. A preferência por produtos naturais está ligada à percepção de que são mais seguros e sustentáveis. No entanto, nem todos os produtos naturais são necessariamente melhores ou livres de riscos. A escolha entre produtos naturais e sintéticos deve considerar sua eficácia, segurança e impacto ambiental.</label>
                    <textarea id="resposta9" name="resposta9" required></textarea>
                </div>

                <div>
                    <label for="resposta10">10. A química pode desenvolver alternativas mais sustentáveis, como plásticos biodegradáveis e produtos reutilizáveis. Como consumidores, podemos adotar práticas como a redução do uso de plástico, a escolha por produtos reciclados e o apoio a empresas que investem em inovação sustentável.</label>
                    <textarea id="resposta10" name="resposta10" required></textarea>
                </div>
            </div>

            <button type="submit" class="submit-button">Enviar Respostas</button>
        </form>

        <div id="feedback-container" class="feedback-container">
            <h2>Feedback da Autocorreção</h2>
            <div id="feedback-content"></div>
        </div>
    </div>

    <script>
        const gabarito = [
            "Os microplásticos podem acumular-se nos organismos...",
            "A produção de CO₂ e CH₄ provém de processos...",
            "Fertilizantes orgânicos minimizam a eutrofização...",
            "COVs contribuem para doenças respiratórias...",
            "Hidrogênio verde é produzido por eletrólise...",
            "A química permite sintetizar aditivos alimentares...",
            "Bioplásticos são fabricados a partir de amido...",
            "Resíduos de medicamentos poluem águas...",
            "A reciclagem química decompõe polímeros...",
            "Nanomateriais oferecem vantagens, mas riscos..."
        ];

        document.getElementById('formulario').addEventListener('submit', async (event) => {
            event.preventDefault();
            const respostas = [];
            const feedbacks = [];

            for (let i = 1; i <= 10; i++) {
                const resposta = document.getElementById(`resposta${i}`).value.trim();
                respostas.push(resposta);
                const correto = gabarito[i - 1].toLowerCase().includes(resposta.toLowerCase());
                feedbacks.push(correto ? 'Correto' : 'Incorreto');
            }

            // Cria um objeto com os dados a serem enviados
            const data = {
                nome: document.getElementById('nome').value,
                serie: document.getElementById('serie').value,
                data: document.getElementById('data').value,
            };

            // Adiciona as respostas e feedbacks ao objeto
            for (let i = 1; i <= 10; i++) {
                data[`resposta${i}`] = respostas[i - 1];
                data[`feedback${i}`] = feedbacks[i - 1];
            }

            try {
                const response = await fetch('https://script.google.com/macros/s/AKfycbx0VIGN8CGX1fxA9pomL4PdlasExBq-W5K-ZwrKw-jj1ID1ykcReEgtED4V9LwvW6U/exec', { // Substitua pela URL do Web App
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json',
                    },
                    body: JSON.stringify(data),
                });

                const result = await response.json();

                if (result.result === 'success') {
                    // Exibe o feedback no formulário
                    let feedback = '';
                    feedbacks.forEach((fb, index) => {
                        feedback += `<p><strong>Questão ${index + 1}:</strong> ${fb}</p>`;
                    });

                    document.getElementById('feedback-content').innerHTML = feedback;
                    document.getElementById('feedback-container').style.display = 'block';

                    // Opcional: Limpar o formulário após o envio
                    document.getElementById('formulario').reset();
                    // Resetar a seta personalizada do select de nomes
                    document.getElementById('nome').selectedIndex = 0;
                } else {
                    alert('Erro ao enviar os dados: ' + result.error);
                }
            } catch (error) {
                alert('Erro ao enviar os dados: ' + error);
            }
        });
    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Atividade Avaliativa - Química Orgânica</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #121212; /* Fundo geral escuro */
            color: #ffffff;
            margin: 0;
            padding: 0;
        }
