+++
date = '2025-07-29T11:05:04+09:00'
draft = false
title = 'CourseraのGenerative AI for Everyoneを受講したら非常に勉強になった'
summary = "今からでも生成AIを勉強しようとする全ての人におすすめできるコースでした。"
tags = ["Generative AI",  "Study Log"]
showToc = true
tocOpen = false
+++

## 受講の動機

生成AIやばいですね。仕事やプライベートではchatGPT, Perplexity, Gemini, Cursorなどを使うようになり、また開発案件でOpenAIのAPIを使ったバックエンド開発を経験したりして、ようやく生成AIがいかにゲームチェンジャーであるかを感じました。遅い。

[Coursera](https://www.coursera.org/)の[Generative AI for Everyone](https://www.coursera.org/learn/generative-ai-for-everyone/)を受講する前は、『[Attention is All You Need](https://arxiv.org/abs/1706.03762)』と『[Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)』の論文をしっかりと読んで、GPT2より小さいパラメータで自前のGPTを作ってみたり、理論的な理解と実装をトライしていました。

ただ、生成AIのプロジェクトの実務に対するイメージを具体的に描けるようになる必要があると感じています。

- プロジェクトはどうやって始めて、進めて、評価するのか
- 具体的な事例やケーススタディはどんなものがあるのか
- RAGやFine-tuningの技術的詳細は？またどうプロジェクトで応用されているのか

実際に受講してみて、このような自分の知識のギャップをかなり埋めてくれたと感じています。(このコースにはRAGやFine-tuningの技術的詳細はありません)

受講前に少し勉強や実装をしましたが、そもそも生成AIのことを全然知らないんだと改めて感じ、もっとこの領域が好きになりました。

## CourseraのGenerative AI for Everyoneとは？

Courseraとはオンライン学習のプラットフォームで、いろんな大学のいろんなコースが学べます。受講だけなら無料で、証明書を得るためにはお金が必要っぽいです。

そのコースの1つにGenerative AI for Everyoneがあります。講師は[Andrew Ng](https://ja.wikipedia.org/wiki/%E3%82%A2%E3%83%B3%E3%83%89%E3%83%AA%E3%83%A5%E3%83%BC%E3%83%BB%E3%83%B3)氏ですね。

3週間で終了するコースで、1つ10分くらいビデオ形式の授業を見て進めていきます。全体でも5時間くらい？で結構ライトです。
ちなみにコースを完了した証明書自体にはアカデミアやキャリア的な希少性はあまりないと思いますが、私は7,000円弱を支払い証明書をもらいました。

以下にコースで学ぶことを列挙します。

### Week 1: Introduction to Generative AI

- どうやって生成AIは動いているか
- LLMを思考のパートナーとして使うには
- 生成AIの3つの側面 - Writing, Reading, Chatting
- プロンプトのTips

### Week 2: Generative AI Projects

- ソフトウェアアプリケーションにおける生成AIの使用
- 生成AIプロジェクトのライフサイクル
- 生成AIにかかるコストに対する直感的な捉え方
- Retrieval Augmented Generation(RAG), Fine-tuning, 事前学習
- モデルの選択
- LLMはどう指示に従うか: インストラクションチューニングとReinforcement Learning from Human Feedback(RLHF)
- その他ツールやエージェント
- 生成AIをコーディングする

### Week 3: Generative AI in Business and Society

- Web UIベースのLLMの日々の使い方
- Jobの分析
- 新たなワークフローと機会
- 生成AIのソフトウェアを作るためのチーム
- 部門横断的な自動化の可能性
- AIの懸念
- 汎用人工知能(Artificial General Intelligence, AGI)
- 責任あるAI

## 印象的なとこ

### プロンプト

初めから完璧なプロンプトを目指すことはやめて、アウトプットを毎回見てプロンプトを調整していくというサイクルを回すべし、とありました。言われると当然ですが、複雑なことをプロンプトで表現しようとすると手が止まってしまうことがあって、心に留めておこうと誓いました。

### プロジェクトのライフサイクル

1. プロジェクトのスコープを決める
2. プロトタイプを作成する
3. 社内など内部の組織で評価する
4. デプロイ・モニターする

これらは順番にされるのではなくて、2, 3, 4を行ったり来たり繰り返してプロジェクトを進めていくとありました。生成AIのプロジェクトは成果がどうなるか分からない部分があり、小さく初めて内部での評価と改善を繰り返していくといいとのこと。

### 増強(Augmenting)と自動化(Automating)

生成AIを使ったプロジェクトでは、人間が行うタスクを楽にする増強(Augmenting)と完全に自動化(Automating)するタイプがある。
いきなり自動化するのではなく、増強での運用を続けて自動化しても問題がないか否かを意思決定するとのことでした。

また生成AIを使ったプロジェクトのポテンシャルを、以下の2つの要素で判断することができるとありました。

1. 技術的な実現可能性
2. ビジネスの価値

前者は「AIによって実現できるか」で、まずはweb ベースのツールでプロンプトで試行錯誤してみてタスクを遂行できそうか否かをみて見ましょうとのことです。プロンプトだけでは対応が難しかったらRAG, Fine-tuningなどを検討してみましょう。

後者は人間がタスクを完遂するのにかかっていた時間や費用が減ったり、ビジネス的な価値で評価する指標として重要であると。


## 最後に

私にとっては非常に価値あるコースでした。素晴らしい学習機会をありがとうございます！