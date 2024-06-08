# 3CX の構築

## 前提

- 外線に電話をかけるには、SIP トランクが必要(今回は、**Brastel** を使用)
- 外線に電話、折り返しができるところまでの設定

## 事前準備

まずは、3CX のアカウントを作成(今回は Google アカウントで作成)

[![3CX](./doc/3cx-logo.png)](https://www.3cx.jp/)

## 構築手順

##### **1.** システムを追加をクリック

<p align="center">
    <img src="./doc/0.png" width="500px"/>
</p>

##### **2.** 「3CX Self Hosted / On Premise (PRO / ENT)」をチェックして、Next

<p align="center">
    <img src="./doc/1.png" width="500px"/>
</p>

##### **3.** 「hostname」と「domain」を入力して、Next

<p align="center">
    <img src="./doc/2.png" width="500px"/>
</p>

##### **4.** 「2 Digits」をチェックして、Next

社内のユーザー数に基づいて、内線番号の数を設定

<p align="center">
    <img src="./doc/3.png" width="500px"/>
</p>

##### **5.** 「Country」と「Language」と「Time Zone」と「Prompts」を入力して、Next

<p align="center">
    <img src="./doc/4.png" width="500px"/>
</p>

##### **6.** URL をクリックして、3CX Phone System のインストーラーのダウンロード

> [!WARNING]
> タブを閉じないでください

<p align="center">
    <img src="./doc/5.png" width="500px"/>
</p>

### 以下、3CX Phone System のインストーラーの手順

---

##### **7.** Next

<p align="center">
    <img src="./doc/6.png" width="500px"/>
</p>

##### **8.** Next

<p align="center">
    <img src="./doc/7.png" width="500px"/>
</p>

##### **9.** 許可して、Next

<p align="center">
    <img src="./doc/8.png" width="500px"/>
</p>

##### **10.** Next

<p align="center">
    <img src="./doc/9.png" width="500px"/>
</p>

##### **11.** Install

<p align="center">
    <img src="./doc/10.png" width="500px"/>
</p>

##### **12.** インストールが完了すると、PbxConfigTool.exe が起動されます

<p align="center">
    <img src="./doc/11.png" width="500px"/>
</p>

##### **13.** 「1」を入力

> [!TIP]
> 今回は、ブラウザを使って構築します

<p align="center">
    <img src="./doc/12.png" width="500px"/>
</p>

##### **14.** 開かれたブラウザで「Upload a new configuration file create on 3CX」をチェックして、Next

<p align="center">
    <img src="./doc/13.png" width="500px"/>
</p>

##### **15.** URL Link をチェック

<p align="center">
    <img src="./doc/14.png" width="500px"/>
</p>

##### **16.** 「6. ~~~」で開いていたタブで、Step3 の Download URL をコピー

> [!WARNING]
> タブを閉じないでください

<p align="center">
    <img src="./doc/15.png" width="500px"/>
</p>

##### **17.** コピーした Download URL をコピーして、URL Link にペーストして、Next

<p align="center">
    <img src="./doc/16.png" width="500px"/>
</p>

##### **18.** 構築中なので、待機

<p align="center">
    <img src="./doc/17.png" width="500px"/>
</p>

##### **19.** 構築完了

<p align="center">
    <img src="./doc/18.png" width="500px"/>
</p>

##### **20.** 「6. ~~~」で開いていたタブで、Step4 の URL にアクセス

> [!NOTE]
> Username か Extension と Password をコピー

<p align="center">
    <img src="./doc/19.png" width="500px"/>
</p>

### 以下、3CX Web Client

---

##### **21.** ログイン

<p align="center">
    <img src="./doc/20.png" width="500px"/>
</p>

##### **22.** 3CX Web Client にアクセス完了

<p align="center">
    <img src="./doc/21.png" width="500px"/>
</p>

##### **23.** 鐘マークをクリック

<p align="center">
    <img src="./doc/22.png" width="500px"/>
</p>

##### **24.** ブロックをクリックして、OK

> [!TIP]
> 今回は「Desktop App」を使用するので、ブラウザの通知をさせたくないため、通知をブロックする

<p align="center">
    <img src="./doc/23.png" width="500px"/>
</p>

##### **25.** Admin をクリック

<p align="center">
    <img src="./doc/24.png" width="500px"/>
</p>

##### **26.** M.Console をクリック

<p align="center">
    <img src="./doc/25.png" width="500px"/>
</p>

### 以下、3CX Management Console

---

##### **27.** ログイン

<p align="center">
    <img src="./doc/26.png" width="500px"/>
</p>

##### **28.** 3CX Management Console にアクセス完了

<p align="center">
    <img src="./doc/27.png" width="500px"/>
</p>

##### **29.** SIP Trunks をクリック

<p align="center">
    <img src="./doc/28.png" width="500px"/>
</p>

##### **30.** Add SIP Trunk をクリック

<p align="center">
    <img src="./doc/29.png" width="500px"/>
</p>

##### **31.** 「Select Country」と「Select Provider in your Country」と「Main Trunk No」を入力して、OK

<p align="center">
    <img src="./doc/30.png" width="500px"/>
</p>

##### **32.** 赤枠部分を入力して、OK

<p align="center">
    <img src="./doc/31.png" width="500px"/>
</p>

##### **33.** SIP Trunk 作成完了

<p align="center">
    <img src="./doc/32.png" width="500px"/>
</p>

##### **34.** Inbound Rules をクリック

<p align="center">
    <img src="./doc/33.png" width="500px"/>
</p>

##### **35.** Add DID Rule をクリック

<p align="center">
    <img src="./doc/34.png" width="500px"/>
</p>

##### **36.** 赤枠部分を入力して、OK

<p align="center">
    <img src="./doc/35.png" width="500px"/>
</p>

##### **37.** Inbound Rule 作成完了

<p align="center">
    <img src="./doc/36.png" width="500px"/>
</p>

##### **38.** Outbound Rules をクリック

<p align="center">
    <img src="./doc/37.png" width="500px"/>
</p>

##### **39.** Add をクリック

<p align="center">
    <img src="./doc/38.png" width="500px"/>
</p>

##### **40.** 赤枠部分を入力して、OK

<p align="center">
    <img src="./doc/39.png" width="500px"/>
</p>

##### **41.** Outbound Rule 作成完了

<p align="center">
    <img src="./doc/40.png" width="500px"/>
</p>

### 以下、3CX Web Client

---

##### **42.** Apps をクリック

<p align="center">
    <img src="./doc/41.png" width="500px"/>
</p>

##### **43.** Desktop App をクリック

<p align="center">
    <img src="./doc/42.png" width="500px"/>
</p>

##### **44.** Install をクリック

<p align="center">
    <img src="./doc/43.png" width="500px"/>
</p>

### 以下、3CX Desktop App

---

##### **45.** インストール完了

<p align="center">
    <img src="./doc/44.png" width="500px"/>
</p>

### 以下、3CX Web Client

---

##### **46.** Provision をクリック

<p align="center">
    <img src="./doc/45.png" width="500px"/>
</p>

##### **47.** 「3CX Desktop App を開く」をクリック

<p align="center">
    <img src="./doc/46.png" width="500px"/>
</p>

### 以下、3CX Desktop App

---

##### **48.** 連携されていることを確認

<p align="center">
    <img src="./doc/47.png" width="500px"/>
</p>

##### **49.** 外線に電話をかけられることを確認

<p align="center">
    <img src="./doc/48.png" width="500px"/>
</p>

##### **50.** 折り返しもかけられることを確認

<p align="center">
    <img src="./doc/49.png" width="500px"/>
</p>

外線への電話、折り返しが正常に動作すれば設定完了

> [!TIP]
> 電話がかからない場合、以下を行えばかかるようになることがあります
>
> 1. 再起動をしてください
> 2. 「3CX Management Console」の設定した SIP Trunk の「Authentication」の「Type of Authentication」を「Register/Account based」から「Do not require - IP Based」に変更して保存
> 3. 「3CX Management Console」の設定した SIP Trunk の「Authentication」の「Type of Authentication」を「Do not require - IP Based」から「Register/Account based」に戻して保存

### 3CX Click2Call の設定

---

HTML で「tel 属性」が設定されているところがリンクされるようになり、クリックすると Desktop App が開かれ、リンクされていた電話番号が自動で Desktop App で入力され、すぐに電話することができるようになります

##### **1.** [拡張機能のダウンロード](https://chromewebstore.google.com/detail/3cx-click2call/baipgmmeifmofkcilhccccoipmjccehn?pli=1)

##### **2.** 「Which 3CX App to launch」で「Desktop App」を選択

- 今回は、「Desktop App」 を使用しているので、「Desktop App」 を選択しています
- 「Exception URL list」 は、「3CX Click2Call」 を適用させたくないサイト を「Add」することで無効化させることができます

<p align="center">
    <img src="./doc/50.png" width="500px"/>
</p>

##### **3.** ブラウザで 「tel:080xxxxyyyy」 と入力し、アクセス

「Desktop App」が開かれて正常に動作すれば設定完了

<p align="center">
    <img src="./doc/51.png" width="500px"/>
</p>

### ライセンスが切れてしまった場合

---

ライセンスが切れたシステムを削除し、1 から新しいシステムを構築することで、無料で使い続けることができます
