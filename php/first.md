# PHPの書き方
```php
<?php

?>
```
基本的には開始タグと終了タグの間にコードを書いていく。<br>
例外としてPHPファイルの中にHTMLのコードを書かない場合は終了タグは書くべきでないというルールになっているので注意が必要。

# 改行の仕方
```php
<?php

echo 'Hi taro' . PHP_EOL;
echo 'Hello jiro' . PHP_EOL;

?>
```
.PHP_EOLと記述してあげると、環境に応じて適切に改行してくれる。<br>
そして、命令文の終わりには必ず;をつけてあげる。<br>