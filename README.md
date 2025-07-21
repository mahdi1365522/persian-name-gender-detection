Persian Name Gender Detection System
A state-of-the-art system for accurate gender detection of Persian names using advanced machine learning, linguistic analysis, and API-powered techniques.
📖 Overview
The Persian Name Gender Detection System is a comprehensive and highly accurate solution designed to predict the gender of Persian names. This project combines three distinct implementations to cater to different needs:  

Ultimate Edition: A self-contained system leveraging ensemble machine learning, deep linguistic analysis, and a built-in database for maximum accuracy without external dependencies.  
Precision Edition: A scientifically validated system focusing on reliability and simplicity, using a comprehensive database and linguistic rules.  
API-Powered Edition: An ultra-precise system that integrates multiple online APIs (NamSor, GenderAPI.io, Genderize.io) with intelligent fallbacks for robust performance.

This project is ideal for researchers, developers, and businesses needing accurate gender detection for Persian names in applications such as data analysis, user profiling, or cultural studies.

🚀 Features

High Accuracy: Achieves 95%+ accuracy for Ultimate and Precision Editions, and up to 98% with API-Powered Edition.  
Comprehensive Database: Includes over 1500 verified Persian names, with continuous learning from user feedback.  
Advanced Linguistic Analysis: Incorporates deep Persian morphological, phonetic, and cultural naming patterns.  
Multiple Implementations: Choose between self-contained (Ultimate/Precision) or API-powered solutions based on your needs.  
Robust Fallbacks: Intelligent fallback mechanisms ensure reliable predictions even when APIs fail.  
Interactive Demos: Built-in interactive testing interfaces for easy evaluation.  
Extensible Design: Easily add new names or integrate additional APIs for enhanced functionality.


🛠️ Installation
Prerequisites

Python 3.8+
Required Python packages:pip install numpy pandas requests sqlite3


For API-Powered Edition, ensure internet access and API keys for NamSor, GenderAPI.io, and Genderize.io (free tiers available).

Setup

Clone the repository:
git clone https://github.com/yourusername/persian-name-gender-detection.git
cd persian-name-gender-detection


Install dependencies:
pip install -r requirements.txt


(Optional) Configure API keys for the API-Powered Edition:

Create a .env file in the root directory.
Add API keys (replace with your own):NAMSOR_API_KEY=your_namsor_api_key
GENDERAPI_IO_KEY=your_genderapi_io_key
GENDERIZE_IO_KEY=your_genderize_io_key




Run any of the three implementations:

Ultimate Edition: python ultimate_persian_gender_detector.py
Precision Edition: python precision_persian_gender_detector.py
API-Powered Edition: python api_powered_gender_detector.py




📚 Usage
Running the Interactive Demos
Each implementation includes an interactive demo for testing. Simply run the respective Python script and follow the prompts:
python ultimate_persian_gender_detector.py

Example output:
🚀 ULTIMATE PERSIAN NAME GENDER DETECTION SYSTEM 🚀
Enter a Persian name (or 'quit' to exit): فاطمه
📊 ANALYSIS RESULTS FOR: فاطمه
👩 Predicted Gender: FEMALE
🎯 Confidence: 95.0% [███████████████████ ]
🔬 Method: Direct Database Lookup
⚡ Processing Time: 12.34 ms

Programmatic Usage
You can integrate the gender detection system into your application:
from precision_persian_gender_detector import PrecisionGenderDetector

detector = PrecisionGenderDetector()
result = detector.predict_gender("مریم", detailed=True)
print(f"Name: {result.name}")
print(f"Gender: {result.predicted_gender}")
print(f"Confidence: {result.confidence:.1%}")
print(f"Explanation: {result.explanation}")


📂 Project Structure
persian-name-gender-detection/
├── ultimate_persian_gender_detector.py   # Ultimate Edition with ensemble ML
├── precision_persian_gender_detector.py  # Precision Edition with linguistic focus
├── api_powered_gender_detector.py        # API-Powered Edition with online APIs
├── data/                                # Database and cached results
│   ├── ultimate_persian_names.db
│   ├── precision_persian_names.db
├── tests/                               # Unit tests for validation
│   ├── test_ultimate.py
│   ├── test_precision.py
│   ├── test_api_powered.py
├── requirements.txt                     # Dependencies
├── README.md                            # Project documentation
└── .gitignore                           # Git ignore file


🧪 Testing
Run the unit tests to verify the system's functionality:
python -m unittest discover tests

The tests cover:

Database integrity and lookup accuracy
Linguistic pattern recognition
API response handling
Edge cases and error scenarios


🤝 Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch: git checkout -b feature/your-feature-name.
Commit your changes: git commit -m 'Add your feature'.
Push to the branch: git push origin feature/your-feature-name.
Submit a pull request.

Please ensure your code follows PEP 8 style guidelines and includes appropriate tests.

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

👨‍💻 Author
Dr. Mahdi Pourabdollah  

Email: mahdi.poorabdollah@gmail.com  
GitHub: [github.com/yourusername ](https://github.com/mahdi1365522) 
LinkedIn: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/dr-mahdi-pourabdollah-89191516b/)


🙏 Acknowledgments

Thanks to the open-source community for providing libraries like NumPy, Pandas, and Requests.
Special appreciation to NamSor, GenderAPI.io, and Genderize.io for their API services.
Inspired by Persian linguistic research and cultural naming conventions.


📬 Contact
For questions, suggestions, or feedback, please open an issue on GitHub or contact the author directly.
