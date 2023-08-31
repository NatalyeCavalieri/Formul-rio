<!DOCTYPE html>
<html>
<head>
    <title>Formulário de Admissão Veterinária</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            width: 60%;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        label {
            font-weight: bold;
        }
        input[type="text"], select {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }
        textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }
        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 3px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Formulário de Admissão Veterinária</h1>
        <form action="processar_formulario.php" method="post">
            <h2>Dados Gerais</h2>
            <label>Número:</label>
            <input type="text" name="numero">
            <label>Nome:</label>
            <input type="text" name="nome">
            <label>Idade:</label>
            <input type="text" name="idade">
            <label>Espécie:</label>
            <input type="text" name="especie">
            <label>Sexo:</label>
            <select name="sexo">
                <option value="macho">Macho</option>
                <option value="femea">Fêmea</option>
            </select>
            <label>Raça:</label>
            <input type="text" name="raca">
            <label>Pelagem:</label>
            <input type="text" name="pelagem">
            <label>Porte:</label>
            <input type="text" name="porte">
            <label>Microchip:</label>
            <input type="text" name="microchip">
            
            <h2>Histórico</h2>
            <label>Castrado:</label>
            <input type="radio" name="castrado" value="sim"> Sim
            <input type="radio" name="castrado" value="nao"> Não
            <br>
            <label>Histórico de procedimentos cirúrgicos/anestésicos:</label>
            <textarea name="historico_procedimentos" rows="4"></textarea>
            <label>Enfermidades prévias:</label>
            <textarea name="enfermidades_previas" rows="4"></textarea>
            <label>Tratamento crônico:</label>
            <textarea name="tratamento_cronico" rows="4"></textarea>
            <label>Alergia? (dieta/medicamentos):</label>
            <input type="text" name="alergia">
            <label>Dieta:</label>
            <input type="text" name="dieta">
            <label>Vacinação:</label>
            <input type="text" name="vacinacao">
            
            <h2>Quadro Atual</h2>
            <label>Veterinário responsável:</label>
            <input type="text" name="veterinario_responsavel">
            <label>Data de Admissão:</label>
            <input type="text" name="data_admissao">
            <label>Sintomatologia:</label>
            <textarea name="sintomatologia" rows="4"></textarea>
            <label>Exames:</label>
            <textarea name="exames" rows="4"></textarea>
            <label>Suspeita Diagnóstica:</label>
            <input type="text" name="suspeita_diagnostica">
            
            <br>
            <input type="submit" value="Enviar Formulário">
        </form>
    </div>
</body>
</html>
