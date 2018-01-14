# Unicode → JIS文字集合 異字体変換テーブル

Unicodeに存在する文字を可能な限りJIS文字集合にマッピングする変換テーブルです。

「髙（はしご高）」「﨑（立つ崎）」「⒜」「Ⓐ」「①」「⑴」「㋐」「㈪」「㊙」などの機種依存文字を変換先文字コードの収録内文字へ変換できます。

## マッピングの生成ルール

* unicode.org の[Unicode正規化テーブル](http://unicode.org/Public/10.0.0/ucd/NormalizationTest.txt)にもとづきNFKC正規化を行い、それが変換先文字コードに存在する場合は、そのマッピングを採用する
* [漢字データベースプロジェクト](http://kanji-database.sourceforge.net/)の[異字体データ](https://github.com/cjkvi/cjkvi-variants)にもとづき正字から異字体へ変換を行い、それが変換先文字コードに存在する場合は、そのマッピングを採用する

## 文字コード

* ISO-2022-JP  
unicode.org の[JIS X 0201](http://unicode.org/Public/MAPPINGS/OBSOLETE/EASTASIA/JIS/JIS0201.TXT)および[JIS X 0208](http://unicode.org/Public/MAPPINGS/OBSOLETE/EASTASIA/JIS/JIS0208.TXT)を変換先文字コードとしてマッピングを生成
