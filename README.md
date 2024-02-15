
# OverView

AI-PaperMiner is a program that simplifies the process of finding academic papers. All you need to do is provide a list of model case papers that represent what you are looking for and specify your search keywords. AI-PaperMiner then automatically retrieves paper information from various databases. Following this, the AI automatically groups the papers, identifying those most relevant to your needs.

# Steps for Usage of AI-PaperMiner for Academic Research

## 1. Data Collection using Findpapers

### Setting Up the Tool
- **Install Findpapers**: Install the Findpapers repository on Google Colab.

### Configuring Your Search
- **Define Search Parameters**: Customize your search by defining queries with relevant keywords and logical operators (AND, OR). Set your desired publication date range, the number of papers you wish to retrieve, and select the databases you want to search.

### Running the Search
- **Execute Findpapers**: With your parameters set, run the Findpapers tool. It will conduct a search across the specified databases and compile the results into a JSON file containing detailed information about each paper.

## 2.2 Exporting Data from JSON to Excel

### Parsing JSON Data
- **Import JSON**: Load the JSON file into your preferred data analysis environment, such as Python with pandas. Extract essential details like titles, publication dates, abstracts, author lists, databases, publishers, journal names, keywords, DOIs, and citation counts.

### Creating an Excel File
- **Compile Data**: Organize the extracted information into a pandas DataFrame. Then, export this DataFrame as an Excel file, which will serve as the basis for further analysis.

## 2.3 Cleaning Abstract Text

### Preprocessing
- **Clean Text**: Apply a predefined function to clean the abstract texts, removing HTML tags, handling missing values, discarding non-English text, and eliminating unnecessary characters and patterns.

### Normalization
- **Standardize Text**: Convert all text to lowercase to ensure uniformity across the dataset.

## 2.4 Generating TF-IDF Feature Matrices

### TF-IDF Transformation
- **Apply TfidfVectorizer**: Use TfidfVectorizer to convert the cleaned abstract texts into a TF-IDF feature matrix, highlighting the importance of words within the documents for analysis.

## 2.5 Determining the Number of Clusters and Clustering

### Elbow Method
- **Optimize Cluster Number**: Utilize the elbow method to find the optimal number of clusters for your dataset by plotting the sum of squared distances against the number of clusters.

### MiniBatchKMeans Clustering
- **Cluster Data**: Implement the MiniBatchKMeans algorithm to efficiently cluster the TF-IDF feature matrix, grouping similar documents together.

### Saving Results
- **Export Clustered Data**: After clustering, save the dataset with assigned cluster labels to an Excel file for convenient access and analysis.

By following these steps, researchers can leverage to streamline the literature collection process, allowing more time for analysis and discovery.
