# CoalQA RAG

**模块目的：**

 根据用户的问题，检索对应信息以增强回答的专业性, 使CoalQA的回答更加专业可靠。检索内容包括但不限于以下几点：

- 煤矿安全相关的问答对
- 煤矿安全相关的案例

**技术路线：**
这个RAG系统各部分的技术路线分别是：

- Embedding 模型：BCE-Embedding

- LLM基座：InternLM2-Chat-1.8B InternLM2-Chat-7B InternLM2-Chat-20B InternLM2-Math-7B

- 使用BAAI/bge-reranker-large做检索后精排

- 向量数据库：

- - FAISS：是Facebook开源的一个高效的向量相似性搜索库。它为大规模向量检索提供了多种索引结构和搜索算法,能够快速查找与给定向量最相似的向量。FAISS擅长处理超高维度的向量数据,在图像检索、推荐系统等场景有广泛应用。
