步驟 1：安裝必要套件
pip install llama-index llama-index-llms-ollama llama-index-embeddings-ollama chromadb

步驟 2：下載 embedding 模型
ollama pull nomic-embed-text



確認安裝成功
python -c "import llama_index; print('llama_index OK')"
python -c "import chromadb; print('chromadb OK')"


python -c "import time,ollama; s=time.time(); r=ollama.embeddings(model='nomic-embed-text', prompt='這是一段測試文字'); print(f'耗時: {time.time()-s:.2f} 秒')"

