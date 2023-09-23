### João Gabryel
<?php
$contasCorrentes = [
    ["titular" => "João", "saldo" => 1000],
    ["titular" => "Jonas", "saldo" => 2000],
    ["titular" => "Jacinto", "saldo" => 3000],
    ["titular" => "Jaime", "saldo" => 4000]
];

foreach ($contasCorrentes as $conta) {
    echo "Titular: " . $conta["titular"] . "<br>";
}
?>