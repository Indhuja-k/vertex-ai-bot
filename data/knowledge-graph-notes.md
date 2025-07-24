# 🧠 Knowledge Graph Summary – Insurance Domain

Although a full-blown knowledge graph was not used, this file summarizes the **structured information** used to support prompt grounding.

This information was also embedded in the uploaded context file: `insurance-policy.pdf`.

---

## 📋 Key Entities

| Entity Type     | Example                              |
|------------------|--------------------------------------|
| Policy Name      | Standard Accident Insurance Plan     |
| Coverage         | Accidental death, hospitalization    |
| Exclusions       | Self-injury, intoxication            |
| Claims Process   | Form + documents + call support      |
| Premium Info     | ₹2500/year, optional riders          |
| Duration         | 1 year                               |

---

## 🧩 Use in Vertex AI Studio

- PDF file uploaded as context
- The prompt refers to this structured data when answering questions
- Ensures grounded, reliable responses

---

## 🔁 Future Ideas

- Convert this into a real knowledge graph using Neo4j or RDF format
- Use Google Cloud's Vertex AI + Graph Databases for dynamic retrieval

---

