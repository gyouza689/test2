<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>発注</title>
    <script>
        function displayInput() {
            // フォームの入力値を取得
            var pum = document.getElementById("pum").value;
            var cuc = document.getElementById("cuc").value;

            // 結果を表示する要素を更新
            document.getElementById("result").innerHTML = "かぼちゃ: " + pum + "<br>きゅうり: " + cuc;
        }
    </script>
</head>
<body>
    <h1>個数を入力してください</h1>
    
    <form action="javascript:void(0);" onsubmit="displayInput()">
        <label for="pum">かぼちゃ:</label>
        <input type="text" id="pum" name="pum" required><br><br>
        
        <label for="cuc">きゅうり:</label>
        <input type="text" id="cuc" name="cuc" required><br><br>

        <button type="submit">送信</button>
    </form>

    <h2>入力内容の確認</h2>
    <div id="result"></div>
</body>
</html>

