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
