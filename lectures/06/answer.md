# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：glossary_search_glossary
- STEP 2 の [tool call]：[tool call]   glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：[tool call]   fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：[tool call]   aws_aws___search_documentation({'topics': ['general'], 'search_phrase': 'Amazon S3 versioning overview'})
- 気づき・疑問：awsのmcpは問い合わせの内容に応じて動的にawsのtoolが選ばれるようだ。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎
- やったこと：toolに定義済みのget_lecture_summaryをmcpで呼び出せるようにした
- 結果：[tool call]   glossary_get_lecture_summary({'lecture': 2})
- 気づき・疑問：明示的にツールを指定せずともmcpで正しくツールが選択された。descriptionがきちんと書かれていたからだろう。
