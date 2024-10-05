# **अक्सर पूछे जाने वाले प्रश्न**
- [**अक्सर पूछे जाने वाले प्रश्न**](#अक्सर-पूछे-जाने-वाले-प्रश्न)
- [Python Jupyter Notebooks चलाने के लिए एक विस्तृत गाइड](#python-jupyter-notebooks-चलाने-के-लिए-एक-विस्तृत-गाइड)
  - [Windows के लिए चरण](#windows-के-लिए-चरण)
    - [चरण 1: `pyenv-win` (Python Version Manager) install करें](#चरण-1-pyenv-win-python-version-manager-install-करें)
    - [चरण 2: `pyenv-win` का उपयोग करके एक विशिष्ट Python संस्करण install करें](#चरण-2-pyenv-win-का-उपयोग-करके-एक-विशिष्ट-python-संस्करण-install-करें)
    - [चरण 3: एक वर्चुअल एनवायरनमेंट बनाएं और सक्रिय करें](#चरण-3-एक-वर्चुअल-एनवायरनमेंट-बनाएं-और-सक्रिय-करें)
    - [चरण 4: JupyterLab और मानक library install करें](#चरण-4-jupyterlab-और-मानक-library-install-करें)
    - [चरण 5: ब्राउज़र में JupyterLab चलाएं](#चरण-5-ब्राउज़र-में-jupyterlab-चलाएं)
    - [चरण 6: टर्मिनल से `.py` फ़ाइलें चलाएं](#चरण-6-टर्मिनल-से-py-फ़ाइलें-चलाएं)
  - [Mac के लिए चरण](#mac-के-लिए-चरण)
    - [चरण 1: `pyenv` (Python Version Manager) install करें](#चरण-1-pyenv-python-version-manager-install-करें)
    - [चरण 2: `pyenv` का उपयोग करके एक विशिष्ट Python संस्करण install करें](#चरण-2-pyenv-का-उपयोग-करके-एक-विशिष्ट-python-संस्करण-install-करें)
    - [चरण 3: एक वर्चुअल एनवायरनमेंट बनाएं और सक्रिय करें](#चरण-3-एक-वर्चुअल-एनवायरनमेंट-बनाएं-और-सक्रिय-करें-1)
    - [चरण 4: JupyterLab और मानक library install करें](#चरण-4-jupyterlab-और-मानक-library-install-करें-1)
    - [चरण 5: ब्राउज़र में JupyterLab चलाएं](#चरण-5-ब्राउज़र-में-jupyterlab-चलाएं-1)
    - [चरण 6: टर्मिनल से `.py` फ़ाइलें चलाएं](#चरण-6-टर्मिनल-से-py-फ़ाइलें-चलाएं-1)
  - [Google Colab में नोटबुक चलाना](#google-colab-में-नोटबुक-चलाना)
    - [चरण 1: एक Google खाता बनाएँ](#चरण-1-एक-google-खाता-बनाएँ)
    - [चरण 2: Google Colab तक पहुँचें](#चरण-2-google-colab-तक-पहुँचें)
    - [चरण 3: एक नई नोटबुक बनाएँ](#चरण-3-एक-नई-नोटबुक-बनाएँ)
    - [चरण 4: Colab में डेटासेट आयात करना और उपयोग करना](#चरण-4-colab-में-डेटासेट-आयात-करना-और-उपयोग-करना)
    - [चरण 5: Colab के साथ Google Drive का उपयोग करना](#चरण-5-colab-के-साथ-google-drive-का-उपयोग-करना)
    - [चरण 6: Colab में अतिरिक्त library install करना](#चरण-6-colab-में-अतिरिक्त-library-install-करना)
    - [चरण 7: नोटबुक को सहेजना और साझा करना](#चरण-7-नोटबुक-को-सहेजना-और-साझा-करना)
  - [डेटा स्रोतों और आगे पढ़ने के लिए संदर्भ](#डेटा-स्रोतों-और-आगे-पढ़ने-के-लिए-संदर्भ)
    - [डेटा स्रोत](#डेटा-स्रोत)
    - [आगे पढ़ने के लिए मुफ्त ऑनलाइन पुस्तकें](#आगे-पढ़ने-के-लिए-मुफ्त-ऑनलाइन-पुस्तकें)
    - [कंप्यूटर विज्ञान](#कंप्यूटर-विज्ञान)
  - [FAQ और संभावित समस्याएँ](#faq-और-संभावित-समस्याएँ)
    - [1. प्रश्न: मैं वर्चुअल एनवायरनमेंट को कैसे निष्क्रिय करूँ?](#1-प्रश्न-मैं-वर्चुअल-एनवायरनमेंट-को-कैसे-निष्क्रिय-करूँ)
    - [2. प्रश्न: अगर `pyenv` कमांड मान्यता प्राप्त नहीं हैं तो क्या करें?](#2-प्रश्न-अगर-pyenv-कमांड-मान्यता-प्राप्त-नहीं-हैं-तो-क्या-करें)
    - [3. प्रश्न: अगर JupyterLab स्वचालित रूप से ब्राउज़र में नहीं खुलता है तो क्या करें?](#3-प्रश्न-अगर-jupyterlab-स्वचालित-रूप-से-ब्राउज़र-में-नहीं-खुलता-है-तो-क्या-करें)
    - [4. प्रश्न: बाद में अतिरिक्त library कैसे install करें?](#4-प्रश्न-बाद-में-अतिरिक्त-library-कैसे-install-करें)
    - [5. प्रश्न: मैं एक वर्चुअल एनवायरनमेंट को कैसे हटाऊँ?](#5-प्रश्न-मैं-एक-वर्चुअल-एनवायरनमेंट-को-कैसे-हटाऊँ)
    - [6. प्रश्न: अगर मुझे Mac पर Homebrew install करते समय अनुमति त्रुटियाँ मिलती हैं तो क्या करें?](#6-प्रश्न-अगर-मुझे-mac-पर-homebrew-install-करते-समय-अनुमति-त्रुटियाँ-मिलती-हैं-तो-क्या-करें)
    - [7. प्रश्न: क्यों `pyenv` Mac पर Python संस्करण install नहीं कर रहा है?](#7-प्रश्न-क्यों-pyenv-mac-पर-python-संस्करण-install-नहीं-कर-रहा-है)

---

# Python Jupyter Notebooks चलाने के लिए एक विस्तृत गाइड

यहाँ एक विस्तृत गाइड है जो एक प्रारंभिक व्यक्ति को `pyenv-win` या `pyenv` का उपयोग करके Windows और Mac मशीनों पर Python Jupyter Notebooks चलाने में मदद करेगा, Python संस्करण प्रबंधित करने के लिए, वर्चुअल एनवायरनमेंट के लिए `venv`, और अन्य संबंधित कार्यों के लिए।

## Windows के लिए चरण

### चरण 1: `pyenv-win` (Python Version Manager) install करें
1. **PowerShell को व्यवस्थापक के रूप में खोलें**:
   - `Windows + X` दबाएँ और **Windows PowerShell (Admin)** चुनें।

2. **`pyenv-win` install करें**:
   PowerShell में, निम्नलिखित कमांड चलाएँ:
   ```bash
   Invoke-WebRequest -UseBasicParsing https://pyenv.run | Invoke-Expression
   ```
   स्थापना के बाद, PowerShell को फिर से चालू करें और जाँचें:
   ```bash
   pyenv --version
   ```

### चरण 2: `pyenv-win` का उपयोग करके एक विशिष्ट Python संस्करण install करें
1. उपलब्ध Python संस्करणों की सूची बनाएं:
   ```bash
   pyenv install --list
   ```

2. एक विशिष्ट संस्करण install करें (जैसे, Python 3.10.5):
   ```bash
   pyenv install 3.10.5
   ```

3. वैश्विक Python संस्करण सेट करें:
   ```bash
   pyenv global 3.10.5
   ```

4. Python संस्करण की पुष्टि करें:
   ```bash
   python --version
   ```

### चरण 3: एक वर्चुअल एनवायरनमेंट बनाएं और सक्रिय करें
1. अपने प्रोजेक्ट के लिए एक नई निर्देशिका बनाएं (वैकल्पिक):
   ```bash
   mkdir my_project
   cd my_project
   ```

2. `venv` का उपयोग करके एक वर्चुअल एनवायरनमेंट बनाएं:
   ```bash
   python -m venv venv
   ```

3. वर्चुअल एनवायरनमेंट को सक्रिय करें:
   ```bash
   .\venv\Scripts\activate
   ```

### चरण 4: JupyterLab और मानक library install करें
1. वर्चुअल एनवायरनमेंट में JupyterLab और आवश्यक library install करें:
   ```bash
   pip install jupyterlab numpy pandas matplotlib
   ```

### चरण 5: ब्राउज़र में JupyterLab चलाएं
1. JupyterLab शुरू करें:
   ```bash
   jupyter lab
   ```
   यह स्वचालित रूप से आपके डिफ़ॉल्ट ब्राउज़र में खुल जाएगा।

### चरण 6: टर्मिनल से `.py` फ़ाइलें चलाएं
1. `.py` फ़ाइलें चलाने के लिए टर्मिनल में निम्नलिखित कमांड चलाएँ:
   ```bash
   python my_script.py
   ```

## Mac के लिए चरण

### चरण 1: `pyenv` (Python Version Manager) install करें
1. **Homebrew install करें** (अगर पहले से नहीं किया है):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **`pyenv` install करें**:
   ```bash
   brew install pyenv
   ```

3. **इंस्टॉलेशन की पुष्टि करें**:
   ```bash
   pyenv --version
   ```

### चरण 2: `pyenv` का उपयोग करके एक विशिष्ट Python संस्करण install करें
1. उपलब्ध Python संस्करणों की सूची बनाएं:
   ```bash
   pyenv install --list
   ```

2. एक विशिष्ट संस्करण install करें (जैसे, Python 3.10.5):
   ```bash
   pyenv install 3.10.5
   ```

3. वैश्विक Python संस्करण सेट करें:
   ```bash
   pyenv global 3.10.5
   ```

4. Python संस्करण की पुष्टि करें:
   ```bash
   python --version
   ```

### चरण 3: एक वर्चुअल एनवायरनमेंट बनाएं और सक्रिय करें
1. अपने प्रोजेक्ट के लिए एक नई निर्देशिका बनाएं (वैकल्पिक):
   ```bash
   mkdir my_project
   cd my_project
   ```

2. `venv` का उपयोग करके एक वर्चुअल एनवायरनमेंट बनाएं:
   ```bash
   python -m venv venv
   ```

3. वर्चुअल एनवायरनमेंट को सक्रिय करें:
   ```bash
   source venv/bin/activate
   ```

### चरण 4: JupyterLab और मानक library install करें
1. वर्चुअल एनवायरनमेंट में JupyterLab और आवश्यक library install करें:
   ```bash
   pip install jupyterlab numpy pandas matplotlib
   ```

### चरण 5: ब्राउज़र में JupyterLab चलाएं
1. JupyterLab शुरू करें:
   ```bash
   jupyter lab
   ```
   यह स्वचालित रूप से आपके डिफ़ॉल्ट ब्राउज़र में खुल जाएगा।

### चरण 6: टर्मिनल से `.py` फ़ाइलें चलाएं
1. `.py` फ़ाइलें चलाने के लिए टर्मिनल में निम्नलिखित कमांड चलाएँ:
   ```bash
   python my_script.py
   ```

## Google Colab में नोटबुक चलाना

### चरण 1: एक Google खाता बनाएँ
1. यदि आपके पास पहले से Google खाता नहीं है, तो [यहाँ एक बनाएं](https://accounts.google.com/signup)।

### चरण 2: Google Colab तक पहुँचें
1. [Google Colab](https://colab.research.google.com/) पर जाएँ।

### चरण 3: एक नई नोटबुक बनाएँ
1. "नई नोटबुक" पर क्लिक करें।

### चरण 4: Colab में डेटासेट आयात करना और उपयोग करना
1. फ़ाइलों को अपलोड करने के लिए:
   ```python
   from google.colab import files
   uploaded = files.upload()
   ```

### चरण 5: Colab के साथ Google Drive का उपयोग करना
1. Google Drive को माउंट करें:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

### चरण 6: Colab में अतिरिक्त library install करना
1. अतिरिक्त library install करने के लिए:
   ```python
   !pip install <library_name>
   ```

### चरण 7: नोटबुक को सहेजना और साझा करना
1. अपने नोटबुक को Google Drive में सहेजने के लिए फ़ाइल मेनू पर क्लिक करें और "सहेजें" चुनें।
2. साझा करने के लिए "साझा करें" बटन पर क्लिक करें और लोगों को आमंत्रित करें या एक लिंक प्राप्त करें।

## डेटा स्रोतों और आगे पढ़ने के लिए संदर्भ

### डेटा स्रोत
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [Data.gov](https://www.data.gov/)

### आगे पढ़ने के लिए मुफ्त ऑनलाइन पुस्तकें
- [Python for Data Analysis by Wes McKinney](https://www.oreilly.com/library/view/python-for-data/9781449323592/)
- [Think Python: How to Think Like a Computer Scientist](https://greenteapress.com/wp/think-python-2e/)
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)
- [Python Documentation](https://docs.python.org/3/)
- [W3Schools Python](https://www.w3schools.com/python/)
- [Real Python](https://realpython.com/)

### कंप्यूटर विज्ञान
- [Open Source CS with Python](https://github.com/ForrestKnight/open-source-cs-python)
- [MIT Computer Science](https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA)

## FAQ और संभावित समस्याएँ

### 1. प्रश्न: मैं वर्चुअल एनवायरनमेंट को कैसे निष्क्रिय करूँ?
- निष्क्रिय करने के लिए टर्मिनल में निम्नलिखित कमांड चलाएँ:
  ```bash
  deactivate
  ```

### 2. प्रश्न: अगर `pyenv` कमांड मान्यता प्राप्त नहीं हैं तो क्या करें?
- सुनिश्चित करें कि आपने `pyenv` को सही ढंग से install किया है और आपकी शेल प्रोफ़ाइल फ़ाइल में आवश्यक पथ सेटिंग्स जोड़ी गई हैं।

### 3. प्रश्न: अगर JupyterLab स्वचालित रूप से ब्राउज़र में नहीं खुलता है तो क्या करें?
- अपने टर्मिनल में URL का मैन्युअल रूप से कॉपी और पेस्ट करें जो टर्मिनल पर प्रदर्शित होता है।

### 4. प्रश्न: बाद में अतिरिक्त library कैसे install करें?
- अपने सक्रिय वर्चुअल एनवायरनमेंट में निम्नलिखित कमांड चलाएँ:
  ```bash
  pip install <library_name>
  ```

### 5. प्रश्न: मैं एक वर्चुअल एनवायरनमेंट को कैसे हटाऊँ?
- वर्चुअल एनवायरनमेंट फ़ोल्डर को हटाएँ:
  ```bash
  rm -rf venv
  ```

### 6. प्रश्न: अगर मुझे Mac पर Homebrew install करते समय अनुमति त्रुटियाँ मिलती हैं तो क्या करें?
- `sudo` का उपयोग करके Homebrew को install करने का प्रयास करें, या अपनी फ़ाइल अनुमतियाँ समायोजित करें।

### 7. प्रश्न: क्यों `pyenv` Mac पर Python संस्करण install नहीं कर रहा है?
- सुनिश्चित करें कि आपके पास Xcode Command Line Tools install हैं:
  ```bash
  xcode-select --install
  ```

---
