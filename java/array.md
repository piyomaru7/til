# Rubyの配列との違い
Javaの配列は、格納する要素の数を最初に決めておく必要があり、かつ後で要素数を変更することができない<br>
要素を増やす場合はArrayListというリストの一種を使用する<br>
ArrayListは要素の数を変更できる配列のようなもので、ウェブアプリケーションの開発ではよく使用される

# 配列の使い方
```java
int[] scores;
scores = new int[3];

scores[0] = 1;
scores[1] = 5;
scores[2] = 10;

System.out.println(scores[0]);
System.out.println(scores[1]);
System.out.println(scores[2]);
```

このように使う<br>
これを
```java
int[] scores;
scores = new int[3];
```
　　　　　　↓
```java
int[] scores = new int[3];
```
のように一行で書くこともできる
```java
scores[0] = 1;
```
の部分はRubyと似ている<br>
型推論を使用する場合
```java
var scores = new int[3];
```
配列の宣言時に代入する値が確定している場合は以下のように記述を省略することができる
```java
int[] scores = {1, 5, 10};
```
# リストとは
Rubyの配列と似たテータ管理の仕組み
- 要素を順序づけて管理する
- 要素を事後的に追加、削除することができる

# ArrayList
ArraListは「可変長配列」を使用するための仕組み.。可変長配列とは、文字通り長さ（要素数）を変更できる配列のこと
```java
import java.util.ArrayList;

class Main {
  public static void main(String[] args) {
    ArrayList<Integer> scores = new ArrayList<Integer>();

    scores.add(1);
    scores.add(5);
    scores.add(10);
    scores.add(15);

    System.out.println(scores.get(0));
    System.out.println(scores.get(1));
    System.out.println(scores.get(2));
    System.out.println(scores.get(3));
  }
}
```
このコードでは<br>
①ライブラリをインポートする
```java
import java.util.ArrayList;
```
②ArrayListの宣言を行う
```java
ArrayList<Integer> scores = new ArrayList<Integer>();
```
③ArrayListに値を代入する
```java
scores.add(1);
```
④ArrayListから要素を取り出す
```java
scores.get(0)
```
