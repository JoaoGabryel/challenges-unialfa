### João Gabryel:
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
</head>

<body>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm" crossorigin="anonymous"></script>
    <div class="container">
        <form method="POST">
            <div class="mb-3">
                <label for="livro" class="form-label">Livro:</label>
                <input type="text" class="form-control" id="livro" name="livro">
            </div>
            <label for="tipo_usuario">Tipo de Usuário:</label>
            <select id="tipo_usuario" name="tipo_usuario" required>
                <option value="professor">Professor</option>
                <option value="aluno">Aluno</option>
            </select><br><br>
            <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
    </div>
    <?php
    if (isset($_POST["livro"]) && isset($_POST["tipo_usuario"])) {
        $livro = $_POST["livro"];
        $tipo_usuario = $_POST["tipo_usuario"];

        if ($tipo_usuario == "professor") {
            echo "<h1>Recibo de Empréstimo</h1>";
            echo "Livro: $livro<br>";
            echo "Como você é $tipo_usuario, você tem 10 dias para devolver o livro.<br>";
        } else {
            echo "<h1>Recibo de Empréstimo</h1>";
            echo "Livro: $livro<br>";
            echo "Como você é $tipo_usuario, você tem 3 dias para devolver o livro.<br>";
        }
    }

    ?>
</body>