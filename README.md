# Fine-Tuning-LLM
Utilize Google Collaboratory to train a pre-trained model on specific datasets like HTML extraction. The tutorial covers data formatting, utilizing LoRA adapters, and integrating the resulting specialized model into Ollama.

# Fine-Tuning an LLM for HTML E-Commerce Data Extraction

This project demonstrates how to fine-tune a large language model (LLM) using **QLoRA (Quantized LoRA)** on HTML e-commerce data to extract structured product information such as title, price, and description.

---

## 🎯 Objective

Train an LLM to:
- Parse raw HTML product pages
- Extract structured product data (title, price, description, features)
- Convert unstructured HTML into clean JSON
- Optionally answer questions about product listings

---

## 📦 Dataset

The dataset consists of e-commerce HTML pages such as:
- Product detail pages
- Product listings
- Category pages

### Example Input (HTML)
```html
<div class="product">
  <h1>Wireless Headphones</h1>
  <span class="price">$49.99</span>
  <p>Noise cancelling Bluetooth headphones</p>
</div>
```
###
```json
{
  "title": "Wireless Headphones",
  "price": "$49.99",
  "description": "Noise cancelling Bluetooth headphones"
}
```

### Instruction:
Extract product details from the HTML.

### Input:
<raw html>

### Output:
<structured json>
