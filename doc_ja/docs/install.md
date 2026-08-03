# インストール方法

## CUDAインストール

1. 下記をダウンロードし、EXEを実行します。
    - [CUDA 12.8.2](https://developer.nvidia.com/cuda-12-8-2-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local)

## cuDNNインストール

1. 下記をダウンロードし、EXEを実行します。
    - [cuDNN 9.23.2](https://developer.nvidia.com/cudnn-9-23-2-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local)

## 環境変数設定

1. Windowsのスタートメニューを開き、「環境変数」と入力して「システム環境変数の編集」を開きます
2. 画面右下の「環境変数(N)...」ボタンをクリックします
3. 「システム環境変数」の「Path」という変数をという変数を選択し、「編集(I)...」をクリックして下記を追加します。
    - C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.8\bin
    - C:\Program Files\NVIDIA\CUDNN\v9.23\bin\12.9\x64

## プラグインインストール

1. [Fab](https://www.fab.com/listings/a049885e-3929-4626-86c7-d4711b345b29)で購入し、Epic Games Launcherからインストールします。
2. Unreal Engine プロジェクトを作成します。
3. プロジェクトを開き、エディタメニューの「Edit > Plugins」を開き、「Magenta Realtime 2」 を有効にし、プロジェクトを再起動します。
