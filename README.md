# uBlacklistFilter

Google Chrome用拡張機能 **[uBlocklist](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe)** で利用できるルール

## 使い方

1. [uBlocklist](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe) をインストール
2. [サブスクリプションリンク](https://iorate.github.io/ublacklist/subscribe?name=m2en-uBlacklistFilter&url=https://raw.githubusercontent.com/m2en/uBlacklistFilter/main/list/uBlacklist-m2en.txt) をクリック
3. **追加** をクリック

## ブロック対象になる特徴のサイト

1. プログラミングスクール系の公式サイト
   - 全てのサービスがそうとは限りませんが、個人的に良いようには思っていないためこのルールではブロック対象になります。
   - (JavaScriptには `sum` メソッドがあると言いながらSEO対策したわりには、文章の中身ではメソッド自作して `sum` メソッドだ！と言い張られても困りますよ。TechAcademyさん。)
2. 技術系スパムサイト
   - Stack Overflowなどの回答を機械翻訳してそれをただ生産するだけのサイトです。
   - GitHubに存在するuBlockListのルールでは大抵排除されてるものですね。不愉快極まりないのでこのルールでは勿論ブロック対象です。
3. [なんJ AdGuard部 Wiki](https://wikiwiki.jp/nanj-adguard/)さんがまとめてくださっているスパムサイト全般
   - この方達がまとめているものは基本的にプログラマーには関係ない可能性がありますが、不愉快なのでこのルールでは排除します。さようならね。
4. その他、検索を妨害するサイト

このリポジトリは基本的に自分専用で使っているので、中には普通はブロック対象にならないようなサイトがブロックされている場合がありますが、その場合はForkして自分でカスタマイズするなりしてください。

またこのリポジトリだけでは全てのスパムサイトを排除することは出来ないかもしれないので、[下に私が使用しているルール](#関連ルール)を貼っておきます。ぜひご活用ください。

## コントリビュート

### 新しいサイトを追加する

新しいサイトを追加する場合は [list/uBlacklist-m2en.txt](./list/uBlacklist-m2en.txt) を改行ごとに編集してください。

使える正規表現等は [uBlacklistのドキュメント](https://iorate.github.io/ublacklist/docs/advanced-features) を確認してください。

Issueだけでも結構です。

### サイトのブロックを解除する

「このサイトはブロックする必要はない」と思うサイトがブロックされていた場合は [Issues](https://github.com/m2en/uBlacklistFilter/issues) からブロック解除申請として新規Issueを作成してください。

## 関連ルール

- [ncaq](https://github.com/ncaq)さんがまとめてくださっている [ncaq/uBlacklistRule](https://github.com/ncaq/uBlacklistRule)
  - 関数型プログラミング言語 Haskell でツールを作ったりしてメンテナンスしてくださっているルールです。
  - 更新頻度が高かったり、ちゃんと的を得たブロックをしてくださっています。ご活用ください。
- [arosh](https://github.com/arosh)さんがまとめてくださっている [arosh/ublacklist-stackoverflow-translation](https://github.com/arosh/ublacklist-stackoverflow-translation)
  - Stack Overflowの機械翻訳サイト専用の除外用フィルターです。
- [tats-u](https://github.com/tats-u)さんがまとめてくださっている [tats-u/tech-spam-filter](https://github.com/tats-u/tech-spam-filter)
  - 技術系スパムサイト専用のフィルターです。
  - 現在はアーカイブリポジトリとなり、メンテナンスはされていません。
- [108EAA0A](https://github.com/108EAA0A)さんがまとめてくださっている [108EAA0A/ublacklist-programming-school](https://github.com/108EAA0A/ublacklist-programming-school)
  - プログラミングスクール専用のフィルターです。
- [uBlacklist公式のブロックリストまとめ](https://iorate.github.io/ublacklist/subscriptions)
  - 公式のブロックリストです。
  - [日本語版](https://iorate.github.io/ublacklist/ja/subscriptions)

また、見つけ次第 [m2enのStarリスト "🚫 uBlacklist"](https://github.com/stars/m2en/lists/ublock) にまとめていきます。
