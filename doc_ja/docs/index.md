# これは何？

<iframe width="560" height="315" src="https://www.youtube.com/embed/OdqQR27XlQ8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Magenta Realtime 2 Plugin for UE](https://vrlab.akiya-souken.co.jp/products/magentart2plugin/)は、リアルタイムかつインタラクティブに音楽を生成し楽器のように演奏することができる[Magenta Realtime 2](https://magenta.withgoogle.com/mrt2)をUnreal Engine上で実行できるようにするプラグインです。

!!! Info "Magenta Realtime 2 とは？"

    - Googleが開発したローカル環境で動作するリアルタイム音楽生成モデル
    - 複数プロンプトの比率を動的に変えながらブレンドしたり、MIDI入力によって音程を操作したりすることができます

## 本プラグインの特徴

- Windows + NVIDIA GPU向けに最適化
- ゲームスレッドをブロックしないよう、AIの重い処理は専用スレッドで実行
- 各種の操作をC++とBPのどこからでもサブシステム経由で呼び出し可能
- 音声出力はMetaSoundノードとして実装されており、MetaSoundの各種信号処理と簡単に接続可能

!!! Warning "注意"

    - NVIDIA GPU (RTX2000シリーズ以降) が必要です。
    - Magenta Realtime 2のモデルのうち、Smallモデルのみが使用可能です。Baseモデルはサポート外で、本プラグインに含まれていません。
