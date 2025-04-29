# Solucoes-Beer

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Soluções Beer</title>

    <link href="https://fonts.googleapis.com/css2?family=Lobster&family=Open+Sans&display=swap" rel="stylesheet">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        body {
            background-color: #000000;
            color: #ffffff;
            margin: 20px;
            animation: aparecer 3s ease-in;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Lobster', cursive;
        }

        p, li, a, label, input, textarea, button {
            font-family: 'Open Sans', sans-serif;
        }

        h1 {
            font-size: 60px;
            text-shadow: 2px 2px 5px #ff9900;
            text-align: center;
        }

        h2 {
            text-align: center;
            line-height: 0;
        }

        h3 {
            font-size: 30px;
        }

        h4 {
            font-size: 20px;
        }

        p {
            color: #cccccc;
            line-height: 1.8;
        }

        .centralizado {
            text-align: center;
        }

        a {
            color: #00ffff;
        }

        h6 {
            color: orange;
        }

        img {
            display: block;
            margin: 20px auto;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(255, 165, 0, 0.4);
        }

        .diferenciais-container {
            display: flex;
            align-items: flex-start;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 30px;
        }

        .texto-diferenciais {
            flex: 1;
            min-width: 300px;
        }

        .img-direita {
            max-width: 300px;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(255, 165, 0, 0.4);
        }

        ul li button {
            background-color: #111111;
            color: #d4af37;
            border: 1px solid #d4af37;
            padding: 10px 20px;
            margin: 5px;
            border-radius: 8px;
            cursor: pointer;
            transition: 1.5s;
        }

        ul li button:hover {
            background-color: #d4af37;
            color: #000000;
            transform: scale(1.1);
        }

        form input, form textarea {
            background-color: #222222;
            color: #ffffff;
            border: 1px solid #444444;
            padding: 8px;
            border-radius: 5px;
            width: 100%;
            max-width: 400px;
        }

        form button {
            background-color: #d4af37;
            color: #000;
            padding: 10px 20px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            transition: 0.3s;
        }

        form button:hover {
            background-color: #ff9900;
            transform: scale(1.1);
        }

        a.cardapio {
            display: inline-block;
            background-color: #d4af37;
            padding: 12px 25px;
            color: #000000;
            text-decoration: none;
            border-radius: 20px;
            font-weight: bold;
            box-shadow: 0 0 15px #d4af37;
            transition: 0.3s;
        }

        a.cardapio:hover {
            background-color: #ff9900;
            box-shadow: 0 0 25px #ff9900;
        }

        @keyframes aparecer {
            from {
                opacity: 0;
                transform: translate(-20px);
            }
            to {
                opacity: 1;
                transform: translate(0);
            }
        }

        @media (max-width: 768px) {
            .imagem-lateral {
                position: static;
                margin-top: 10px;
                opacity: 1 !important; /* Sempre visível no mobile */
                
            }

        .diferenciais-container {
            flex-direction: column;
            align-items: center;
        }
        .img-direita {
            margin-top: 20px;
        }

        }


        .botao-com-imagem {
            display: flex;
            align-items: center;
            gap: 20px;
            position: relative;
        }

        .imagem-lateral {
            max-width: 320px;
            position: absolute;
            left: 450px;
            top: -275px;
            border-radius: 12px;
            box-shadow: 0 0 15px rgba(255, 165, 0, 0.4);
            transition: opacity 0.3s ease-in-out;
            opacity: 0;
            pointer-events: none;
            z-index: 10;
        }


        #img-runberry {
    left: 450px; 
    top: -325px;
        }

        #img-curacaublue {
    left: 450px; 
    top: -375px;
        }

        #img-Marula {
    left: 450px; 
    top: -425px;
        }

        #img-Sunset {
    left: 450px; 
    top: -475px;
        }

        #img-Saquinho {
    left: 450px; 
    top: -525px;
        }

        #imagemCardapio {
    display: none;
    text-align: center;
    margin-top: 30px;
    position: relative;
    transition: top 0.5s ease-in-out;
        }

        #imagemCardapio.mover-para-cima {
    top: -750px; 
        }

        #formulario {
    transition: transform 0.5s ease-in-out;
        }

        #formulario.mover-para-cima {
    transform: translateY(-50px); 
        }

        #instagramBtn {
      position: relative;
      transition: top 0.5s ease;
        }

        .subir {
      top: -10px;
        }

        body {
    padding-bottom: 100px; 
        }


        .carrossel {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: -760px;
            display: none;
        }

        .carrossel img {
            max-width: 80%;
            max-height: 800px;
            display: none;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(255, 165, 0, 0.4);
        }

        .carrossel img.ativo {
            display: block;
        }

        .botao-carrossel {
            background-color: #d4af37;
            color: #000;
            padding: 10px;
            margin: 5px;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }

        .botao-carrossel:hover {
            background-color: #ff9900;
            transform: scale(1.1);
        }
        
   

    </style>
 
