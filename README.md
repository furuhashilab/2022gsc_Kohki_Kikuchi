# 2022gsc_Kohki_Kikuchi
菊池洸希の2022年度ゼミ論用レポジトリ
# 【2022年度ゼミ論】「Mapbox GL JS」Style Specificationの日本語訳作成と図式化
地球社会共生学部　地球社会共生学科　4年A組89番  

学籍番号：1A119059  　氏名：菊池洸希 

指導教員：古橋 大地教授   

©︎Furuhashi Laboratory/Kikuchi Kohki, CC BY 4.0

## 概要  
本研究では、「Mapbox GL JS Style Specification - Layers」の日本語訳を作成し、その概要を図式化した。

## Introduction
　1970年代、四分木（Quadtree)というデータ構造が生まれてから今日に至るまでデジタルマップは進化を続けてきた。2000年代にはタイル技術が生まれ、2005年にGoogleがラスターピラミッドの機能を持ったラスタータイルマップの完成版であるGoogleマップをリリースした。2006年、ブラウザで地図データを表示するためのJavaScriptライブラリであるOpenLayersがリリース。ライブラリを非公開にしているGoogleマップに対して、OpenLayersはオープンソースであった。さらに2011年には、これらに並んで広く使われているLeafletがVladimir Agafonkin氏によって開発される。Vladimir Agafonkin氏が2013年にMapboxに加入すると、翌年にベクタータイルマップに対応したオープンソースライブラリである「Mapbox GL JS」をリリースした。これは2020年に行われたv2.0への移行によって独自ライセンス化するが、この件に批判的なユーザー達が同年、MapboxGLエコシステムのフォークであるMapLibreを開始した。こうしてデジタル地図は進化を続け、現在では非常に速く、軽量で、自由な地図開発が可能になっている。しかし、地図開発において重要なドキュメントの多くは日本語対応していないのが現状である。今後、日本でより多くの人が地図開発を行えるようにこれらのドキュメントを日本語に翻訳していく必要がある。また、地図開発の学習を始める上で、ドキュメントの構造が図式化されているとより理解が深まるが、まだドキュメントの図式化は進んでいない。本研究では、国土地理院が開発している「地理院地図Vector（仮称）」にも採用されている「Mapbox GL JS」のStyle Specificationで特に重要な項目であるLayersの日本語訳を作成し、その概要を図式化した。

## Methods　　

本研究で行うことは以下の2つである。
  
### ①「Mapbox GL JS Style Specification - Layers」の日本語訳の作成

