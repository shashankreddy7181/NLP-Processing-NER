# NLP-Processing-NER

Student Info

Name: Shashank Reddy Dasari
Student ID: 700781569
Assignment: NLP Tokenization, Lemmatization, POS Filtering & NER

📖 Problem Statement

Perform NLP preprocessing and entity extraction on given input texts.

You must implement:

Q1. Text Preprocessing

Tokenization

Stopword removal

Lemmatization (no stemming)

Keep only verbs and nouns using POS tags

Q2. Named Entity Recognition + Pronoun Ambiguity Detection

Perform Named Entity Recognition (NER)

If the text contains a pronoun ("he", "she", "they"), print a warning

All code must run without spaCy (Python 3.14 incompatible), so the implementation uses NLTK only.

📝 Q1 — Text Preprocessing
Input Text

"John enjoys playing football while Mary loves reading books in the library."

Steps Performed

1️⃣ Tokenized the sentence into word tokens
2️⃣ Removed English stopwords
3️⃣ Applied WordNet lemmatization
4️⃣ Filtered to keep only verbs and nouns
5️⃣ Printed final processed tokens

📝 Q2 — NER + Pronoun Ambiguity Detection
Input Text

"Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch."

Steps Performed

1️⃣ Tokenized the input text
2️⃣ Applied NLTK POS tagging
3️⃣ Performed Named Entity Recognition (PERSON, GPE, ORGANIZATION)
4️⃣ Checked for pronouns (“he”, “she”, “they”)
5️⃣ Printed a warning message if ambiguity detected

📈 Results Summary
✔ Q1 Output

Only nouns and verbs retained after preprocessing.
The pipeline successfully:

removed stopwords

lemmatized tokens

extracted verbs and nouns

✔ Q2 Output

NER detected:

Chris → PERSON

Alex → PERSON

Apple → ORGANIZATION

California → GPE

Pronoun “He” was found →
⚠️ Warning: Possible pronoun ambiguity detected!
