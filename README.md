<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mini Cursos</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: #000;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
        }

        #termos {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            z-index: 9999;
        }

        button {
            padding: 12px 22px;
            font-size: 16px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
        }

        #btnContinuar {
            background-color: #1db954;
            color: white;
            margin-top: 20px;
        }

        #btnComprar {
            background-color: #0084ff;
            color: white;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <div id="termos">
        <h2>Termo de Segurança</h2>
        <p>Depois de comprar o curso não tem devolução, então só compre se não fizer falta.</p>
        <button id="btnContinuar">Concordar e Continuar</button>
    </div>

    <h1>Compre Mini Cursos</h1>
    <p>Compre tutoriais para investir</p>

    <a href="https://wa.me/558396056952" target="_blank">
        <button id="btnComprar">Comprar Mini Curso</button>
    </a>

    <script>
        alert('Termo de segurança: Depois de comprar o curso não tem devolução.');
        document.getElementById("btnContinuar").addEventListener("click", function () {
            document.getElementById("termos").style.display = "none";
        });
    </script>

</body>
</html>


[site.txt](https://github.com/user-attachments/files/23338666/site.txt)
