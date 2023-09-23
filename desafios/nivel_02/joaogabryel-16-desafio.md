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
        <form method="POST" >
            <div class="mb-3">
                <label for="mult" class="form-label">Número</label>
                <input type="number" class="form-control" id="mult" name="mult">

            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>
    </div>
    <?php
        if (isset($_POST["mult"])) {
            $mult = $_POST["mult"];
            for ($i = 1; $i <= 10; $i++) {
                echo "$mult X $i = " . ($mult * $i) . "<br>";
            }
        }
?>
</body>

</html>