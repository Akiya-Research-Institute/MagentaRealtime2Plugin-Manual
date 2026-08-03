# パッケージのビルド

Magenta Realtime 2プラグインを使用したプロジェクトをビルドしてパッケージを作成するには、AIモデルのアセットをパッケージに含むようにアセットマネージャーを設定する必要があります。

## アセットマネージャー設定方法

「Project Settings > Game > Asset Manager > Primary Asset Types to Scan」に要素を追加し、下記の値を設定します。  
または、デフォルトでIndex=1に既に「PrimaryAssetLabel」が設定されているので、この要素を編集してもOKです。

1. **Primary Asset Types**を「PrimaryAssetLabel」に設定します。
1. **Asset Base Class**を「PrimaryAssetLabel」に設定します。
1. **Is Editor Only**をオフにします。
1. **Specific Assets**に要素を追加し「MagentaRealtime2_AudioGeneration_FP16」を指定します。

!!! Info "[32-bit float](../performance/#fp16fp32)を用いる場合"
    「MagentaRealtime2_AudioGeneration_**FP16**」ではなく、「MagentaRealtime2_AudioGeneration_**FP32**」を指定します。

!!! Info "[状態を音声から設定](../state/#_4)する機能を用いる場合"
    **Specific Assets**にさらに要素を追加し「MagentaRealtime2_Prefill」を指定します。
