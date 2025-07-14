# 🖼️ Semantic Image Retrieval

This project uses [OpenAI's CLIP](https://openai.com/research/clip) model to semantically search a set of meme images based on a natural language query.

## 📦 Project Structure

- Downloads 5 meme images
- Embeds the memes and search queries using CLIP (ViT-B/32)
- Performs semantic image search based on cosine similarity
- Displays the top matching meme visually and prints the rest of the results

## 🧰 Dependencies

- `openai-clip`
- `torch`
- `PIL`
- `requests`

Dependencies are installed directly in the Colab notebook for easy one-click execution.

## ▶️ How to Use

1. **Run the Notebook in Colab**
2. The following steps are executed:
   - Downloads meme images from FringeCore’s server
   - Loads and preprocesses the CLIP model
   - Embeds all memes once
   - Takes a text query input (e.g., `"girl crying"`)
   - Ranks and displays memes most relevant to the query

## 🔍 Example Query

```python
query = "girl crying"
results = search_images(query)
