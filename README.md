# 🏥 Medical Imaging Diagnosis Agent

![Medical Imaging Banner](https://i.imgur.com/JZhVcbX.png)

A powerful AI-powered application for analyzing and diagnosing medical images. This tool leverages Google's Gemini model to provide detailed analysis of various medical imaging formats including X-rays, MRIs, CT scans, and DICOM files.

**⚠️ DISCLAIMER: This tool is for educational and informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of qualified healthcare providers for any medical concerns.**

## 🌟 Features

- **Modern, Intuitive UI**: Clean and professional interface built with Streamlit
- **Multi-format Support**: Handles standard image formats (JPG, PNG) and medical DICOM files
- **AI-Powered Analysis**: Utilizes Google's Gemini 2.0 model for state-of-the-art image interpretation
- **Comprehensive Reports**: Generates structured analysis including:
  - Image Type & Region Identification
  - Detailed Key Findings
  - Diagnostic Assessment with Confidence Levels
  - Patient-Friendly Explanations
  - Research Context with Recent Medical Literature

## 📋 Sample Analysis Output

The analysis provides a structured report with the following sections:

```markdown
### 1. Image Type & Region
- X-ray imaging of the chest, PA (posteroanterior) view
- Good image quality with proper exposure and positioning

### 2. Key Findings
- Clear lung fields without infiltrates or masses
- Normal cardiac silhouette
- No pleural effusions
- Normal bony structures

### 3. Diagnostic Assessment
- Primary: Normal chest radiograph (95% confidence)
- No acute cardiopulmonary process identified

### 4. Patient-Friendly Explanation
Your chest X-ray looks normal. The lungs appear clear without any signs of infection or fluid...

### 5. Research Context
Recent studies on normal chest radiographs:
- [Link to relevant medical literature]
- [Standard protocols for chest X-ray interpretation]
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- Google API Key from [Google AI Studio](https://aistudio.google.com/apikey)

### Step-by-Step Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/medical-image.git
   cd medical-image
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

1. **Start the application**
   ```bash
   streamlit run med.py
   ```

2. **Enter your Google API Key**
   - On first launch, you'll be prompted to enter your Google API Key in the sidebar
   - This key is securely stored in your session state and not shared externally

3. **Upload a medical image**
   - Click the upload button to select an image file
   - Supported formats: JPG, JPEG, PNG, DICOM
   
4. **Get AI Analysis**
   - Click the "Analyze Image" button
   - Wait for the AI to process the image (typically 10-30 seconds)
   - Review the comprehensive analysis report

## 📸 Screenshots

### Application Interface
![App Interface](https://i.imgur.com/JZhVcbX.png)

### Sample Analysis
![Sample Analysis](https://i.imgur.com/JZhVcbX.png)

## 🔒 Privacy & Security

- All image processing happens on your local machine
- API keys are stored only in your session state and not persisted
- No patient data is stored or transmitted beyond what's needed for analysis

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [Streamlit](https://streamlit.io/) for the amazing web app framework
- [Google Gemini](https://deepmind.google/technologies/gemini/) for the AI model
- [Agno AI](https://github.com/agnoai/agno) for the agent framework 