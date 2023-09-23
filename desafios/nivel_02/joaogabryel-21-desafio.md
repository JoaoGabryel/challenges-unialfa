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
        <h1>Conta Corrente</h1>
        <form method="POST">
            <div class="mb-3">
                <label for="titular" class="form-label">Titular:</label>
                <input type="text" class="form-control" id="titular" name="titular">
            </div>
            <div class="mb-3">
                <label for="saldo" class="form-label">Saldo:</label>
                <input type="number" class="form-control" id="saldo" name="saldo">
            </div>
            <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
    </div>
   <?php
   if(isset($_POST["titular"]) && isset($_POST["saldo"])){
    $titular = $_POST["titular"];
    $saldo = $_POST["saldo"];
 
     for($i=1;$i<=4;$i++){
         echo "Titular da Conta $i: $titular<br>";
     }
   }
  
   ?>
</body>