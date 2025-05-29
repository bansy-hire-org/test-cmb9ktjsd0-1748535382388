# Efficient Document Similarity Scoring

Implement a function to efficiently calculate the similarity score between two documents using TF-IDF and cosine similarity.

## Requirements
Python 3.9+
scikit-learn

## Test Cases
### Test Case 1
- Description: Test case for high similarity between two documents.
- Input: ["This is a test document.", "This is another test document."]
- Expected Output: 0.9

### Test Case 2
- Description: Test case for moderate similarity between two documents.
- Input: ["This is document one.", "This is document two."]
- Expected Output: 0.7

### Test Case 3
- Description: Test case for low similarity between two documents.
- Input: ["Completely unrelated text.", "Another completely unrelated text."]
- Expected Output: 0.0

### Test Case 4
- Description: Test case for handling empty documents.
- Input: [" ", " "]
- Expected Output: 1.0

### Test Case 5
- Description: Test case for handling one empty document.
- Input: ["This is a test.", ""]
- Expected Output: 0.0

### Test Case 6
- Description: Test case for single word documents.
- Input: ["Test", "Test"]
- Expected Output: 1.0

### Test Case 7
- Description: Test case for documents with minor differences.
- Input: ["The quick brown fox jumps over the lazy dog.", "The quick brown fox jumps over the lazy cat."]
- Expected Output: 0.9