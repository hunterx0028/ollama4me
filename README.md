步驟 1：安裝必要套件
pip install llama-index llama-index-llms-ollama llama-index-embeddings-ollama chromadb

步驟 2：下載 embedding 模型
ollama pull nomic-embed-text



確認安裝成功
python -c "import llama_index; print('llama_index OK')"
python -c "import chromadb; print('chromadb OK')"

$env:OLLAMA_API_BASE = "http://localhost:11434"
cd "你的專案路徑"
aider --model ollama/qwen2.5:3b-instruct-q4_K_M --no-git --map-tokens 0 --assistant-output-color "white" --tool-error-color "bright_yellow" --tool-warning-color "bright_yellow"

