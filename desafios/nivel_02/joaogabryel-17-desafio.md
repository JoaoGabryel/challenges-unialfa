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
                <label for="peso" class="form-label">Peso:</label>
                <input type="number" class="form-control" id="peso" name="peso">
            </div>
            <div class="mb-3">
                <label for="altura" class="form-label">Altura:</label>
                <input type="number" class="form-control" id="altura" name="altura">
            </div>
            <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
    </div>
    <?php
if (isset($_POST["peso"]) && isset($_POST["altura"])) {
    $peso = $_POST["peso"];
    $altura = $_POST["altura"];
    $imc = $peso / ($altura * $altura);

    if ($imc < 0.0017) {
        echo "Seu peso é $peso kg, sua altura é $altura cm e seu IMC é de $imc, você está abaixo do peso.";
    } else if ($imc >= 0.0025) {
        echo "Seu peso é $peso kg, sua altura é $altura cm e seu IMC é de $imc, você está acima do peso.";
    } else{
        echo "Seu peso é $peso kg, sua altura é $altura cm e seu IMC é de $imc, peso regular.";
    }
}
?>
</body>

</html>