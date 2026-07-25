# Movie-Recommendation-System
Content Based Movie Recommendation System using Streamlit
🔗 Movie Recommendation Website
Python Frontend API API

A content-based movie recommendation system that recommends movies based on user preferences using cosine similarity.

Extensively trained the model on a diverse dataset of over 7,500 movies, including a substantial collection of 2,850 Indian regional films.

The Recommendations are made by computing similarity scores for movies using cosine similarity. For each movie tags are created by combining various details like genre of the movie, title, top cast, director and then they are converted to vectors using which similarity matrix is formed. Then for any searched movie the movies with the largest similarity score with it are sorted and then recommended.

System Architecture
System Architecture

How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

image

Similarity Score :
How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

More about Cosine Similarity : Understanding the Math behind Cosine Similarity

How to run the project locally?
Clone or download this repository to your local machine.

cd into the cloned folder.

Install virtual environment python package using command:

pip install virtualenv
Create a virtual environment using command:

python3 -m venv [Enter Folder name]
Activate virtual environment using command:

source [virtual environment name]/bin/activate
Install all the libraries mentioned in the requirements.txt file with the command:

 pip install -r requirements.txt
Install ipykernel using command:

pip install ipykernel
Create a kernel user using command:

ipython kernel install --user --name=[Enter kernel_name]
Get your API key from themoviedb.org

Create a .env file and paste the API key insde the file as follows:

API_KEY = YOUR_API_KEY
Run the file app.py by executing the command:

streamlit run app.py
The streamlit app will locally run on your browser using your default browser or run it manually in any browser using the local url provided in your terminal as follows:

 You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501 (port number can be different) [copy and paste in any browser]
  Network URL: http://192.168.0.103:8501

Hurray! That's it. 🥳
