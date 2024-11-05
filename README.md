# Rock-Paper-Scissors
This is a beginner-friendly craft kit used at DIY events as a material for hands-on soldering.  
<img src="image\complete.JPEG" width=300>

# じゃんけん判定器キット
- 初級用のはんだ付け教材を想定した電子工作キットです。  
- 地域イベントなどで、電子工作のはんだ付け体験（ハンズオン）に利用できます。  
- 不特定の来場者が短時間の参加で完成できる様、はんだ付け個所を24と少なくしています。  
- 難易度を下げるため、取り付ける部品はタクトスイッチのみとしています。  
- 安価な部品を使用し、コストを下げています。  

## 注意
- プリント基板やはんだには有毒な重金属(鉛など)が含まれています。
    - 工作した後や遊んだ後は、石鹸で手を洗ってください。
    - 小動物などがかじらない様にご注意ください。
    - 廃棄の際は自治体の指定に従ってください。
- 部品やはんだなどの突起物があります。
    - 部品や突起物に衣類を引っ掛けたり怪我をしないようご注意ください。
    - ケースやカバーを作成される場合は、四隅の穴をご利用ください。
- 小さなお子様には特にご注意ください。
    - プリント基板を舐めたりしない様、ご注意ください。
    - コイン電池などを飲み込まない様、ご注意ください。

## 内容物
- プリント基板(74x56mm, タクトスイッチ以外の部品は実装済) x1
- タクトスイッチ 赤 x3, 緑 x3
- コイン電池 CR2032 x1
- 説明書 x1  
※ケースやカバーは、ありません。  
※組み立てには、はんだ、はんだごてを含む工具が必要です。  
<img src="image\included.JPEG" width=300>

## 組み立て
### 1. プリント基板にタクトスイッチ6個を挿入します。
(1) 電池ホルダーを奥側に置いたとき、左側3個が緑、右側3個が赤です。  
<img src="image\1_part.JPEG" width=300>  
(2) タクトスイッチがプリント基板に密着するまでしっかりと挿入します。  
<img src="image\2_put.JPG" width=300>  

### 2. はんだ付けします。  
(1) プリント基板を裏返し、タクトスイッチ6個分24個所全てをはんだ付けします。  
<img src="image\3_solder.JPG" width=300>  

### 3. コイン電池(CR2032)を電池ホルダーに取り付けます。  
(1) コイン電池のプラス(+)を上にします。  
<img src="image\4_cr2032a.JPG" width=300>  
(2) 電池ホルダーの、スライドスイッチに近い方の金具に、コイン電池を差し込み引っ掛けます。  
<img src="image\5_cr2032b.JPG" width=300>  
(3) コイン電池の、電池ホルダーに引っ掛けた反対側を、押し込みます。  
<img src="image\6_cr2032c.JPG" width=300>  

## 遊び方
### 1. 電源を入れます。
(1) スライドスイッチをONの位置にします。オレンジ色が点灯します。  
<img src="image\7_pon.JPG" width=300>  

### 2. じゃんけんをします。
(1) 赤と緑に分かれて遊びます。  
(2) 「じゃんけんポン！」で、赤の人と緑の人が各々「グー」、「チョキ」、「パー」のボタンのどれかを押します。  
(3) 赤色が点灯すれば赤の勝ち、緑色が点灯すれば緑の勝ち、黄色が点灯すれば「あいこ」です。  
<img src="image\8_play.JPG" width=300>  

### 3. 電源を切ります。
(1) 遊び終わったらスライドスイッチをONと反対の位置に戻します。  

## 回路図
- [回路図](./bf-043a_scm.pdf)  
- コイン電池(3V)で動作するよう74HCシリーズを使用し、Vf=2V程度のLEDを選択しています。
- 入手容易で安価なICを使うため、入力ボタンはハイサイドでプルダウン抵抗付きとし、出力もハイサイドで直接LEDを駆動しています。
- 明るさを合わせるため、緑LEDのみ電流制限抵抗を小さくしています。
- タクトスイッチのみ、はんだ付けハンズオン用にスルーホール部品を使用しています。赤色・緑色も選択できました。

## 実装図
- [実装図](./bf-043a_pcb.pdf)  

## 製造データ
- [KiCadデータ(単体)](./V01L02)  
- [製造データ(面付け12枚)](./V01L02/production)  

以上