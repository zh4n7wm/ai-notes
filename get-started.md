## 提示工程 (prompt)

- [Prompt Engineering](https://www.kaggle.com/whitepaper-prompt-engineering)
- [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)
   + web version: <https://www.promptingguide.ai/>

## 训练/微调 (Finetune)

- [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory)
- [unsloth](https://github.com/unslothai/unsloth)

## RAG

### 概览

- [【同济大学 王昊奋】Agentic RAG时代：DeepSeek引领推理模型升级下的知识检索增强](https://www.bilibili.com/video/BV1gwXrYMECi)

优化：

- [Seven Failure Points When Engineering a Retrieval Augmented Generation System](https://arxiv.org/abs/2401.05856)

### 开源产品

- [netease-youdao/QAnything](https://github.com/netease-youdao/QAnything)
  + [architecture](https://qanything.ai/docs/architecture)
- [getzep/graphiti](https://github.com/getzep/graphiti)
- [microsoft/PIKE-RAG](https://github.com/microsoft/PIKE-RAG)


### 开源库

- [langchain-ai/langchain](https://github.com/langchain-ai/langchain)
- [run-llama/llama_index](https://github.com/run-llama/llama_index)
- [facebookresearch/faiss](https://github.com/facebookresearch/faiss)
- [deepset-ai/haystack](https://github.com/deepset-ai/haystack)
  + [haystack-cookbook](https://github.com/deepset-ai/haystack-cookbook)
  + [O’Reilly Technical Guide: RAG in Production with Haystack](https://www.deepset.ai/guides/oreilly-guide-rag-in-production-with-haystack)
- [BerriAI/litellm](https://github.com/BerriAI/litellm)

一些使用观点：

- [grok：做 RAG 选用 langchain 还是 haystack？](https://x.com/i/grok/share/hbUNrNPuVq2Pvp3wtR21UxxVJ)
- [why we no longer use LangChain for building our AI agents](https://www.octomind.dev/blog/why-we-no-longer-use-langchain-for-building-our-ai-agents)

#### preprocessing

##### 提取文本

提取文档中的内容是很痛苦、枯燥的事情，参考：

- [Ask HN: What are you using to parse PDFs for RAG?](https://news.ycombinator.com/item?id=41072632)

解析 pdf

- [marker](https://github.com/VikParuchuri/marker) ，**目前测试后效果最好**
- [tika](https://github.com/apache/tika)
- [pymupdf4llm](https://github.com/pymupdf/RAG)
- [mineru](https://github.com/opendatalab/mineru)
- [camelot](https://github.com/camelot-dev/camelot) ，从 pdf 中提取表格
- [Filimoa/open-parse](https://github.com/Filimoa/open-parse/)

##### chunk

- [Five Levels of Chunking Strategies in RAG| Notes from Greg’s Video](https://medium.com/@anuragmishra_27746/five-levels-of-chunking-strategies-in-rag-notes-from-gregs-video-7b735895694d)
- [Enhancing RAG performance with smart chunking strategies](https://developer.ibm.com/articles/awb-enhancing-rag-performance-chunking-strategies/)

### Embedding Models

参考：

- [Xinference Embedding Models](https://inference.readthedocs.io/en/v1.1.0/models/builtin/embedding/index.html)
- [Embedding Leaderboard](https://huggingface.co/spaces/mteb/leaderboard)
- [如何选对Embedding模型？](https://zhuanlan.zhihu.com/p/31981408298)
- [Boosting RAG: Picking the Best Embedding & Reranker models](https://www.llamaindex.ai/blog/boosting-rag-picking-the-best-embedding-reranker-models-42d079022e83)

### 向量数据库

选型：

- [RAG技术实践：从知识库构建到向量数据库选型](https://zhuanlan.zhihu.com/p/25172238481)
  + 推荐的向量数据库：[Milvus](https://github.com/milvus-io/milvus)、[Weaviate](https://github.com/weaviate/weaviate)、[Qdrant](https://github.com/qdrant/qdrant)
- [Comprehensive Guide to Choosing the Right Database for RAG Implementation: Leveraging Elasticsearch, Vector Databases, and Knowledge Graphs](https://medium.com/@sampan090611/comprehensive-guide-to-choosing-the-right-database-for-rag-implementation-leveraging-47e7c6583fdc)

