# mecab-sakedic
mecab用の日本酒辞書です。

* sake.dic ユーザー辞書
* sake_mecab.csv 辞書化する前のCSV

## 使い方
sake.dicを適当なディレクトリに置いて、mecabrcに以下を追加してください
```
userdic = /path/to/sake.dic
```

## Sample

```
$ echo '獺祭と而今と十四代の純米大吟醸を四合瓶で買った' | mecab

獺祭	名詞,固有名詞,一般,*,*,*,だっさい,ダッサイ,ダッサイ
と	助詞,並立助詞,*,*,*,*,と,ト,ト
而今	名詞,一般,*,*,*,*,*
と	助詞,並立助詞,*,*,*,*,と,ト,ト
十四代	名詞,固有名詞,一般,*,*,*,じゅうよんだい,ジュウヨンダイ,ジュウヨンダイ
の	助詞,連体化,*,*,*,*,の,ノ,ノ
純米大吟醸	名詞,固有名詞,一般,*,*,*,じゅんまいだいぎんじょう,ジュンマイダイギンジョウ,ジュンマイダイギンジョウ
を	助詞,格助詞,一般,*,*,*,を,ヲ,ヲ
四合瓶	名詞,固有名詞,一般,*,*,*,しごうびん,シゴウビン,シゴウビン
で	助詞,格助詞,一般,*,*,*,で,デ,デ
買っ	動詞,自立,*,*,五段・ワ行促音便,連用タ接続,買う,カッ,カッ
た	助動詞,*,*,*,特殊・タ,基本形,た,タ,タ
EOS
```
```
$ echo 'カプエチ感があるフルーティーな山田錦や美山錦より濃醇な雄町が好き' | mecab

カプエチ	名詞,固有名詞,一般,*,*,*,かぷえち,カプエチ,カプエチ
感	名詞,接尾,一般,*,*,*,感,カン,カン
が	助詞,格助詞,一般,*,*,*,が,ガ,ガ
ある	動詞,自立,*,*,五段・ラ行,基本形,ある,アル,アル
フルーティー	名詞,形容動詞語幹,*,*,*,*,フルーティー,フルーティー,フルーティー
な	助動詞,*,*,*,特殊・ダ,体言接続,だ,ナ,ナ
山田錦	名詞,固有名詞,一般,*,*,*,やまだにしき,ヤマダニシキ,ヤマダニシキ
や	助詞,並立助詞,*,*,*,*,や,ヤ,ヤ
美山錦	名詞,固有名詞,一般,*,*,*,みやまにしき,ミヤマニシキ,ミヤマニシキ
より	助詞,格助詞,一般,*,*,*,より,ヨリ,ヨリ
濃醇	名詞,固有名詞,一般,*,*,*,のうじゅん,ノウジュン,ノウジュン
な	助動詞,*,*,*,特殊・ダ,体言接続,だ,ナ,ナ
雄町	名詞,固有名詞,一般,*,*,*,おまち,オマチ,オマチ
が	助詞,格助詞,一般,*,*,*,が,ガ,ガ
好き	名詞,形容動詞語幹,*,*,*,*,好き,スキ,スキ
EOS
```