</head>


<body id="pagina">

    <h1>Bem-vindo ao Soluções Beer</h1>
    <h2>O melhor bar da cidade</h2>

    <p class="centralizado">Trabalhamos com os <strong>melhores drinks</strong>, cervejas <em>geladas</em> e porções de tira gosto.</p>

    <div class="diferenciais-container">
        <div class="texto-diferenciais">
            <h3>Nossos diferenciais:</h3>
            <p>
                Ambiente moderno <br>
                Atendimento exclusivo <br>
                Drinks personalizados
            </p>

            <h4>Visite-nos e viva a experiência!</h4>
            <h6>BEBA COM MODERAÇÃO</h6>

            <h3>Drinks Mais Pedidos:</h3>

            <ul>
                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-caipirinha">Caipirinhas</button>
                        <img id="img-caipirinha" src="IMG1/Caipirinhas.png" alt="Caipirinha" class="imagem-lateral">                        
                    </div>
                </li>

                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-RunBerry">Drink Run Berry</button>
                        <img id="img-runberry" src="IMG1/runberry.png" alt="Run Berry" class="imagem-lateral">

                    </div>
                </li>

                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-curacaublue">Drink Curaçau Blue</button>
                        <img id="img-curacaublue" src="IMG1/CuracauBlue.png" alt="Curacau blue" class="imagem-lateral">

                    </div>
                </li>


                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-Marula">Drink Marula</button>
                        <img id="img-Marula" src="IMG1/Marula.png" alt="Marula" class="imagem-lateral">
                    
                    </div>
                </li>


                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-Sunset">Drink Sunset</button>
                        <img id="img-Sunset" src="IMG1/Sunset.png" alt="Sunset" class="imagem-lateral">
                    
                    </div>                  
                </li>


                <li>
                    <div class="botao-com-imagem">
                        <button id="btn-Saquinho">Drinks Gourmet-Delivery</button>
                        <img id="img-Saquinho" src="IMG1/Saquinho.png" alt="Saquinho" class="imagem-lateral">
                    
                    </div>
                    
                </li>


                
            </ul>
        </div>


        <img src="IMG1/Entrada.jpg" width="300" alt="Entrada do Soluções Beer" class="img-direita">
    </div>

    
        <div id="conteudo-principal">
            <!-- todo o conteúdo atual que você quer esconder -->
        </div>
    

    <div style="text-align: center;">
        <a href="#" class="cardapio" id="btn-cardapio">Nosso Cardápio</a>
    </div>

     <div id="imagemCardapio" style="display: none; text-align: center; margin-top: 30px;">
        <img src="IMG1/cardapio1.png" alt="Imagem do Cardápio" style="width: 80%; max-width: 600px; border-radius: 10px;">
        
      </div>
      
      <div id="carrossel" class="carrossel">
        <button class="botao-carrossel" id="btn-anterior">Anterior</button>
        
        <img src="IMG1/cardapio2.png" alt="cardapio2" class="carrossel-imagem ativo">
        <img src="IMG1/cardapio3.png" alt="cardapio3" class="carrossel-imagem">
        <button class="botao-carrossel" id="btn-proximo">Próximo</button>
    </div>
      

    <br><br>

    <form id="formulario" action="#" method="post" onsubmit="enviarWhatsApp(event)">
        <label>Nome:</label><br>
        <input type="text" name="nome" id="nome" required><br><br>
    
        <label>Telefone:</label><br>
        <input type="tel" name="telefone" id="telefone" required><br><br>
    
        <label>Mensagem:</label><br>
        <textarea name="mensagem" id="mensagem"></textarea><br><br>
    
        <button type="submit" id="btnEnviar">Enviar</button>
    </form>

    <br>

    <a id="instagramBtn" href="https://instagram.com" target="_blank">Nosso Instagram</a>
    



    <!-- JavaScript para mostrar/ocultar a imagem da caipirinha -->
    <script>
        const btnCaipirinha = document.getElementById('btn-caipirinha');
        const imgCaipirinha = document.getElementById('img-caipirinha');
        const containerCaipirinha = btnCaipirinha.closest('.botao-com-imagem');
        containerCaipirinha.addEventListener('mouseenter', () => {
            imgCaipirinha.style.opacity = '1';
        });

        containerCaipirinha.addEventListener('mouseleave', () => {
            imgCaipirinha.style.opacity = '0';
        });


        const btnRunBerry = document.getElementById('btn-RunBerry');
        const imgRunBerry = document.getElementById('img-runberry');
        const containerRunBerry = btnRunBerry.closest('.botao-com-imagem');
        containerRunBerry.addEventListener('mouseenter', () => {
            imgRunBerry.style.opacity = '1';

        });

        containerRunBerry.addEventListener('mouseleave', () => {
            imgRunBerry.style.opacity = '0';
        });


        const btnCuracauBlue = document.getElementById('btn-curacaublue');
        const imgCuracauBlue = document.getElementById('img-curacaublue');
        const containerCuracauBlue = btnCuracauBlue.closest('.botao-com-imagem');
        containerCuracauBlue.addEventListener('mouseenter', () => {
            imgCuracauBlue.style.opacity = '1';

        });

        containerCuracauBlue.addEventListener('mouseleave', () => {
    imgCuracauBlue.style.opacity = '0';
});


        const btnMarula = document.getElementById('btn-Marula');
