---
title: トップ
---

# medicalcloud

漢方の古典の原文と現代語訳、正史に残る医療の記録、そして漢方医学の教育や研究のために作ったツールを公開しています。作成と公開は高田英明が行っています。

すべてのリポジトリの一覧は、GitHub の [medicalcloud](https://github.com/medicalcloud) で見ることができます。

## 漢方の古典 原文・現代語訳

漢方医学の基本となる古典を、条文や段落ごとの小さな単位に分け、句読点を付けた原文、資料ごとの異同（校異）、注釈書の注、日本語訳と英訳、解説を組み合わせたものです。

人が読むためだけでなく、LLM（大規模言語モデル）が読みやすいことも目指しました。そのため、1つの単位を1つのファイルにし、ファイルの頭に機械で読める情報を付けています。訳と解説は LLM（Claude）を用いて作成したもので、誤りを含むことがあります。

| 書名 | 内容 | ウェブで読む | データ |
|---|---|---|---|
| 傷寒論 | 宋本（趙開美翻刻本の系統）。成無己の注。全829単位 | [ページ](https://medicalcloud.github.io/shokanron/) | [GitHub](https://github.com/medicalcloud/shokanron) |
| 金匱要略 | 新編金匱要略方論（四部叢刊本）。徐彬の注。全782単位 | [ページ](https://medicalcloud.github.io/kinkiyoryaku/) | [GitHub](https://github.com/medicalcloud/kinkiyoryaku) |
| 黄帝内経 | 素問・霊枢の全篇。張志聡集注など | [ページ](https://medicalcloud.github.io/koteidaikei/) | [GitHub](https://github.com/medicalcloud/koteidaikei) |
| 神農本草経 | 孫星衍の輯本。他の輯本・本草書の条と注釈書。全818単位 | [ページ](https://medicalcloud.github.io/shinnohonzokyo/) | [GitHub](https://github.com/medicalcloud/shinnohonzokyo) |
| 和剤局方 | 太平恵民和剤局方。全1431単位 | [ページ](https://medicalcloud.github.io/wazaikyokuho/) | [GitHub](https://github.com/medicalcloud/wazaikyokuho) |
| 難経 | 王翰林集註本。全81難。集註と滑寿注付き。日本語訳のみ | [ページ](https://medicalcloud.github.io/nangyo/) | [GitHub](https://github.com/medicalcloud/nangyo) |
| 薬徴 | 吉益東洞の著。東大本。全52単位。日本語訳のみ | [ページ](https://medicalcloud.github.io/yakucho/) | [GitHub](https://github.com/medicalcloud/yakucho) |
| 山海経 | 正統道蔵本。全18巻792単位。郭璞注付き。医学書ではなく、本草学の背景資料として。効能の一覧と本草書との対応付き。日本語訳のみ | [ページ](https://medicalcloud.github.io/sengaikyo/) | [GitHub](https://github.com/medicalcloud/sengaikyo) |
| 脾胃論 | 金の李杲（東垣）の著。明の仁寿堂刊本。全105単位。日本語訳のみ | [ページ](https://medicalcloud.github.io/hiiron/) | [GitHub](https://github.com/medicalcloud/hiiron) |
| 内外傷弁惑論 | 金の李杲（東垣）の著。脾胃論の前著。明の仁寿堂刊本。全73単位。日本語訳のみ | [ページ](https://medicalcloud.github.io/naigaishobenwakuron/) | [GitHub](https://github.com/medicalcloud/naigaishobenwakuron) |

## 二十四史の医療の記事

『史記』から『明史』までの中国の二十四の正史から、医療に関わる記事を集め、句読点を付けた原文と日本語訳、解説を付けたものです。医師の伝を集めた「医師列伝集」と、皇帝や官人の病、疫病への対策、薬物の献上など、本紀や列伝に散らばる記事を集めた「医療・疾病・薬物に関連する引用集」の二部からなります。正史に書かれた医学の歴史を閲覧し、検索するための資料です。

- [ウェブで読む](https://medicalcloud.github.io/24shi/)
- [GitHub](https://github.com/medicalcloud/24shi)

## 漢方医学の教育と研究のためのツール

- **[KampoBench](https://github.com/medicalcloud/kampobench)**：日本語の漢方診療の相談で、LLM の能力を評価するためのベンチマークです。OpenAI の HealthBench を土台にしています。74の場面と310の評価基準からなり、LLM が下書きしたものを、複数の漢方専門医が見直して作りました。リポジトリには評価用のコードがあり、データは別に公開しています（[論文（medRxiv）](https://doi.org/10.64898/2026.10.07.26365005)、[データ（Zenodo）](https://doi.org/10.5281/zenodo.23129442)）。
- **[漢方医学問診シミュレータ](https://github.com/medicalcloud/kampo_interview_trainer)**：研修医や医学生が、LLM を患者役にして漢方医学の問診を練習するためのものです。ChatGPT の GPTs と、ほかの LLM で使えるプロンプトがあります。
- **[kampo-formula-lookup](https://github.com/medicalcloud/kampo-formula-lookup)**：漢方処方の構成生薬と分量を、記憶に頼らず一次情報で調べるための、AI エージェント用のスキルです。LLM が処方の構成生薬をそれらしく誤って答えてしまうのを防ぐため、手元のデータを先に引き、無いものだけをウェブで照合させます。

## ライセンスと注意

古典の文はパブリックドメインです。このプロジェクトで新しく作ったもの（句読点、訳、解説など）のライセンスは、それぞれのリポジトリの LICENSE に書いてあります（古典の訳は CC BY-SA 4.0）。いずれの資料も、医療上の判断の根拠にはしないでください。
