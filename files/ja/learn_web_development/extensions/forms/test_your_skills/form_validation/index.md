---
title: "スキルテスト: フォーム検証"
slug: Learn_web_development/Extensions/Forms/Test_your_skills/Form_validation
original_slug: Learn_web_development/Extensions/Forms/Test_your_skills:_Form_validation
l10n:
  sourceCommit: 5b20f5f4265f988f80f513db0e4b35c7e0cd70dc
---

{{learnsidebar}}

このスキルテストの目的は、あなたが[クライアント側のフォーム検証](/ja/docs/Learn_web_development/Extensions/Forms/Form_validation)の記事を理解したかどうかを評価することです。

> [!NOTE]
> このページのインタラクティブエディターや、[CodePen](https://codepen.io/)、[JSFiddle](https://jsfiddle.net/)、[Glitch](https://glitch.com/)などのオンラインエディターで解決策を試すことができます。
>
> 行き詰まった場合は、[コミュニケーションチャンネル](/ja/docs/MDN/Community/Communication_channels)のいずれかに連絡してください。

## フォーム検証 1

この課題では、単純なサポートの問い合わせフォームを提供し、それに検証機能を追加してもらいます。

1. フォームを送信する前に、入力フィールドをすべて入力必須にしてください。
2. 「メールアドレス」と「電話番号」フィールドの型を変更し、ブラウザーが要求するデータに適した、より具体的な検証が適用するようにします。
3. 「ユーザー名」フィールドの要求される長さを 5 文字から 20 文字、「電話番号」フィールドの最大長を 15 文字、「コメント」フィールドの最大長を 200 文字にします。

フォームを送信してみてください。上記の制約が続くまで送信されず、適切なエラーメッセージが表示されるはずです。フォームフィールドが有効か不正かを表示させる単純な CSS を追加することを検討してください。

> [!CALLOUT]
>
> [この課題の開始点をダウンロード](https://github.com/mdn/learning-area/blob/main/html/forms/tasks/form-validation/form-validation1-download.html)すると、自分のエディターやオンラインエディターで取り組むことができます。

## フォーム検証 2

これで前回の課題と同じフォームを取り（必要であれば前回の回答を使用します）、正規表現を使って最初の 3 つのフィールドに固有のパターン検証を追加してください。

1. アプリケーションのユーザー名はすべて、単一の文字、続いてドット、続いて 3 つ以上の文字もしくは数字で構成されます。文字はすべて小文字にしてください。
2. ユーザーのメールアドレスはすべて、1 文字以上の英字（小文字または大文字）または数字の後に "@bigcorp.eu" が続きます。
3. 電話番号フィールドに長さの検証が存在する場合は、それを除去し、10 桁を受け入れられるように設定します。10 桁を連続して入力するか、3 桁、3 桁、4 桁のパターンをスペース、ダッシュ、ドットのいずれかで区切って入力してください。

> [!NOTE]
> 正規表現は実に難しいものですが、絶望しないでください。助けを求めることは恥ずかしいことではありません。[正規表現リファレンス](/ja/docs/Web/JavaScript/Guide/Regular_expressions)や、[Stack Overflow](https://stackoverflow.com/) で検索すれば、これらの質問に答えるのに必要なものはすべて見つかります。

この場合も、フォームフィールドが有効か無効かを表示させる単純な CSS を追加することを検討するとよいでしょう。

> [!CALLOUT]
>
> [この課題の開始点をダウンロード](https://github.com/mdn/learning-area/blob/main/html/forms/tasks/form-validation/form-validation2-download.html)すると、自分のエディターやオンラインエディターで取り組むことができます。

## フォーム検証 3

この最後の課題では、制約検証 API といくつかのフォーム検証属性を使用して、独自のエラーメッセージを提供してください。制約検証 API とフォーム検証属性を使用して、独自の有効性メッセージをプログラムしてください。

1. 入力必須とし、最小 10 文字とします。
2. 入力された値がメールアドレスであるかどうか、十分な長さであるかどうかを調べるイベントリスナーを追加してください。メールアドレスに見えないか、短すぎる場合は、適切なカスタムエラーメッセージをユーザーに提供してください。

> [!CALLOUT]
>
> [この課題の開始点をダウンロード](https://github.com/mdn/learning-area/blob/main/html/forms/tasks/form-validation/form-validation3-download.html)すると、自分のエディターやオンラインエディターで取り組むことができます。
