<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agrinho 2026 - Agricultura de Precisão</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="container">
            <!-- Tema principal do Concurso Agrinho 2026 -->
            <p class="tagline">Concurso Agrinho 2026</p>
            <h1>Agro forte, futuro sustentável: equilíbrio entre produção e meio ambiente</h1>
        </div>
    </header>

    <main class="container">
        
        <!-- Introdução ao Assunto Escolhido -->
        <section id="introducao" class="card">
            <h2>O que é Agricultura de Precisão?</h2>
            <p>A agricultura de precisão é um sistema de gestão agrícola que utiliza tecnologias avançadas — como GPS, sensores, drones e inteligência artificial — para observar, medir e responder à variabilidade das lavouras. Em vez de tratar o campo inteiro de forma igual, cada pedaço da terra recebe exatamente o que precisa.</p>
        </section>

        <!-- O Problema -->
        <section id="problema" class="card">
            <h2>O Problema: O Desperdício Tradicional</h2>
            <p>Na agricultura convencional, a aplicação de fertilizantes, defensivos agrícolas e água é feita de maneira uniforme por toda a plantação. Isso gera dois grandes problemas: o desperdício financeiro para o produtor e a sobrecarga do solo. O excesso de produtos químicos é lavado pela chuva, poluindo rios, lençóis freáticos e prejudicando a biodiversidade local.</p>
        </section>

        <!-- A Solução -->
        <section id="solucao" class="card">
            <h2>A Solução: Tecnologia Alinhada ao Campo</h2>
            <p>Com o uso de sensores de solo e imagens de satélite, o agricultor consegue mapear quais áreas estão com falta de nutrientes e quais estão saudáveis. As máquinas agrícolas reguladas por computador aplicam os insumos apenas onde há necessidade real, reduzindo drasticamente o uso de químicos e otimizando o tempo de trabalho.</p>
        </section>

        <!-- Interatividade (Script.js atuará aqui) -->
        <section id="interatividade" class="card highlight">
            <h2>Simulador de Impacto Sustentável</h2>
            <p>Descubra como a tecnologia reduz o desperdício. Escolha uma área de plantio e veja a diferença entre a agricultura tradicional e a de precisão!</p>
            
            <div class="form-group">
                <label for="tamanho-campo">Tamanho da sua plantação (em hectares):</label>
                <input type="number" id="tamanho-campo" min="1" max="1000" value="10">
            </div>
            
            <button onclick="calcularImpacto()">Simular Economia</button>

            <div id="resultado" class="hidden">
                <h3>Resultado da Simulação:</h3>
                <ul>
                    <li><strong>Água economizada:</strong> <span id="economia-agua">0</span> litros por ano.</li>
                    <li><strong>Defensivos evitados:</strong> <span id="economia-quimicos">0</span> kg/litros deixaram de poluir o solo.</li>
                    <li><strong>Redução de custos:</strong> R$ <span id="economia-financeira">0</span> economizados em insumos.</li>
                </ul>
                <p class="feedback-text">A tecnologia aplicada ao campo garante comida na mesa e preservação ambiental!</p>
            </div>
        </section>

        <!-- Relação com a Sustentabilidade -->
        <section id="sustentabilidade" class="card">
            <h2>Equilíbrio e Sustentabilidade</h2>
            <p>Este assunto conecta-se diretamente ao tema do Agrinho 2026. A agricultura de precisão prova que produzir mais não significa destruir mais. Ao preservar a saúde do solo e economizar recursos hídricos, garantimos que as futuras gerações também tenham terras férteis para cultivar. É a tecnologia garantindo o futuro do nosso planeta.</p>
        </section>

        <!-- Conclusão -->
        <section id="conclusao" class="card">
            <h2>Conclusão</h2>
            <p>O futuro do agro é tecnológico e verde. A agricultura de precisão transforma o setor produtivo em um aliado do meio ambiente. Unir a ciência da computação ao trabalho do campo é o caminho definitivo para um Brasil com agro forte e sustentabilidade real.</p>
        </section>

        <!-- Referências -->
        <section id="referencias" class="card text-muted">
            <h2>Referências</h2>
            <ul>
                <li>EMBRAPA. <strong>Agricultura de Precisão</strong>. Disponível em: &lt;https://embrapa.br&gt;.</li>
                <li>SENAR. <strong>Coleção Senar: Inovação e Tecnologias no Campo</strong>.</li>
                <li>Ministério da Agricultura e Pecuária. <strong>Plano ABC+ (Agricultura de Baixa Emissão de Carbono)</strong>.</li>
            </ul>
        </section>

    </main>

    <footer>
        <p>&copy; 2026 Projeto Escolar - Concurso Agrinho. Desenvolvido para o Ensino Médio.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Configurações Globais e Cores da Natureza */
