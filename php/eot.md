# 長めのテキストを表現する方法
このように<<<EOT,改行,EOT;としてあげると、この中に書いたテキストや改行、字下げは保持されたまま変数$textに代入される<br>
EOTは終端記号と呼ばれていて、好きな名前をつけることが可能。今回はEnd Of TextのEOTとしている。<br>
<<<EOTの後は何も書いてはいけないルールがある。コメントであっても書いてはいけない。
```php
<?php

$text = <<<EOT

EOT;
```
このように、中にテキストを書くことができる
```php
<?php

$text = <<<EOT
hello!
  this is looooong
text!

EOT;

echo $text;
```
また、変数を中に入れることもできる
```php
<?php

$name = 'taguchi';

$text = <<<EOT
hello! $name
  this is looooong
text!

EOT;

echo $text;
```

