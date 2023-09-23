### João Gabryel:
### Código HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabela</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <h1>Dados Pessoais</h1>
    <table>
        <tr>
            <th> Nome </th>
            <th> Idade </th>
            <th> E-mail </th>
            <th> Endereço </th>
        </tr>
        <tr>
            <td>João</td>
            <td>19</td>
            <td>joao@gmail.com</td>
            <td>Rua A, 111, Jardim B</td>
        </tr>
        <tr>
            <td>João Gabryel</td>
            <td>25</td>
            <td>joaox@gmail.com</td>
            <td>Rua B, 111, Jardim B</td>
        </tr>
        <tr>
            <td>João Santos</td>
            <td>18</td>
            <td>joaoxd@gmail.com</td>
            <td>Rua C, 111, Jardim A</td>
        </tr>
    </table>
</body>

</html>

### CSS
body{
    background-color: cornflowerblue;
    font-family: Arial, Helvetica, sans-serif;
}
h1{
    text-align: center;
    border: 1px solid black;
    background-color: darkblue;
}
table {
    border-collapse: collapse;
    width: 100%;
    text-align: center;
    border: 1px solid black;
}
table th{
    background-color: rgb(219, 178, 90);
}
table td{
    background-color: rgb(160, 8, 8);
}
td, th {
    border: 1px solid #080808;
    text-align: center;
    padding: 15px;
}

  