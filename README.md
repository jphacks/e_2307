# BuccalTimer 
## ー クリオネを集めよう！ポモドーロタイマー集中力継続アプリ ー

[![ヘッダー画像](images/BuccalTimer_icon.png)](https://www.youtube.com/watch?v=yYRQEdfGjEg)

## チーム名：be Careful (ビーケアフル)
### チームメンバー
前田 泰一（リーダー・Unityアプリケーション開発），渡邉 珠海（キャラクターデザイン・モデリング・UI），\
多賀 康太（ハードウェア設計・回路設計），パニアグア カルロス（ハードウェア設計・通信設計）\
(奈良先端科学技術大学院大学 [CareLab所属](https://carelab.info/ja/))

# 集中 × Tech
## 製品概要
### 背景（製品開発のきっかけ、課題等）
勉強や作業をしているときにスマホが気になり集中力が途切れることはありませんか？\
作業に集中できるように，クリオネ育成をベースにした**ポモドーロ・テクニック**を活用するアプリケーションを紹介します！\
独自開発した無線マイコンを内蔵の卓上ライトの照明色温度による作業↔集中の切り替えや，スマホの振動機能，オーディオなど様々な技術を用います．

**ポモドーロ・テクニック**：1980年代にイタリア人のフランチェスコ・シリロ（Francesco Cirillo）によって考案された25分の作業と5分ほどの短い休息で作業時間と休息時間を分割する時間管理術．(https://ja.wikipedia.org/wiki/%E3%83%9D%E3%83%A2%E3%83%89%E3%83%BC%E3%83%AD%E3%83%BB%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF)


### 製品説明・使い方
予めアプリをインストールし，専用卓上ライトに内蔵されたM5stack Atom Matrixをスマホと同じWi-Fiアクセスポイントに接続する．（システム図参照）

本アプリでは一旦タイマーを作動させて、スマホの画面を下にして配置する．タイマー初期設定ではポモドーロ・・テクニックが推奨する作業25分，休憩5分に設定されており，ユーザは自由に時間を調整できる．タイマー作動と同時に自動的に卓上ライトの照明が作業に集中力を高める最適な色温度に点灯する．


![説明1](https://github.com/jphacks/KB_2307/assets/136322740/a294aa71-187b-436d-9a66-b3482883aab8)


タイマー作動後，スマホを持ち上げ画面の方を見ようとすると、クリオネが激高し奇声と激しい動きをしながら襲ってくる．卓上ライトの照明も赤色に点灯し，ユーザを作業に戻るよう精神的に誘導する．

![説明2](images/exp2.png)

スマホを再度伏せれば，クリオネが落ち着き，卓上ライト照明も元に戻る．

![説明3](images/exp3.png)

タイマー終了後，卓上ライトの照明がリラックス効果をに最適な色温度に点灯し，休憩時間に入る．この際はスマホは自由に触ることができる．

![説明4](images/exp4.png)

休憩終了後，再度作業タイマーが再開し，照明ももとに戻る．以後終了まで繰り返し．

![説明5](images/exp5.png)

### 特長
- [x] 特長1：必要なものは専用の卓上ライトとスマホアプリだけ！

  - 1.アプリをインストール▶2.専用卓上ライトを電源に接続▶3.同一のWIfiに接続▶完了！！

- [x] 特長2：卓上ライトの照明によるリラックス↔集中の切り替え

  - 集中・リラックス効果を促進する照明温度が実験で証明されている．(https://www.monotaro.com/note/readingseries/shoumei/0505/)
  - リラックス効果：温かみのある色温度（2700〜3000K［ケルビン］）
  - 集中効果：涼しげな色温度（4000〜5000K［ケルビン］）
  - 作業時間と休憩時間にこれらの照明を切り替えていく．
  - 
  - ![特徴2](images/feature1.png)

- [x] 特長3：クリオネ・バッカルコーンによる精神的誘導
  - スマホによる集中力低下を防ぐため，休憩時間外にスマホを持ち上げるとクリオネが激高する．
  - エフェクト，奇声，スマホの振動によりユーザに作業に戻るよう促す．
  - 専用卓上ライトからの赤色照明のフラッシュ効果も発動．
  - 
  - ![特徴3](images/feature2.png)
  
- [x] 特長４：クリオネの育成要素
  - ポモドーロ・テクニック１サイクル（作業25分,休憩5分）を達成するごとにクリオネが水槽に追加される．
  - つまり，作業や勉強に多くの時間を費やすほど，クリオネが増えていき水槽が充実する．
   
   ![特徴4](images/feature3.png)
  
### 解決出来ること
* 学生の普段の自習学習から受験勉強のサポートになる．
* 職場やリモートワークでの作業の生産性向上を図る．
* クリオネ収集をモチベーションとし，勉強や作業の意欲を向上させる．

### 今後の展望
現在はスマホの加速度センサーの情報を元に持ち上げていることを検知しているが，今後AIカメラによる物体検知により勉強や作業に関係のないもの（ゲーム機，漫画，おもちゃ）に触れると同様にアラームを鳴らすことを検討している．

また，室内の二酸化炭素濃度や室内温度によって集中力の低下に影響することが報告されている．（https://diamond.jp/category/s-FukaiShuuChuu/info）
二酸化炭素センサーや温度センサーなど集中力を高める要因を様々なセンサーを用いてユーザの集中力を極限まで向上させる．

### 注力したこと（こだわり等）
* Wi-Fi通信による単純な通信設計
* ユーザの興味をそそるキャラクターモデル
* 卓上ライトの正確な照明温度，明暗調整

## 開発技術
### 活用した技術
#### システム図
![システム図](images/JPHacks2023.png)

#### API・データ
* なし

#### フレームワーク・ライブラリ・モジュール
* iPhone
  * Unity2022
  * C#
* M5stack Atom Matrix
  * Visual Studio Code（Platform IO）
  * C++
  * FastLED Library
* キャラクターデザイン・モデリング，UI
  * Maya
  * Procreate
  * Ilustrator

#### デバイス
* iPhone（ジャイロセンサー，TapticEngine）
* M5stack Atom Matrix
* Adafruit LEDテープ

### 独自技術
#### ハッカソンで開発した独自機能・技術 
* [専用卓上ライトの照明制御プログラム](https://github.com/jphacks/KB_2307/tree/2c56a18d0727cbee86edd5a5a3a852e75043fe98/LEDtape)
* [「buccalTimer」 Unityアプリケーション]()

#### 製品に取り入れた研究内容（データ・ソフトウェアなど）（※アカデミック部門の場合のみ提出必須）
* なし
