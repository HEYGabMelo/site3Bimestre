<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transformação Pessoal - Seu Caminho para o Crescimento</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --primary: #4F46E5;
            --secondary: #10B981;
            --dark: #1F2937;
            --light: #F9FAFB;
            --accent: #F59E0B;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }
        
        .skip-link {
            position: absolute;
            top: -40px;
            left: 0;
            background: var(--primary);
            color: white;
            padding: 8px;
            z-index: 1000;
            transition: top 0.3s;
        }
        
        .skip-link:focus {
            top: 0;
        }
        
        .high-contrast {
            --primary: #000000;
            --secondary: #FFFF00;
            --dark: #000000;
            --light: #FFFFFF;
            --accent: #FF0000;
            filter: contrast(1.4);
        }
        
        .image-container {
            position: relative;
            overflow: hidden;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .image-container img {
            width: 100%;
            height: auto;
            transition: transform 0.3s ease;
        }
        
        .image-container:hover img {
            transform: scale(1.05);
        }
        
        .accessibility-controls {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: white;
            padding: 15px;
            border-radius: 50px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            z-index: 1000;
            display: flex;
            gap: 10px;
        }
        
        .contrast-btn, .text-size-btn {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            border: none;
            background: var(--primary);
            color: white;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .contrast-btn:hover, .text-size-btn:hover {
            transform: scale(1.1);
            background: var(--secondary);
        }
        
        .large-text {
            font-size: 1.2em;
            line-height: 1.8;
        }
        
        @media (max-width: 768px) {
            .accessibility-controls {
                bottom: 10px;
                right: 10px;
                padding: 10px;
            }
            
            .contrast-btn, .text-size-btn {
                width: 40px;
                height: 40px;
                font-size: 0.8em;
            }
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Skip link para acessibilidade -->
    <a href="#main-content" class="skip-link">Pular para o conteúdo principal</a>
    
    <!-- Controles de acessibilidade -->
    <div class="accessibility-controls">
        <button class="contrast-btn" onclick="toggleContrast()" aria-label="Alternar modo de alto contraste">
            A/C
        </button>
        <button class="text-size-btn" onclick="toggleTextSize()" aria-label="Aumentar tamanho do texto">
            A+
        </button>
    </div>

    <!-- Header -->
    <header class="bg-white shadow-lg">
        <nav class="container mx-auto px-6 py-4" aria-label="Navegação principal">
            <div class="flex justify-between items-center">
                <a href="#" class="text-2xl font-bold text-indigo-600" aria-label="Transformação Pessoal - Página inicial">
                    🌱 Transformação Pessoal
                </a>
                
                <div class="hidden md:flex space-x-8">
                    <a href="#sobre" class="text-gray-700 hover:text-indigo-600 transition-colors">Sobre</a>
                    <a href="#recursos" class="text-gray-700 hover:text-indigo-600 transition-colors">Recursos</a>
                    <a href="#blog" class="text-gray-700 hover:text-indigo-600 transition-colors">Blog</a>
                    <a href="#contato" class="text-gray-700 hover:text-indigo-600 transition-colors">Contato</a>
                </div>
                
                <button class="md:hidden text-gray-700" aria-label="Abrir menu">
                    ☰
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-gradient-to-r from-indigo-500 to-purple-600 text-white py-20">
        <div class="container mx-auto px-6 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold mb-6" style="text-shadow: 2px 2px 4px rgba(0,0,0,0.3);">
                    Descubra Seu Potencial Ilimitado
                </h1>
                <p class="text-xl mb-8 opacity-90">
                    Ferramentas e estratégias para seu crescimento pessoal e profissional com acessibilidade para todos.
                </p>
                <div class="flex flex-wrap gap-4">
                    <button class="bg-white text-indigo-600 px-8 py-3 rounded-full font-semibold hover:bg-gray-100 transition-colors">
                        Começar Agora
                    </button>
                    <button class="border-2 border-white text-white px-8 py-3 rounded-full font-semibold hover:bg-white hover:text-indigo-600 transition-colors">
                        Saiba Mais
                    </button>
                </div>
            </div>
            <div class="md:w-1/2">
                <div class="image-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/173b1c1c-e2b6-4753-9e3c-00862872f136.png" alt="Pessoa meditando em posição de lótus com luz suave do amanhecer ao fundo representando paz interior e autoconhecimento" />
                </div>
            </div>
        </div>
    </section>

    <!-- Sobre -->
    <section id="sobre" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-16 text-gray-800">Sobre Desenvolvimento Pessoal</h2>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <div class="image-container">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d3f70f93-337d-4a8f-9a9a-c36bb39b32f9.png" alt="Grupo diversificado de pessoas em workshop de desenvolvimento pessoal compartilhando experiências e aprendizado colaborativo" />
                    </div>
                </div>
                <div>
                    <h3 class="text-2xl font-semibold mb-6 text-indigo-600">O que é Desenvolvimento Pessoal?</h3>
                    <p class="text-gray-700 mb-6">
                        Desenvolvimento pessoal é uma jornada contínua de autoconhecimento, crescimento e transformação. 
                        Envolve o desenvolvimento de habilidades, competências e atitudes que nos permitem alcançar 
                        nosso máximo potencial em todas as áreas da vida.
                    </p>
                    <p class="text-gray-700 mb-8">
                        Nossa missão é tornar essa jornada acessível para todos, independentemente de habilidades 
                        físicas, cognitivas ou sensoriais. Acreditamos que o crescimento pessoal deve ser inclusivo 
                        e disponível para cada pessoa.
                    </p>
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-indigo-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-indigo-800 mb-2">Autoconhecimento</h4>
                            <p class="text-sm text-gray-600">Descubra suas forças e áreas de crescimento</p>
                        </div>
                        <div class="bg-green-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-green-800 mb-2">Habilidades</h4>
                            <p class="text-sm text-gray-600">Desenvolva competências para o sucesso</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Recursos -->
    <section id="recursos" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-16 text-gray-800">Recursos Acessíveis</h2>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Recurso 1 -->
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
                    <div class="image-container mb-6">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/3c1dacac-f5bb-4153-9060-97eaf9bf9d1f.png" alt="Pessoa usando leitor de tela com fones de ouvido enquanto navega em conteúdo digital acessível com interface limpa e clara" />
                    </div>
                    <h3 class="text-xl font-semibold mb-4 text-indigo-600">Conteúdo Acessível</h3>
                    <p class="text-gray-700 mb-4">
                        Todos nossos materiais são desenvolvidos seguindo as diretrizes de acessibilidade WCAG, 
                        garantindo que pessoas com diferentes habilidades possam acessar o conteúdo.
                    </p>
                    <ul class="text-sm text-gray-600 space-y-1">
                        <li>• Leitores de tela compatíveis</li>
                        <li>• Alto contraste disponível</li>
                        <li>• Navegação por teclado</li>
                    </ul>
                </div>
                
                <!-- Recurso 2 -->
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
                    <div class="image-container mb-6">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/18c8ded5-11ec-438d-b038-a476a588b14c.png" alt="Workshop virtual com intérprete de libras em vídeo e legendas em tempo real para participantes com deficiência auditiva" />
                    </div>
                    <h3 class="text-xl font-semibold mb-4 text-green-600">Workshops Inclusivos</h3>
                    <p class="text-gray-700 mb-4">
                        Oferecemos workshops e treinamentos com recursos de acessibilidade como intérpretes de libras, 
                        legendas e materiais em formatos alternativos.
                    </p>
                    <ul class="text-sm text-gray-600 space-y-1">
                        <li>• Intérpretes de libras</li>
                        <li>• Legendas em tempo real</li>
                        <li>• Materiais adaptados</li>
                    </ul>
                </div>
                
                <!-- Recurso 3 -->
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
                    <div class="image-container mb-6">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/43388a8a-dfa3-4f54-80d2-46046b323f54.png" alt="Comunidade online diversa interagindo em plataforma acessível com interface adaptável e suporte para diferentes necessidades" />
                    </div>
                    <h3 class="text-xl font-semibold mb-4 text-orange-600">Comunidade</h3>
                    <p class="text-gray-700 mb-4">
                        Participe de uma comunidade inclusiva onde todos são bem-vindos. Compartilhe experiências, 
                        aprenda com outros e cresça junto em um ambiente acolhedor.
                    </p>
                    <ul class="text-sm text-gray-600 space-y-1">
                        <li>• Grupos de apoio</li>
                        <li>• Mentoria acessível</li>
                        <li>• Eventos inclusivos</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Blog -->
    <section id="blog" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center mb-16 text-gray-800">Artigos Recentes</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Artigo 1 -->
                <article class="bg-gray-50 rounded-xl overflow-hidden hover:shadow-lg transition-shadow">
                    <div class="image-container">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/20a42cdb-5d5f-4e91-96ef-eb89d6ed83ad.png" alt="Pessoa praticando mindfulness em ambiente natural tranquilo com técnica de respiração consciente e relaxamento" />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-3 text-indigo-600">Mindfulness no Dia a Dia</h3>
                        <p class="text-gray-700 mb-4">
                            Descubra como praticar mindfulness pode transformar sua rotina e melhorar sua qualidade de vida.
                        </p>
                        <a href="#" class="text-indigo-600 font-semibold hover:underline">Ler mais →</a>
                    </div>
                </article>
                
                <!-- Artigo 2 -->
                <article class="bg-gray-50 rounded-xl overflow-hidden hover:shadow-lg transition-shadow">
                    <div class="image-container">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c4ea2904-5824-473f-8ba0-e5f31b35054e.png" alt="Metas e objetivos organizados em quadro visual com cores vibrantes e sistema de acompanhamento de progresso" />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-3 text-green-600">Definindo Metas Realistas</h3>
                        <p class="text-gray-700 mb-4">
                            Aprenda a estabelecer metas alcançáveis e criar um plano de ação eficaz para seu crescimento.
                        </p>
                        <a href="#" class="text-green-600 font-semibold hover:underline">Ler mais →</a>
                    </div>
                </article>
                
                <!-- Artigo 3 -->
                <article class="bg-gray-50 rounded-xl overflow-hidden hover:shadow-lg transition-shadow">
                    <div class="image-container">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f1efd280-faa8-44a1-8f41-4ef3dc4b6ecf.png" alt="Rede de apoio com pessoas diversas se conectando e compartilhando experiências de crescimento pessoal em ambiente inclusivo" />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-3 text-orange-600">Construindo Redes de Apoio</h3>
                        <p class="text-gray-700 mb-4">
                            Como criar e manter relacionamentos saudáveis que apoiam seu desenvolvimento pessoal.
                        </p>
                        <a href="#" class="text-orange-600 font-semibold hover:underline">Ler mais →</a>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section class="py-20 bg-gradient-to-r from-indigo-500 to-purple-600 text-white">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-3xl font-bold mb-6">Junte-se à Nossa Comunidade</h2>
            <p class="text-xl mb-8 opacity-90 max-w-2xl mx-auto">
                Receba conteúdos exclusivos, dicas de desenvolvimento pessoal e novidades sobre acessibilidade.
            </p>
            <form class="max-w-md mx-auto flex flex-col sm:flex-row gap-4">
                <input 
                    type="email" 
                    placeholder="Seu melhor email" 
                    class="flex-1 px-4 py-3 rounded-full text-gray-800 focus:outline-none focus:ring-2 focus:ring-white"
                    aria-label="Digite seu email para se inscrever na newsletter"
                    required
                >
                <button 
                    type="submit" 
                    class="bg-white text-indigo-600 px-8 py-3 rounded-full font-semibold hover:bg-gray-100 transition-colors"
                >
                    Inscrever
                </button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contato" class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-semibold mb-4">Transformação Pessoal</h3>
                    <p class="text-gray-400">
                        Desenvolvimento pessoal acessível para todos. Crescimento inclusivo e transformador.
                    </p>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Links Rápidos</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#sobre" class="hover:text-white">Sobre</a></li>
                        <li><a href="#recursos" class="hover:text-white">Recursos</a></li>
                        <li><a href="#blog" class="hover:text-white">Blog</a></li>
                        <li><a href="#contato" class="hover:text-white">Contato</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Suporte</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#" class="hover:text-white">Acessibilidade</a></li>
                        <li><a href="#" class="hover:text-white">FAQ</a></li>
                        <li><a href="#" class="hover:text-white">Privacidade</a></li>
                        <li><a href="#" class="hover:text-white">Termos</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Contato</h4>
                    <p class="text-gray-400 mb-2">contato@transformacaopessoal.com</p>
                    <p class="text-gray-400 mb-4">+55 (11) 99999-9999</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white" aria-label="Facebook">📘</a>
                        <a href="#" class="text-gray-400 hover:text-white" aria-label="Instagram">📷</a>
                        <a href="#" class="text-gray-400 hover:text-white" aria-label="YouTube">📺</a>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>© 2024 Transformação Pessoal. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Funções de acessibilidade
        function toggleContrast() {
            document.body.classList.toggle('high-contrast');
            const btn = document.querySelector('.contrast-btn');
            if (document.body.classList.contains('high-contrast')) {
                btn.textContent = 'A/C';
                btn.setAttribute('aria-label', 'Desativar modo de alto contraste');
            } else {
                btn.textContent = 'A/C';
                btn.setAttribute('aria-label', 'Ativar modo de alto contraste');
            }
        }
        
        function toggleTextSize() {
            document.body.classList.toggle('large-text');
            const btn = document.querySelector('.text-size-btn');
            if (document.body.classList.contains('large-text')) {
                btn.textContent = 'A-';
                btn.setAttribute('aria-label', 'Reduzir tamanho do texto');
            } else {
                btn.textContent = 'A+';
                btn.setAttribute('aria-label', 'Aumentar tamanho do texto');
            }
        }
        
        // Smooth scrolling para links âncora
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
        
        // Focar no conteúdo principal após skip link
        document.querySelector('.skip-link').addEventListener('click', function() {
            setTimeout(() => {
                document.getElementById('main-content')?.focus();
            }, 1000);
        });
    </script>
</body>
</html>
