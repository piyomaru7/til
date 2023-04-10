# ユーザーから入力を受け取る方法
Scannerという仕組みを使う。しかし、Scannerは記述が長くなってしまうのでimportという命令を使う。
```java
import java.util.Scanner;
```
こうするだけで良い。その上でキーボードの入力を受け取るために
```java
new Scanner(System.in).next();
```
と記述する<br>
下記のように変数を定義してあげると入力された値を扱うことができる。変数を定義するには、変数の宣言が必要である。
```java
String name = new Scanner(System.in).next();
```
