# YouTubeのハックチュートリアル  
## [EnglishTutorial](/docs/english-README.md)
## 1.テキストグリッチ  
![image](https://user-images.githubusercontent.com/85279289/210968779-fe86b148-33f3-4183-8e26-6eef956441ee.png)
**ステップ1**  
FirefoxとBurpSuiteをダウンロードします  
**ステップ2**  
YouTubeStudioにログインしてください  
※この時、サブアカウントを使うことを推奨します
理由:BAN対策に  
**ステップ3**  
チャンネルのカスタマイズページに飛びます  
**ステップ4**  
"チャンネル登録者向けの動画"を選択します  
**ステップ5**  
BurpSuiteでインターセプトを有効化します  
**ステップ6**  
YouTubeStudioに戻り、
右上の公開ボタンを押します  
**ステップ7**  
BurpSuiteでPOSTをゲットし、  
VideoIDとTitleを探します  
![image](https://user-images.githubusercontent.com/85279289/210966367-187b493e-05b6-49ba-b04f-b7b9349fbd92.png)
**ステップ8**  
"ttitle",""という項目があります  
この中の""を任意にすることでこのバグを使うことができます  
※"title"は変更しないでください  
,のあとの""の中身を書き換えてください  
**ステップ9**  
転送を押し、インターセプトを切ります  
これで完了です  
  
### チュートリアル動画  
https://youtu.be/xBOzAGteGoI  

## 2.メンバーシップ  
**ステップ1**  
メンバーシップ限定にしたい動画で、限定公開を選びます  
※その時にインターセプトをつけてください  
**ステップ2**  
![image](https://github.com/yukkuributti/YouTubeBug/blob/main/screenshot/%E7%84%A1%E9%A1%8C%202023-01-06%2023-27-53.png?raw=true)  
画像の場所にいき、次の内容を付け足します  
```   
"sponsorsOnly":{
"isSponsorsOnly":true
},
```   
画像のようになればOKです  
![image](https://github.com/yukkuributti/YouTubeBug/blob/main/screenshot/%E7%84%A1%E9%A1%8C%202023-01-06%2023-28-07.png?raw=true)  
つけたし終わったら転送をし、インターセプトを切ります  
するとメンバー限定になっているはずです  
