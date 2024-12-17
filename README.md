# Intelligent Recommendation Engine Similarity Metrics

![License](https://img.shields.io/github/license/Baci-Ak/repository-name)
![GitHub stars](https://img.shields.io/github/stars/Baci-Ak/Intelligent-Recommendation-Engine-Similarity?style=social)
![GitHub forks](https://img.shields.io/github/forks/Baci-Ak/Intelligent-Recommendation-Engine-Similarity-Metrics?style=social)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Similarity Metrics](#similarity-metrics)
- [Installation](#installation)
- [Usage](#usage)
  - [Modules](#modules)
  - [Examples](#examples)
- [Data Requirements](#data-requirements)
- [Contributing](#contributing)
- [Contact](#contact)

## Overview

In the era of information overload, selecting relevant content from the vast expanse of online data has become increasingly challenging. This repository offers a collection of seven robust similarity metrics designed for intelligent recommendation engines. While originally developed for a book recommendation system, these metrics are versatile and can be adapted for various recommendation applications across different domains.

By leveraging these similarity metrics, developers and data scientists can enhance their recommendation systems, improving user satisfaction and engagement by delivering more personalized and accurate content suggestions.

## Features

- **Seven Similarity Metrics**: Includes Squared Euclidean Distance, Minkowski Distance, Spearman Correlation, Chebyshev Distance, Hamming Distance, Cosine Similarity, and Pearson Correlation.
- **Modular Design**: Organized into three primary modules for data loading, similarity computation, and testing.
- **Easy Integration**: Clone and integrate the metrics into your existing projects with minimal setup.
- **Flexible Usage**: Applicable to user-user, item-item, and user-item similarity computations.
- **Comprehensive Documentation**: Detailed explanations and usage guidelines to facilitate seamless implementation.

## Similarity Metrics

1. **Squared Euclidean Distance**
2. **Minkowski Distance**
3. **Spearman Correlation**
4. **Chebyshev Distance**
5. **Hamming Distance**
6. **Cosine Similarity**
7. **Pearson Correlation**

Each metric is implemented as a separate function within the `similarity_module`, allowing for easy selection and customization based on your specific recommendation needs.

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/Baci-Ak/Intelligent-Recommendation-Engine-Similarity-Metrics.git
cd Intelligent-Recommendation-Engine-Similarity
```

Ensure you have Python 3.6 or higher installed. It's recommended to use a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

*Note: If `requirements.txt` is not provided, ensure you have the necessary libraries such as `numpy`, `pandas`, and `scipy` installed.*

## Usage

### Modules

The repository is organized into three main modules:

1. **load_dataset_module2**: Handles data loading and preprocessing.
2. **similarity_module2**: Contains implementations of the seven similarity metrics.
3. **test_module2**: Provides an interface for testing and interacting with the similarity computations.

### Examples

#### Loading Data

```python
from load_dataset_module import load_user_preferences

user_preferences = load_user_preferences('path/to/Users.csv', 'path/to/Books.csv', 'path/to/Book-Ratings.csv')
```

#### Computing Similarity

```python
from similarity_module import cosine_similarity

user1 = 'UserID_1'
user2 = 'UserID_2'

similarity_score = cosine_similarity(user_preferences, user1, user2)
print(f"Cosine Similarity between {user1} and {user2}: {similarity_score}")
```

#### Running the Test Module

```bash
python test_module.py
```

This will launch an interactive prompt where you can:

- Query similarity between users.
- Query similarity between books.
- Exit the application.

## Data Requirements

Ensure you have the following datasets in the designated folders:

1. **Users.csv**: Contains user information including User-ID, Location, and Age.
2. **Books.csv**: Contains book details such as ISBN, Title, Author, Year of Publication, Publisher, and cover image URLs.
3. **Book-Ratings.csv**: Contains user ratings for books with columns UserId, ISBN, and Rating.

*Example of Book-Ratings.csv:*



![image](https://github.com/user-attachments/assets/5846481b-18a4-44a2-87d6-94f93c7e4204)


## Contributing

Contributions are welcome! Whether it's improving documentation, adding new similarity metrics, or enhancing existing functionalities, your input is valuable.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

Please ensure your code adheres to the project's coding standards and includes relevant tests.


## Contact

For any questions, suggestions, or feedback, please reach out to:

- **Name**: Bassey Akom
- **LinkedIn**: [LINK>>](https://www.linkedin.com/in/basseyakom/)

---

*Happy Coding!*
