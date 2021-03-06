# 「UNIXという考え方」読書メモ

## 第一章

### UNIXの歴史
UNIXを作ったのはAT&Tのケン＝トンプソン。
UNIXが画期的なのはタイムシェアリングシステム。これなしでは今までのUNIXの発展はない。
UNIXはMulitcsというシステムから派生している。
トンプソンは独自で一からシステムを作らず、既存の素晴らしいものに付加価値をつけてさらに良いものを作った。

UNIXは移植性の高さが売り。
しかし初めからその方針ではなかった。
もともとはアセンブリで書かれて始めていた。
しかしB言語で書き直され、そしてそこからデニス＝リッチーがC言語を発明して、使用した。

UNIXの多くの機能はトンプソン以外が実装している。

### タイムシェアリングシステムとは

一つのCPUを時間単位で複数ユーザーで分け合い、単一のコンピューターを複数人で同時に使用できるようにした機能。
メインフレーム時代に活躍して、その後パーソナルコンピューターになってからはプロセスを複数走らせるための手法として、
今もなお活用され続けている。

### UNIXの考え方まとめ

重要度の高いもの

- できるだけ小さい単位にまとめる(Small is Beautiful)
- 1ファンクションには1機能
- 可能な限り早く試作する
- 効率より移植性
- データの移植性(数値データはASCIIフラットファイルに保存する)
- ソフトウェアを梃子として使う
- シェルスクリプトによって梃子の効果と移植性を高める
- 過度の対話インターフェースを避ける(対話インターフェースはユーザーを拘束する)
- 全てのプログラムをフィルタとして設計する

重要度の低いもので面白かったもの

UNIXは詳細なエラーを出さないことを推奨している。

