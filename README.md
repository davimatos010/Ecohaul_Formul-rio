!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ecohaul - Página Inicial</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            text-align: center;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 3em 0;
        }
        .container {
            padding: 2em;
        }
        .description {
            margin-bottom: 1em;
        }
        .images img {
            width: 200px;
            margin: 1px;
        }
        .buttons {
            margin-top: 0.5em;
        }
        .buttons a {
            display: inline-block;
            padding: 1em 1em;
            margin: 1 2em;
            text-decoration: none;
            color: white;
            background-color: #4CAF50;
            border-radius: 5px;
        }
        .buttons a:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>Ecohaul: Sua Solução de Transporte Sustentável</h1>
    </header>
    <div class="container">
        <div class="description">
            <p>Ecohaul é uma plataforma inovadora que oferece soluções de transporte ecológicas, conectando clientes e transportadores comprometidos com a sustentabilidade.</p>
        </div>
        <div class="images">
            <img src="https://tse3.mm.bing.net/th?id=OIP.OkRr3yMa67QVz_NeGpamuAHaFj&pid=Api&P=0&h=180"Caminhão Elétrico">
            <img src="https://tse2.mm.bing.net/th?id=OIP.XY7GR9KVULdZIxFBgF1pqQHaHa&pid=Api&P=0&h=180" alt="Logotipo Ecohaul">
        </div>
        <div class="buttons">
            <a href="cadastro_cliente.html">Sou Cliente</a>
            <a href="cadastro_transportador.html">Sou Transportador</a>
        </div>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro de Cliente - Ecohaul</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background-color: white;
            padding: 2em;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
        }
        .form-container h2 {
            margin-bottom: 1em;
            color: #4CAF50;
        }
        .form-container label {
            display: block;
            margin-bottom: 0.5em;
            font-weight: bold;
        }
        .form-container input[type="text"],
        .form-container input[type="email"],
        .form-container input[type="password"],
        .form-container textarea {
            width: 100%;
            padding: 0.5em;
            margin-bottom: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .form-container button {
            width: 100%;
            padding: 0.5em;
            border: none;
            border-radius: 5px;
            background-color: #4CAF50;
            color: white;
            font-size: 1em;
        }
        .form-container button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h2>Cadastro de Cliente</h2>
        <form action="/submit_cliente" method="post">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="senha">Senha:</label>
            <input type="password" id="senha" name="senha" required>
            
            <label for="endereco">Endereço:</label>
            <textarea id="endereco" name="endereco" rows="4" required></textarea>
            
            <button type="submit">Cadastrar</button>
        </form>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro de Transportador - Ecohaul</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background-color: white;
            padding: 2em;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
        }
        .form-container h2 {
            margin-bottom: 1em;
            color: #4CAF50;
        }
        .form-container label {
            display: block;
            margin-bottom: 0.5em;
            font-weight: bold;
        }
        .form-container input[type="text"],
        .form-container input[type="email"],
        .form-container input[type="password"],
        .form-container input[type="tel"],
        .form-container textarea {
            width: 100%;
            padding: 0.5em;
            margin-bottom: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .form-container button {
            width: 100%;
            padding: 0.5em;
            border: none;
            border-radius: 5px;
            background-color: #4CAF50;
            color: white;
            font-size: 1em;
        }
        .form-container button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h2>Cadastro de Transportador</h2>
        <form action="/submit_transportador" method="post">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="senha">Senha:</label>
            <input type="password" id="senha" name="senha" required>
            
            <label for="telefone">Telefone:</label>
            <input type="tel" id="telefone" name="telefone" required>
            
            <label for="veiculo">Tipo de Veículo:</label>
            <textarea id="veiculo" name="veiculo" rows="2" required></textarea>
            
            <button type="submit">Cadastrar</button>
        </form>
    </div>
</body>
</html>
