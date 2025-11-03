# 🚀 Code Summarization and Evaluation Tool (CSET)

**Code Summarization and Evaluation Tool (CSET)** is a full-stack web application designed to enhance **code understanding** and **evaluation** through AI-driven summarization and multilingual translation. Built using **ReactJS**, **Flask**, and **MySQL**, CSET integrates powerful LLMs and APIs to generate meaningful code summaries, support user-specific insights, and deliver a seamless user experience for both developers and administrators.

---

## 🎯 **Overview**

CSET bridges the gap between raw source code and human interpretation by automatically generating concise, natural summaries of code snippets. It empowers users to:

* Quickly comprehend unfamiliar codebases.
* Translate summaries into their preferred languages.
* Provide feedback to continuously refine the model’s performance.
* View detailed usage insights and evaluation metrics through an **Admin Dashboard**.

---

## ⚙️ **Tech Stack**

| Tier                       | Framework / Tool |
| -------------------------- | ---------------- |
| **Frontend**               | ReactJS          |
| **Backend**                | Flask            |
| **Database**               | MySQL            |
| **Code Summarization API** | Gemini PaLM API  |
| **Translation API**        | MyMemory API     |

---

## 🌟 **Key Features**

### 🧠 **AI-Powered Code Summarization**

CSET uses the **Gemini PaLM API** to analyze code logic and produce human-readable summaries:

> “Summarize the following code. It must be natural, useful, and consistent. The summary should explain the logic — not syntax — in concise bullet points.”

### 🌍 **Multilingual Translation**

Using the **MyMemory API**, users can translate generated summaries into their preferred language — making code comprehension globally accessible.

### 👤 **User Categorization**

Upon registration, users specify their domain (e.g., Data Science, Machine Learning, Full Stack Development, etc.), enabling the admin to analyze how the tool performs across professional categories.

### 🛠️ **Admin Dashboard**

Admins can:

* Manage users and administrators.
* View user statistics via graphs and metrics.
* Evaluate summaries based on user feedback.
* Switch to user mode to test summarization functionalities.

### 💻 **User Dashboard**

Users can:

* Paste code snippets or upload files to generate summaries.
* Translate summaries into other languages.
* View and manage their previous summaries.
* Update account credentials easily.

---

## 🧩 **Running the Application**

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/dhaminideva/Code-Summarizer.git
cd Code-Summarizer
```

### 2️⃣ Launch the Frontend

Navigate to the **src** directory and run:

```bash
npm install
npm start
```

Runs on: `http://localhost:3000`

### 3️⃣ Launch the Backend

From the root folder, run:

```bash
python server.py
```

Runs on: `http://localhost:5000`

📝 **Before starting**, ensure your **Gemini PaLM API key** is configured.
Get your key from [Google AI Studio](https://aistudio.google.com/app/apikey).

### 4️⃣ Set Up the Database

Run the provided SQL script in your MySQL instance:

```sql
source DB_script.txt;
```

### 5️⃣ Access the Application

Visit `http://localhost:3000` and sign up or use the default admin credentials:

```
Username: Admin
Password: Admin
```

---

## 🧪 **Testing**

| Type                           | Tool    |
| ------------------------------ | ------- |
| Unit Testing                   | Jest    |
| Integration Testing            | Postman |
| Equivalence (Blackbox) Testing | Manual  |

Refer to `Code_Summarizer_Testing.pdf` for detailed test coverage and outcomes.

---

## 🧱 **Architecture Overview**

* **Frontend:** Built with ReactJS for an interactive, modular, and responsive UI.
* **Backend:** Flask serves RESTful APIs for summarization, translation, and database operations.
* **Database:** MySQL stores user data, summaries, feedback, and analytics.
* **APIs:** Separate LLMs are used for summarization (Gemini PaLM) and translation (MyMemory) to ensure optimized results for each domain.

---

## 💡 **Design Highlights**

* Modular architecture for scalability and maintainability.
* Distinct APIs for translation and summarization to minimize error propagation.
* Domain-based feedback aggregation for targeted improvement.
* Fast and lightweight frontend for real-time interaction.

---

## 📹 **Demo Video**

🎥 Watch the full project walkthrough here:
[**CSET Demo Video**](https://drive.google.com/file/d/1RGKxd95VcAF5jfAb_ZcPxeV2TU8HgqMk/view?usp=sharing)

---

## 🧭 **Future Scope**

* Integrate **user-specific fine-tuning** to adapt summaries based on domain.
* Extend API support to other models like GPT and Claude.
* Enable collaborative summarization and annotation.
* Provide visual comparison between AI-generated and user-edited summaries.

---

## 🏁 **Conclusion**

CSET represents a major step toward AI-assisted code comprehension.
By combining the strengths of Gemini PaLM, MyMemory API, and intuitive dashboards, it empowers developers, educators, and researchers to navigate complex codebases efficiently — one summary at a time.

---

**Developed with ❤️ by Team CSET | UMass Amherst**
