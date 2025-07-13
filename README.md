🍽️ Restaurant Recommendation System
This project is a content-based restaurant recommendation system that suggests similar restaurants based on user preferences and selected restaurant features using cosine similarity.

📌 Features Used for Recommendations
Cuisine Preferences:

south_indian_or_not

north_indian_or_not

fast_food_or_not

street_food

biryani_or_not

bakery_or_not

Other Features:

average_price

rating

⚙️ How It Works
The dataset is preprocessed using Min-Max Scaling to normalize values.

A cosine similarity matrix is computed between all restaurant feature vectors.

Given a restaurant name, the system finds and recommends the top N most similar restaurants.

🗂️ Dataset
Make sure your CSV file indian_restaurants.csv has at least the following columns:

restaurant_name

location

south_indian_or_not

north_indian_or_not

fast_food_or_not

street_food

biryani_or_not

bakery_or_not

average_price

rating

🐍 Requirements
Install the required Python libraries:

bash
Copy
Edit
pip install pandas scikit-learn
🚀 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/restaurant-recommendation-system.git
cd restaurant-recommendation-system
Place your indian_restaurants.csv in the project folder.

Run the Python script:

python
Copy
Edit
python recommendation.py
Sample usage:

python
Copy
Edit
results = recommend_restaurants_by_name("#BBQ", top_n=5)
print(results)
📦 Output
The system returns a DataFrame with the top similar restaurants:

restaurant_name

location

rating

average_price

✅ Example Result
python-repl
Copy
Edit
  restaurant_name     location    rating   average_price
0      Tandoori Hub      Chennai     4.2           300
1     Andhra Meals     Hyderabad    4.3           250
2     Street Bites     Mumbai       4.0           150
...
✍️ Author
Prasanna Ganesan

📜 License
This project is open source and available under the MIT License.
