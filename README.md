# How to use 3rd party TTF fonts on Zebra Designer 3 
 3rdパーティフォントをZebra Designer 3 で利用する方法

1. Windows PC にZebraNet Bridge Enterprise(以降ZNB)をインストールする。</br>
https://www.zebra.com/ap/en/support-downloads/printer-software/zebranet-bridge-enterprise.html

2. ZNB起動　> メニュー「ツール」> フォント・ウィザード

3. ウィザード画面を下記の通り、設定する。</br>
   インポートするフォント → 任意のTTFフォント</br>
   プリンタ出力先情報 → E:ANDMJ</br>
   フォントのインポート先 → 任意のフォルダ + myfont.zpl</br>

4. プリンタに"E:ANMDJ.TTF"が存在する場合は削除。</br>
   ! U1 do "file.delete" "E:ANMDJ.TTF"

5. myfont.zplをプリンタに送付

6. プリンタに"E:ANMDJ.TTF"が作成されたことを確認。</br>
　　! U1 do "file.dir" "E"</br>
  　- DIR E:*.* </br>
　　* E:ANMDJ.TTF   8046712  </br>
  
7. ANMDJ.TTFを使用してテスト印字をする。</br>
　 サンプル印刷用ZPL → testPrint_ANMDJ.zpl
  
   
