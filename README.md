Vibe Matcher is a mini AI project that recommends fashion products based on a user’s vibe or mood expressed in natural language.
It uses OpenAI text embeddings and cosine similarity to find products with similar semantic meaning, showcasing how AI can personalize user experiences in e-commerce.
Creates a small sample fashion dataset (5–10 products)

 Converts product descriptions into vector embeddings using OpenAI’s text-embedding-ada-002
 Takes a vibe query (e.g., “urban chic”, “boho festival look”)
 Uses cosine similarity to rank the most relevant products
 Displays the top-3 matches with similarity scores
 Handles low-similarity cases with a fallback prompt

Tech Stack:
Language: Python
Libraries: Pandas, Scikit-learn, OpenAI API
Platform: Jupyter / Google Colab
Version Control: Git & GitHub

How It Works:

Prepare mock product data with names, descriptions, and vibe tags.
Generate text embeddings for each description.
Take a user’s vibe input and embed it.
Compare all vectors using cosine similarity.
Return top product matches ranked by score.

Example Query:
Input: "energetic urban chic""
Output:
1 Urban Bomber - 0.867462
2	Sporty Runner	- 0.824866
3	Tailored Blazer	- 0.824502

Reflection
This project demonstrates how AI embeddings can be used for intelligent, vibe-based recommendations.
Future enhancements include integrating with Pinecone vector database and deploying a web interface for real-time results.
