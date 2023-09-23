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
                <label for="n1" class="form-label">Primeiro Número:</label>
                <input type="number" class="form-control" id="n1" name="n1">
            </div>
            <div class="mb-3">
                <label for="n2" class="form-label">Segundo Número:</label>
                <input type="number" class="form-control" id="n2" name="n2">
            </div>
            <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
    </div>
    <?php
     if (isset($_POST["n1"]) && isset($_POST["n2"])){
    $n1 = $_POST["n1"];
    $n2 = $_POST["n2"];
    $soma = $n1 + $n2;
   
        if ($soma > 20) {
            echo "A soma dos dois números é: $soma";
            echo "<br>";
            echo "Serão somados mais 8: ";
            $soma = $soma + 8;
            echo $soma;
        } else {
            echo "A soma dos dois números é: $soma";
            echo "<br>";
            echo "Serão subtraídos 5: ";
            $soma = $soma - 5;
            echo $soma;
        }
    }
    
    ?>

</body>