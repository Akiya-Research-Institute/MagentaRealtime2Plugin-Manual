# 重みの設定

各スロットに設定されたプロンプトの寄与度を重みとして設定します。

![](images/set_weight.png){ loading=lazy }  

set_blend_weight関数でスロットごとの重みを設定できます。

- **Index**: 重みを設定するスロットを指定します（0-5）
- **Weight**: 重み

set_blend_weights関数で全スロットの重みをまとめて設定できます。複数のスロットの重みを変更する場合は、内部での再計算が一度で済むので効率的です。

- **Weights**: 重みの配列。要素のIndexがスロットのIndexに対応します。7個目以降の要素は無視されます。

!!! Info "正規化"
    
    重みは、全スロットの重みの絶対値の合計が1になるよう内部処理で正規化されます。

!!! Info "負の重み"

    このプラグインでは、負の値を重みに設定しても上記の正規化処理が問題なく動作するようにMagenta Realtime 2自体を改造済みです。負の値を設定することでそのスロットがNegativeプロンプトとして働くことが期待されますが、実験的な機能です。

    ??? Info "保存した埋め込み表現の符号を反転"

        UnrealエディタのコンテンツブラウザでMagentaRealtime2SavedEmbeddingアセットを右クリックし「Scripted Asset Actions」から「[ Magenta Realtime 2] Negate Audio Embedding」を実行すると、指定した埋め込み表現の各Float値に-1を掛けて保存します。これにより、負の重みを設定したときと同じ挙動をさせることができます。

        ![](images/negate_asset.png){ loading=lazy }  