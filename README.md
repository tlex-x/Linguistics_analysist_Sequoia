# Linguistic Analysis of French Corpora
Based on the Computational Linguistics program assessment:
https://u-paris.fr/linguistique/en/pre-requisites-for-the-computational-linguistics-program/

## **Part 2: 
- EMEA (European Medicines Agency) data set: French medical/pharmaceutical texts, focusing on word frequency distribution and POS tag ambiguity. Dev file only.
- Conll-U file
- Goal: A dictionary with key: word form, and value: frequency

### **Task 2.1: Simple Frequency-Based Sorting**
- **Goal**: A dictionary with key: word form, and value: frequency. Sort words by decreasing frequency and display the top 100 most frequent words with their occurrence counts
- **Requirements**:
  - Exclude punctuation (PUNCT POS tag)
  - Preserve original case of word forms
  - Use a dictionary to count word occurrences
  - Parse a CoNLL-U formatted file (`emea-fr-dev.conllu`) without using parse().
  - Count word frequencies and display the top 100 words with their counts

**Example result**: The top frequent words are French function words like "de" (541), "la" (229), "à" (218), etc.

---

### **Task 2.2: Computing POS-Category Ambiguity Rates**
- **Goal**: Compute and compare two measures of ambiguity:
  1. **Type-level ambiguity**: Average number of possible POS categories per distinct form (vocabulary level)
  2. **Token-level ambiguity**: Average number of possible POS categories per token occurrence (corpus level)

**Key Steps**:
1. For each word form, track all POS tags it appears with and their counts
2. Calculate how many different POS tags each form has
3. Print ambiguous forms (those with multiple POS tags) sorted by frequency
4. Display each POS category and its count for every ambiguous word

**Example result**: The word "le" appears as DET (198 times) and PRON (1 time), showing it has 2 possible POS categories

---
## Part 3:
- Sequoia dataset
- 
- Goal: 
