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

5. myfont.zplをプリンタに送付。

6. プリンタに"E:ANMDJ.TTF"が作成されたことを確認。</br>
　　! U1 do "file.dir" "E"</br>
  　- DIR E:*.* </br>
　　* E:ANMDJ.TTF   8046712  </br>
  
7. ANMDJ.TTFを使用してテスト印字をする。</br>
　 サンプル印刷用ZPL → testPrint_ANMDJ.zpl
  
--------

# Downloadable Files

testPrint_ANMDJ.zpl: サンプル印刷用ZPL</br>
ANMDJ_IPAG.zpl: IPA Gothic をANDMJ.TTFとしてインストールするZPL</br>
ANMDJ_IPAM.zpl: IPA Mincho をANDMJ.TTFとしてインストールするZPL</br>

------

# 免責事項

以下の内容について一切その責任を負いません。あらかじめご了承ください。</br>

1. 本ファイルは利用者の責任において本規約に基づき利用されるものとし、情報配信元は本規約に明示的に定められている場合を除き、本ファイルの利用について責任を負いません。</br>
2. 情報配信元は提供する本ファイルが正常に作動することおよび将来にわたり正常に作動すること、ならびに、本ファイルが全てのプリンタや運用環境において利用できることを保証しません。</br>
3. 本ファイルが正常に作動しないことおよび本ファイルが利用できないことによりお客様が損害を被った場合、情報配信元は当該損害に関して一切責任を負いません。</br>
5. 利用者の本ファイルの利用にあたり、運用データが破壊、消失または変更された場合、情報配信元は一切責任を負いません。</br>
7. 情報配信元は、利用者が本ファイルを通じて得た情報等につき、その正確性および特定の目的への適合性等について、いかなる保証もしません。</br>
7. 情報配信元は、利用者が他の利用者あるいは第三者との間に本ファイルを通じて提供された情報によって生じた権利侵害等の紛争に関して一切責任を負いません。</br>
