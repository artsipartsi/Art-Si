<?php
// Kovakoodattu taulu (tulevaisuudessa voidaan hakea MySQL:stä)
$vocabulary = [
    ["id" => 1, "word" => "AURINKO", "clue" => "Taivaankappale"],
    ["id" => 2, "word" => "KUU", "clue" => "Maan kiertolainen"],
    ["id" => 3, "word" => "TÄHTI", "clue" => "Loistaa yöllä"],
    ["id" => 4, "word" => "METRO", "clue" => "Kaupunkijuna"],
    ["id" => 5, "word" => "JOULU", "clue" => "Juhlitaan joulukuussa"],
    ["id" => 6, "word" => "LAIVA", "clue" => "Kulkee merellä"],
    ["id" => 7, "word" => "VUORI", "clue" => "Korkea maastonmuoto"],
    ["id" => 8, "word" => "KYLMÄ", "clue" => "Matala lämpötila"],
    ["id" => 9, "word" => "HÄRKÄ", "clue" => "Iso sarvipäinen eläin"],
    ["id" => 10, "word" => "KALA", "clue" => "Elää vedessä"],
    // Lisää 40 muuta sanaa...
];

// Funktio, joka muuntaa jokerimerkit * ja . regulaari-ilmaisuksi
function wildcardToRegex($pattern) {
    $pattern = str_replace('*', '.*', $pattern); // * → mielivaltainen merkkijono
    $pattern = str_replace('.', '.', $pattern); // . → mikä tahansa yksi merkki
    return "/^" . $pattern . "$/u"; // Lisää alku- ja loppumerkit, jotta koko sana täsmää
}

// Käsitellään hakuehto
$searchQuery = isset($_GET['query']) ? strtoupper(trim($_GET['query'])) : '';
$results = [];

if ($searchQuery !== '') {
    $regex = wildcardToRegex($searchQuery);
    foreach ($vocabulary as $entry) {
        if (preg_match($regex, $entry["word"])) {
            $results[] = $entry;
        }
    }
}
?>

<!DOCTYPE html>
<html lang="fi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ristikkohaku</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
</head>
<body class="container mt-4">
    <h2>Ristikkohaku</h2>
    <form method="GET" class="mb-3">
        <input type="text" name="query" class="form-control" placeholder="Kirjoita hakuehto (esim. K.*A)" value="<?= htmlspecialchars($searchQuery) ?>">
        <button type="submit" class="btn btn-primary mt-2">Hae</button>
    </form>

    <?php if ($searchQuery !== ''): ?>
        <h3>Hakutulokset:</h3>
        <table class="table table-bordered">
            <thead>
                <tr>
                    <th>Sana</th>
                    <th>Vihje</th>
                </tr>
            </thead>
            <tbody>
                <?php if (count($results) > 0): ?>
                    <?php foreach ($results as $entry): ?>
                        <tr>
                            <td><?= htmlspecialchars($entry["word"]) ?></td>
                            <td><?= htmlspecialchars($entry["clue"]) ?></td>
                        </tr>
                    <?php endforeach; ?>
                <?php else: ?>
                    <tr>
                        <td colspan="2">Ei osumia</td>
                    </tr>
                <?php endif; ?>
            </tbody>
        </table>
    <?php endif; ?>
</body>
</html>