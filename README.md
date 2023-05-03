# OpenArknightsFBS

本仓库包含了简中版 2.0.01 版本开始使用的 FlatBuffers 二进制数据格式对应的 Schema 文件。

### 共建指南

感谢您为 OpenArknightsFBS 贡献内容，在您编写或修改对应的 FBS 文件前，请阅读以下的共建指南。

- 1.请阅读[FlatBuffers: Grammer of the schema language](https://flatbuffers.dev/flatbuffers_grammar.html)，学习如何编写正确的 FBS 文件。
- 2.在对 FBS 完成编写后，请使用 [FlatBuffers Compiler](https://github.com/google/flatbuffers/releases) `flatc` 对当前版本的最新数据文件使用来验证您编写的 FBS。
```bash
.\flatc.exe --json --raw-binary ".\FBS\chapter_table.fbs" -- .\chapter_table.json --strict-json --natural-utf8
```
- 3.请验证您编写的 FBS 中的字段名和数量是否与官方 JSON 一致。`JsonPropertyAttribute` `JsonIgnoreAttribute`

目前版本(CN 2.0.01)有 15 个数据文件使用 FlatBuffers 格式：

- activity_table
- building_data
- campaign_table
- chapter_table
- character_table
- charword_table
- enemy_database
- handbook_info_table
- medal_table
- open_server_table
- roguelike_topic_table
- sandbox_table
- shop_client_table
- skill_table
- stage_table