:root {
    --primary-color: #2e7d32; /* Verde folha/campo */
    --secondary-color: #8d6e63; /* Marrom terra */
    --accent-color: #e8f5e9; /* Verde claro de fundo */
    --text-color: #3e2723; /* Marrom escuro para leitura confortável */
    --bg-color: #faf8f5; /* Bege bem claro */
    --white: #ffffff;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: var(--bg-color);
    color: var(--text-color);
    line-height: 1.6;
    padding-bottom: 40px;
}

.container {
    width: 90%;
    max-width: 900px;
    margin: 0 auto;
}

/* Cabeçalho */
header {
    background: linear-gradient(135deg, var(--primary-color), #1b5e20);
    color: var(--white);
    padding: 40px 0;
    text-align: center;
    border-bottom: 5px solid var(--secondary-color);
    margin-bottom: 30px;
}

header h1 {
    font-size: 1.8rem;
    margin-top: 10px;
    font-weight: 600;
}

.tagline {
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: #a5d6a7;
}

/* Cartões de Conteúdo */
.card {
    background-color: var(--white);
    padding: 25px;
    margin-bottom: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    border-left: 5px solid var(--primary-color);
}

.card h2 {
    color: var(--primary-color);
    margin-bottom: 12px;
    font-size: 1.4rem;
}

/* Destaque para a Seção Interativa */
.highlight {
    border: 2px solid var(--primary-color);
    background-color: var(--accent-color);
}

.form-group {
    margin: 20px 0 15px 0;
}

label {
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
}

input[type="number"] {
    width: 100%;
    max-width: 200px;
    padding: 10px;
    border: 2px solid var(--secondary-color);
    border-radius: 4px;
    font-size: 1rem;
}

button {
    background-color: var(--primary-color);
    color: var(--white);
    border: none;
    padding: 12px 24px;
    font-size: 1rem;
    font-weight: bold;
    border-radius: 4px;
    cursor: pointer;
    transition: background 0.3s;
}

button:hover {
    background-color: #1b5e20;
}

/* Resultados do Simulador */
#resultado {
    margin-top: 20px;
    padding: 15px;
    background-color: var(--white);
    border-radius: 6px;
    border: 1px solid #c8e6c9;
}

#resultado h3 {
    color: var(--secondary-color);
    margin-bottom: 10px;
}

#resultado ul {
    list-style-type: none;
    margin-bottom: 10px;
}

#resultado li {
    margin-bottom: 8px;
}

.feedback-text {
    font-style: italic;
    color: var(--primary-color);
    font-weight: bold;
}

.hidden {
    display: none;
}

/* Referências e Rodapé */
.text-muted {
    font-size: 0.9rem;
    border-left-color: var(--secondary-color);
}

.text-muted ul {
    padding-left: 20px;
}

footer {
    text-align: center;
    padding: 20px 0;
    color: var(--secondary-color);
    font-size: 0.85rem;
    margin-top: 40px;
}

/* Responsividade para Celulares */
@media (max-width: 600px) {
    header h1 {
        font-size: 1.4rem;
    }
    
    .card {
        padding: 15px;
    }
}
/**
 * Função interativa para o Concurso Agrinho 2026
 * Objetivo: Calcular estimativas de economia ambiental e financeira
 * baseado no tamanho da propriedade usando Agricultura de Precisão.
 */
function calcularImpacto() {
    // Captura o valor digitado pelo usuário no campo HTML
    const hectaresInput = document.getElementById('tamanho-campo').value;
    const hectares = parseFloat(hectaresInput);

    // Validação simples para garantir que o número é válido
    if (isNaN(hectares) || hectares <= 0) {
        alert("Por favor, insira um número válido de hectares maior que zero.");
        return;
    }

    // Dados médios estimados de economia por hectare/ano com tecnologia de precisão:
    // - 15.000 litros de água economizados (irrigação inteligente)
    // - 8 kg de defensivos evitados (aplicação localizada)
    // - R$ 450,00 de economia em insumos desperdiçados
    const aguaPorHectare = 15000;
    const quimicosPorHectare = 8;
    const reaisPorHectare = 450;

    // Realiza os cálculos multiplicando pelo tamanho informado
    const totalAgua = hectares * aguaPorHectare;
    const totalQuimicos = hectares * quimicosPorHectare;
    const totalReais = hectares * reaisPorHectare;

    // Insere os resultados calculados diretamente nas tags do HTML
    // toLocaleString('pt-BR') formata o número com os pontos de milhar nacionais
    document.getElementById('economia-agua').innerText = totalAgua.toLocaleString('pt-BR');
    document.getElementById('economia-quimicos').innerText = totalQuimicos.toLocaleString('pt-BR');
    document.getElementById('economia-financeira').innerText = totalReais.toLocaleString('pt-BR');

    // Remove a classe 'hidden' do CSS para tornar a div de resultados visível
    const divResultado = document.getElementById('resultado');
    divResultado.classList.remove('hidden');
}
