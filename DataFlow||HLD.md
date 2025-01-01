### Data Flow Diagram (Flowchart for Semantic Grouping of Clinical Trials)

#### **High-Level Components:**

1. **User Input**: Query for retrieving similar clinical trials.
2. **Data Ingestion**: Clinical trials dataset (structured and unstructured).
3. **Preprocessing**: Cleaning and preparing data.
4. **Feature Engineering**: Generating multi-modal embeddings.
5. **Model Training**: Learning similarity patterns.
6. **Query Processing**: Comparing user input to dataset.
7. **Explainability Module**: Providing interpretable results.
8. **Result Presentation**: Displaying final output.

---

**Flowchart Steps:**

**Start**
   |
   v
**1. User Input** (Study Title, Primary Outcome, Secondary Outcome, Criteria)  
   |
   v
**2. Data Ingestion**  
   - Load raw dataset from clinicaltrials.gov.
   |
   v
**3. Preprocessing**  
   - Normalize text (remove stopwords, tokenization).
   - Encode structured data (e.g., phases, conditions).
   |
   v
**4. Feature Engineering**  
   - Generate embeddings for textual data (using BioBERT/ClinicalBERT).
   - Combine with structured data features.
   |
   v
**5. Model Training**  
   - Train similarity models (Siamese Networks or Contrastive Learning).
   |
   v
**6. Query Processing**  
   - Embed user query.
   - Perform similarity search (FAISS or cosine similarity).
   |
   v
**7. Explainability Module**  
   - Highlight key features influencing similarity.
   |
   v
**8. Result Presentation**  
   - Display ranked clinical trials with explanations.
   |
   v
**End**
