## 最長片道経路算出プログラム
最長経路算出用のJupyterNotebookファイル．GoogleColaboratory等の環境で実行可能．  
任意の範囲の路線データが入ったcsvファイルを読み込むことで任意の範囲の最長経路を算出できる．一部の範囲のcsvファイルも公開している．  
  
### 使用方法
1行目に`start,end,kiro,line`，2行目以降は`[駅名1],[駅名2],[営業キロ],[路線名]`の例により記述したcsvファイルのパスを2つ目のコードセルにある`read_csv()`関数の第一引数に指定する．又，2つ目のコードセル22行目の変数nに代入した値に依りn番目に長い経路を算出することができる．  
以上，2つの操作の後実行することで，最長片道経路を求めることができる．  
<span style="color: #ff0000; ">graphillionでグラフを扱う場合は同じ頂点を1度しか通ることができないという性質上，P型やO型となる経路は終着駅の1つ手前の駅までのパスが算出される．その為，n+1番目に長い経路がP型やO型であるとき，算出された経路の終着点と本来の終着点との距離を足したものがn番目に長い経路よりも長くなる可能性がある為，注意が必要である．</span>  
***より詳しい使用方法は今後公開予定である．***  
  
#### 最終更新日
2022.2.24 ( readme.md 更新 )

