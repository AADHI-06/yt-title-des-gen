
# 🎯 YouTube Metadata Generator using IBM Watsonx

## 📖 Overview
This project showcases how Generative AI can automate and enhance content creation workflows—specifically, generating YouTube titles, descriptions, and hashtags from video summaries. By leveraging IBM Watsonx's foundation model `meta-llama/llama-3-2-1b-instruct`, we demonstrate how structured prompting can deliver high-quality, SEO-optimized metadata with minimal human input.

## 🎯 Objectives
- Utilize pre-trained generative models for natural language generation tasks.
- Design structured prompts to generate metadata from video summaries.
- Implement a user-friendly, Python-based metadata generator.
- Demonstrate the application of Generative AI in digital marketing.

## ⚙️ Execution and Demonstration
The implementation followed a structured workflow:

- **Model Selection:** Used `meta-llama/llama-3-2-1b-instruct` on IBM Watsonx for its human-like text generation.
- **Prompt Engineering:** Developed domain-specific prompts to generate YouTube titles, descriptions, and hashtags.
- **API Integration:** Integrated IBM Watsonx API with Python for real-time prompt inference.
- **Code Implementation:** Developed a complete Python script to manage credentials, input, and output.
- **Sample Testing:** Demonstrated outputs across domains like History, Finance, and Vlogging.

## 🧠 Prompt Design Strategy
The prompts were designed to instruct the model to output three distinct elements: a title, a long description, and a list of relevant hashtags. The tone was kept neutral and SEO-focused. Examples of prompt templates were tested for multiple domains to ensure generalizability.

## ✅ Testing Strategy
To ensure the solution was both reliable and effective, we followed a well-rounded testing approach focused on performance, accuracy, and user experience.

- **Functional Testing:** Verified proper output format.
- **Input Variety:** Tested with casual, technical, long, and short summaries.
- **Content Accuracy:** Checked semantic relevance between input and output.
- **User Feedback:** Gathered qualitative feedback on output quality.

## 🧪 Types of Testing Conducted
1. **Unit Testing:** Verified credential loading, model connection, and prompt generation.
2. **Integration Testing:** Validated end-to-end script and API communication.
3. **User Testing:** Real users tested the tool using custom summaries.
4. **Performance Testing:** Measured latency for different input lengths.

## 📊 Testing Results

| Test Type          | Result Summary                                              |
|--------------------|-------------------------------------------------------------|
| Functional Testing | Outputs were correctly structured.                          |
| Input Variety      | Handled different tones and lengths effectively.            |
| Accuracy           | Over 90% semantic alignment with the summary input.         |
| User Feedback      | Users found the output relevant and useful.                 |
| Performance        | ~1.4s (short) and ~2.3s (long) average response time.        |

## 🔮 Future Enhancements
1. **User Interface:** Add a web-based UI using Gradio or Streamlit.
2. **Preprocessing Layer:** Integrate summarization for raw transcripts.
3. **Batch Input:** Enable processing of multiple summaries at once.
4. **Customization Options:** Allow tone and audience selection.
5. **Multilingual Support:** Expand to global languages.
6. **Analytics:** Capture user feedback for prompt refinement.

## 📸 Sample Output

**Input Summary:**  
"This video discusses the 2008 financial crisis, exploring the collapse of major institutions and government interventions."

**Generated Metadata:**
- **Title:** The 2008 Financial Crisis Explained: What Really Happened
- **Description:**  
  Discover the causes behind the 2008 global financial meltdown, the collapse of Lehman Brothers, and the U.S. government's rescue strategies that shaped economic recovery.
- **Hashtags:** #Finance #2008Crisis #LehmanBrothers #EconomicHistory

## 🧾 Conclusion
This project demonstrates the practical application of Generative AI in automating YouTube metadata creation. It reduces manual effort, improves efficiency, and serves as a scalable template for AI-driven content tools in marketing, education, and communication.

## 📁 File Structure
- `yt-title-des-gen.ipynb`: Main Jupyter notebook demonstrating API integration and metadata generation
- `README.md`: Project documentation and usage guide

## 🔧 Installation & Setup

```bash
# Clone the repository
git clone https://github.com/your-username/yt-metadata-generator.git

# Navigate to the folder
cd yt-metadata-generator

# Install required packages
pip install -r requirements.txt
```

To use the notebook:
1. Obtain your IBM Cloud API Key.
2. Add the API Key to the credential cell in the notebook.
3. Run the notebook step by step to test or modify prompts.

## 💡 Use Cases
- YouTube Creators and Influencers
- Marketing Teams managing content pipelines
- Educational Institutions publishing video tutorials
- Media Houses optimizing video SEO at scale

## 🚧 Known Limitations
- The model occasionally generates overly generic or promotional descriptions.
- Metadata length may exceed YouTube character limits in some cases.
- Currently supports only English input.

## 🙏 Acknowledgments
- IBM Watsonx Team and Foundation Model API
- Prompt Lab (IBM Prompt Engineering Interface)
- OpenAI for conversational inspiration

## 📬 Contact
For any feedback, suggestions, or collaborations, feel free to connect via GitHub issues.