const imgMarula = document.getElementById('img-Marula');
const containerMarula = btnMarula.closest('.botao-com-imagem');
containerMarula.addEventListener('mouseenter', () => {
    imgMarula.style.opacity = '1';
});
containerMarula.addEventListener('mouseleave', () => {
    imgMarula.style.opacity = '0';
});

const btnSunset = document.getElementById('btn-Sunset');
const imgSunset = document.getElementById('img-Sunset');
const containerSunset = btnSunset.closest('.botao-com-imagem');
containerSunset.addEventListener('mouseenter', () => {
    imgSunset.style.opacity = '1';
});
containerSunset.addEventListener('mouseleave', () => {
    imgSunset.style.opacity = '0';
});

const btnSaquinho = document.getElementById('btn-Saquinho');
const imgSaquinho = document.getElementById('img-Saquinho');
const containerSaquinho = btnSaquinho.closest('.botao-com-imagem');
containerSaquinho.addEventListener('mouseenter', () => {
    imgSaquinho.style.opacity = '1';
});
containerSaquinho.addEventListener('mouseleave', () => {
    imgSaquinho.style.opacity = '0';
});

        const botaoCardapio = document.getElementById("btn-cardapio");
        const imagemCardapio = document.getElementById("imagemCardapio");
        const conteudoPrincipal = document.getElementById("conteudo-principal");

        const pagina = document.getElementById('pagina');
        pagina.style.paddingBottom = '0';
    

        botaoCardapio.addEventListener("click", function(e) {
         e.preventDefault(); 
         conteudoPrincipal.style.display = "none"; 
         imagemCardapio.style.display = "block"; 
         imagemCardapio.classList.add("mover-para-cima");
         document.getElementById("formulario").classList.add("mover-para-cima");
         moverInstagram();

         function moverInstagram() {
         document.getElementById('instagramBtn').classList.add('subir');
    }

        });

     


    function mostrarInstagram() {
      document.getElementById('instagramBtn').style.display = 'inline-block';
    }


    function enviarWhatsApp(event) {
        event.preventDefault(); // Previne o envio padrão do formulário

        const nome = document.getElementById("nome").value;
        const telefone = document.getElementById("telefone").value;
        const mensagem = document.getElementById("mensagem").value;

        // Formatação da mensagem
        const textoMensagem = `Olá, ja vamos te atender... ${nome}, meu telefone é ${telefone}. Mensagem: ${mensagem}`;

        // Número do WhatsApp da empresa
        const numeroWhatsApp = "5511947511907"; // Substitua com o número real da empresa

        // Link do WhatsApp com a mensagem
        const urlWhatsApp = `https://wa.me/${5511947511907}?text=${encodeURIComponent(textoMensagem)}`;

        // Redireciona para o WhatsApp
        window.open(urlWhatsApp, '_blank');
    }

   

    
    // Aqui você pode ocultar o formulário ou mostrar uma mensagem de sucesso
    alert('Enviado com sucesso!');
    document.getElementById('formulario').reset();  // Limpar o formulário
         

        
        const carrossel = document.getElementById("carrossel");
        const imagensCarrossel = document.querySelectorAll(".carrossel-imagem");
        const btnAnterior = document.getElementById("btn-anterior");
        const btnProximo = document.getElementById("btn-proximo");
        let indiceAtual = 0;

        botaoCardapio.addEventListener("click", function (e) {
            e.preventDefault();
            carrossel.style.display = "flex";
        });

        btnProximo.addEventListener("click", function () {
            imagensCarrossel[indiceAtual].classList.remove("ativo");
            indiceAtual = (indiceAtual + 1) % imagensCarrossel.length;
            imagensCarrossel[indiceAtual].classList.add("ativo");
        });

        btnAnterior.addEventListener("click", function () {
            imagensCarrossel[indiceAtual].classList.remove("ativo");
            indiceAtual = (indiceAtual - 1 + imagensCarrossel.length) % imagensCarrossel.length;
            imagensCarrossel[indiceAtual].classList.add("ativo");
        });


  

    </script>

    

</body>
</html>
