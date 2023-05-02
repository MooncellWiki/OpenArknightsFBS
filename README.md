# OpenArknightsFBS
本仓库包含了简中版2.0.01版本开始使用的FlatBuffers二进制数据格式对应的Schema文件。  

### 共建指南
感谢您为OpenArknightsFBS贡献内容，在您编写或修改对应的FBS文件前，请阅读以下的共建指南。  
* 1.请阅读[FlatBuffers: Grammer of the schema language](https://flatbuffers.dev/flatbuffers_grammar.html)，学习如何编写正确的FBS文件。  
* 2.在对FBS完成编写后，请使用[FlatBuffers Compiler](https://github.com/google/flatbuffers/releases)```flatc```对当前版本的最新数据文件使用来验证您编写的FBS。  
* 3.请验证您编写的FBS中的字段名和数量是否与官方JSON一致。```JsonPropertyAttribute``` ```JsonIgnoreAttribute```  

目前版本(CN 2.0.01)有15个数据文件使用FlatBuffers格式：
* activity_table
* building_table
* campaign_table
* chapter_table
* character_table
* charword_table
* enemy_database
* handbook_info_table
* medal_table
* open_server_table
* roguelike_topic_table
* sandbox_table
* shop_client_table
* skill_table
* stage_table