Githubレポジトリ[「StyleSpecification4mapbox」](https://github.com/furuhashilab/StyleSpecification4mapbox)内に、「Mapbox GL JS Style Specification[^1] - Layers」の日本語訳をMarkdown形式で作成する。留意点は以下の通り。
[^1]:Mapox. “Mapbox GL JS Style Specification”. Mapbox Docs. 2022-1-6. https://docs.mapbox.com/mapbox-gl-js/style-spec/, (参照 2022-2-3).

- 作業効率化のため、基本的にGoogle Chromeのページ翻訳ツールを利用する。翻訳結果に異常があった場合は、Google翻訳を使って正しい日本語訳を作成する。

<img width="70%" alt="mb_ss_j_miss" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_j_miss.png">

<img width="70%" alt="gt_01" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/gt_01.png">

- 各タイトルやワードには原文と同様のリンクを付け、Mapboxのページに移動できるようにする。

<img width="70%" alt="mb_ss_j_link" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_j_link.png">

- 列挙型で用いられる"visible"や"none"のようなワード、ブルー値で用いられる"true"と"false"、文字列の配列で用いられる"visible"や "none"等のワードは開発の際にそのまま使用することを考慮し、原文の通りに記載する。

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_j_word.png">

- 日本語に適当な言葉がない場合は、固有名詞か否かによって翻訳が異なる。固有名詞の場合は原文のまま英語表記を用いる。一般名詞の場合はカタカナ表記を用いる。

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_j_words.png">

- 開発時にコードとして書き込むワードにはバッククォート機能を用いる。

<img width="70%" alt="mb_ss_j_word" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_j_back.png">

### ②「Mapbox GL JS Style Specification - Layers」の図式化

図式化の取り組みとしては、以下の２つである。

- 「UML 2 クラス図の概要[^2]」を参照し、UMLクラス図の形式に則り、「Mapbox GL JS Style Specification - Layers」の図式化を行う。図の作成にはChatGPTを利用する。正式な形式に近づけるため、図は英語表記にする。
[^2]:Scott W. Ambler. “UML 2 クラス図の概要”. アジャイルモデリング(AM) 公式サイト. 2003. https://www.ogis-ri.co.jp/otc/swec/process/am-res/am/artifacts/classDiagram.html#DesignClassDiagrams, (参照 2022-2-3).

- より視覚的に理解を促すため、グラフィックレコーディング形式で図式化を行う。図の作成には、手書き・ibisPaintX を併用する。こちらは日本語訳のリポジトリを読む際に補助的な役割を果たすため、日本語で制作する。

## Results　　

Githubレポジトリ　[StyleSpecification4mapbox/Layers](https://github.com/furuhashilab/StyleSpecification4mapbox/blob/fd5ef5c7cfc9304c7b704431d6ab746eb0ad68a5/Layers.md)

<img alt="qr_StyleSpecification4mapbox:Layers" src="https://github.com/furuhashilab/2021gsc_Kohki_Kikuchi/blob/9d1cab7154cf27f8b7dba5427592b587fa7a98a4/qr_StyleSpecification4mapbox:Layers.png">

UMLクラス図

```mermaid
%%{init:{'theme':'base'}}%%
classDiagram
  class Style {
    +layers: Layer[]
    +sources: Source[]
    +zoom: number
    +center: number[]
    +bearing: number
    +pitch: number
    +light: Light
    +sprite: string
    +glyphs: string
  }
  class Layer {
    +id: string
    +type: string
    +source: string
    +source-layer: string
    +minzoom: number
    +maxzoom: number
    +filter: any[]
    +layout: Layout
    +paint: Paint
  }
  class Source {
    +type: string
    +url: string
    +tiles: string[]
    +tileSize: number
    +bounds: number[]
    +coordinateTransform: function
  }
  class Layout {
    // specific layout properties depend on layer type
  }
  class Paint {
    // specific paint properties depend on layer type
  }
  class Light {
    +anchor: string
    +color: string
    +intensity: number
  }
  Style "1" -- "*" Layer
  Layer "0..*" -- "1" Source
  Layer "0..*" -- "1" Layout
  Layer "0..*" -- "1" Paint
  ```
  
グラフィックレコーディング

<img width="80%" alt="uml_layers_01" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/mb_ss_layers_gr.PNG">

## Discussion

### 日本語訳について
本研究によってドキュメントの翻訳ルールを整理することができた。以後、「Mapbox GL JS Style Specification」の他項目の翻訳を行う際は本研究に目を通すことで、速やかかつ正確な翻訳を作成できる。また、本研究を先行事例とし、他の地図開発に関係するドキュメントの日本語化が進むことが望ましい。

### UML図について
ChatGPTは自然言語処理モデルであるため、不確実な側面も否定できないが、本研究で生み出された図は正確なものであった。また、こうしたドキュメントに関係する図は互換性の観点からMarkdown記法に展開可能なMermaidを利用することを推奨する。

### グラフィックレコーディングについて
ドキュメントにグラフィックレコーディングを用いることで、視覚的に内容を伝えることができ、読者の理解を深めることができる。全ての内容を記載すると情報過多になるため、目次としての活用が望ましい。一方で、ドキュメントを提供している公式のページにこうした視覚的な情報を載せることは難しい。

## Conclusion　　　

今後の課題としては、以下の２つが挙げられる。　　      
- 「Mapbox GL JS Style Specification」全項目の日本語訳作成
- 「Mapbox GL JS Style Specification」各項目の図式化、グラフィックレコーディング作成

デジタル地図に関するドキュメントの日本語訳はまだ少ないが、今後日本国内で独自の地図開発が広がると、ドキュメントの日本語訳の需要は高まる。しかし各ドキュメントが独自の翻訳ルールで作成していてはユーザーにとっては理解し難くなる。本研究をさらに進めることでそうしたユーザーのサポートができる。さらにオープンソース等が図式化されていくことでユーザーの理解が深まり、より発展的な活用が期待できる。

## Acknowledgements
本研究を進めるにあたり地球社会共生学部の古橋大地教授をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## グラレコ

<img width="80%" alt="uml_layers_01" src="https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi/blob/main/image/2022_gr.PNG">

## 昨年度資料
**Githubレポジトリ**  
https://github.com/furuhashilab/2022gsc_Kohki_Kikuchi  
**進捗管理用プロジェクト**  
https://github.com/orgs/furuhashilab/projects/27/views/1  
**最終プレゼン資料**  
https://docs.google.com/presentation/d/13QyPYV9XP0rMW9lBEhvvMw2V1saTevBbOVW-3ukvOms/edit?usp=sharing    
**参考文献リスト**   
https://docs.google.com/spreadsheets/d/1LZPnsnPRdWjBaV5Ot01X83DJXEIk3v2-w4xsitTto2E/edit#gid=0　  
**「Mapbox GL JS Style Specification」日本語版　Githubレポジトリ**  
https://github.com/furuhashilab/StyleSpecification4mapbox/blob/ed5cd80c0f0872f9057f81ea1e251339c9d272d4/Layers.md  
**Medium**  
https://medium.com/furuhashilab/2021%E5%B9%B4%E5%BA%A6%E3%82%BC%E3%83%9F%E8%AB%96-mapbox-gl-js-style-specification%E3%81%AE%E6%97%A5%E6%9C%AC%E8%AA%9E%E8%A8%B3%E4%BD%9C%E6%88%90%E3%81%A8%E5%9B%B3%E5%BC%8F%E5%8C%96-5ad5afb1557d
