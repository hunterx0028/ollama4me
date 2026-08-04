步驟 1：安裝必要套件
pip install llama-index llama-index-llms-ollama llama-index-embeddings-ollama chromadb

步驟 2：下載 embedding 模型
ollama pull nomic-embed-text

步驟 3：確認 tree-sitter 的 C# 語法套件
pip install tree-sitter tree-sitter-language-pack



確認安裝成功
python -c "import llama_index; print('llama_index OK')"
python -c "import chromadb; print('chromadb OK')"




