# **Book Recommendation System**

1. **Problem**

     Design a Recommender System which recommends the best read books to new users 
     and recommends similar books to existing users if they like any particular book 📙.



2. **Dataset**

     The data we're using is from Kaggle's book-recommender dataset.

     https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?select=Books.csv

3. **Information about the data:**

     The data contains 3 datasets 

      **Books.csv**->Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavours (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon web site.

      **Ratings.csv**->Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

      **Users.csv**->Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL-values.

4. 💡**Solution**:
        We apply the **Nearest Neighbour Algorithm** to recommend similar items as those liked by users.
