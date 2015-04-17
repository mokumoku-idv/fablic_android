# fabric_android

##アカウント作成

1. [公式ページ](https://get.fabric.io/) からアカウントを作成する必要がある  
(登録ボタンを押下後、認証されるまで少し時間がかかることがあるようです)
2. 認証後、会社名やチーム名を入力

##Android Studioに導入

1. 上記の会社名やチーム名を入力後、使用するIDEの選択画面になる
2. 今回はAndroid Studioを選択(プラグインがダウンロードされます)
3. プラグインをインストール
    1. Android Studioを開く
    2. Preferencesを開く
    3. Pluginを選択し、先ほどダウンロードした**Fabric for Android Studio**を選択し、OKを押下
    4. Android Studioを再起動後、Toolbarにfabricアイコンが追加される

##SDKをインストール

1. Android Studioに追加されたfabricアイコンを押下しログインする
2. SDKをインストールするプロジェクトを選択し、インストールするSDKを押下
3. SDKを選択後、インストールが終わると、SDKを使用するために必要なgradleのコードが表示されるので、  
   コピペをするか、Applyボタンを押下し、gradleにコードを埋め込む
4. gradleの変更をSyncする

##アプリ完成後、テスターにアプリを配布

※テスターに配布するには**Crashlytics**をインストールする必要がある  
（インストール方法は上記の"SDKをインストール"を参照）  

1. apkファイルを出力  
    * Build -> Generate Signed APK から作成可能  
    * debug・releaseの選択可能（指示通り進めていくと選択画面が出てくる）  
2. fabricアイコンを押下  
3. 配布するプロジェクトを選択  
4. **Distributions**を選択し、先ほど作成したapkファイルをドラッグ＆ドロップ  
5. 配布する相手のメールアドレスを入力  
6. 配布が完了し、fabricのダッシュボード(ブラウザでfabricにログイン)でテスターのテスト状況やアプリのクラッシュ情報などを確認できる

##テスター

fabricからのメールの「Open Your Device」を押下し、指示どおり進めると、
端末にアプリがダウンロードでき、テストが出来る  
fabricの管理用アプリ？のような「Beta」というアプリも追加される