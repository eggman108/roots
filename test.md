<script type="text/javascript">
<!--
document.write("ブラウザの名前 …… " + navigator.appName + "<br>");
document.write("ブラウザのコード名 …… " + navigator.appCodeName + "<br>");
document.write("ブラウザのバージョン …… " + navigator.appVersion + "<br>");
document.write("プラットフォーム …… " + navigator.platform + "<br>");
document.write("ユーザーエージェント …… " + navigator.userAgent + "<br>");
//-->
</script>

<script type="text/javascript">
<!--
function test() {
  //描画コンテキストの取得
  var canvas = document.getElementById('sample');
  if (canvas.getContext) {
    var context = canvas.getContext('2d');
    //ここに具体的な描画内容を指定する
    //新しいパスを開始する
    context.beginPath();
    //パスの開始座標を指定する
    context.moveTo(100,20);
    //座標を指定してラインを引いていく
    context.lineTo(150,100);
    context.lineTo(50,100);
    //パスを閉じる（最後の座標から開始座標に向けてラインを引く）
    context.closePath();
    //現在のパスを輪郭表示する
    context.stroke();
  }
}
//-->
</script>
