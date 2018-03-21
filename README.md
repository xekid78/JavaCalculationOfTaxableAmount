# JavaCalculationOfTaxableAmount
税込み金額の計算

## 処理
定価6500円の品物を割り引いた金額と税込みの金額の算出と5人で割った一人当たりの金額とその余りを計算します。

## コード
```  
public class Calctax {

	public static void main(String[] args) {

		int price = 6500;
		System.out.println("定価：" + price + "円");

		int discountPrice = (int)(price * 0.85);
		System.out.println("割引価格は、" + discountPrice + "円です。");

		int amount = (int)(discountPrice * 1.08);
		System.out.println("税込み金額は、" + amount + "円です。");

		int person = 5;
		System.out.println("人数が、" + person + "人の場合。");

		int amountPerPerson = amount / person;
		int remainder = amount % person;
		System.out.println("一人当たり" + amountPerPerson + "円、余り" + remainder + "円です。");
	}

}
```  

## 出力結果
```
定価：6500円  
割引価格は、5525円です。  
税込み金額は、5967円です。  
人数が、5人の場合。  
一人当たり1193円、余り2円です。 
```
  
## 開発環境
| 開発ツール |  |
|:-|:-|
| OS | Windows10 |
| 統合開発環境(IDE) | Eclipse 4.7.0 Oxygen |
| 開発言語 | Java8 |
