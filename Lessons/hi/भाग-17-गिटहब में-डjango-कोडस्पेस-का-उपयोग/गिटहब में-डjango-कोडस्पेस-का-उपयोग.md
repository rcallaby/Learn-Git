# सामग्री की तालिका
- [GitHub में Django Codespaces](#django-codespaces-in-github)
  - [अनुभाग 1: GitHub Codespaces क्या हैं?](#section-1-what-are-github-codespaces)
  - [अनुभाग 2: आवश्यकताएँ](#section-2-prerequisites)
  - [अनुभाग 3: Django के लिए एक Codespace बनाना](#section-3-creating-a-codespace-for-django)
  - [अनुभाग 4: Django Codespaces में विकास](#section-4-developing-in-django-codespaces)
  - [अनुभाग 5: ऑफ़लाइन कार्य करना](#section-5-working-offline)
- [निष्कर्ष](#conclusion)
- [GitHub Actions Django Codespaces में](#github-actions-in-django-codespaces)
  - [निरंतर एकीकरण (CI)](#continuous-integration-ci)
  - [स्टेजिंग या प्रोडक्शन में तैनाती](#deploy-to-staging-or-production)
  - [अनुसूचित कार्य](#scheduled-tasks)

# GitHub में Django Codespaces

GitHub Codespaces एक शक्तिशाली क्लाउड-आधारित विकास वातावरण है जो डेवलपर्स को अपने ब्राउज़र में सीधे एप्लिकेशन कोड, निर्माण, और परीक्षण करने की अनुमति देता है। यह स्थानीय विकास सेटअप की आवश्यकता को समाप्त करके एक कुशल और सहज कोडिंग अनुभव प्रदान करता है। यह लेख आपको GitHub में Django Codespaces को सेटअप और उपयोग करने की प्रक्रिया के माध्यम से ले जाएगा, जिससे आप आसानी से और सुविधाजनक तरीके से Django एप्लिकेशन विकसित कर सकते हैं।

### अनुभाग 1: GitHub Codespaces क्या हैं?
GitHub Codespaces एक ऐसा फ़ीचर है जो डेवलपर्स को क्लाउड में एक पूरी तरह से कॉन्फ़िगर किया हुआ विकास वातावरण बनाने की अनुमति देता है। यह Visual Studio Code के परिचित इंटरफ़ेस और सुविधाओं का लाभ उठाता है, जिससे डेवलपर्स के लिए उनके स्थानीय विकास वातावरण से क्लाउड में संक्रमण करना आसान हो जाता है।

### अनुभाग 2: आवश्यकताएँ
GitHub में Django Codespaces का उपयोग करने के लिए, आपको निम्नलिखित की आवश्यकता होगी:

GitHub खाता: GitHub Codespaces तक पहुँचने के लिए आपके पास एक GitHub खाता होना चाहिए।
Django प्रोजेक्ट: आपके पास GitHub पर होस्ट किया गया एक Django प्रोजेक्ट रिपॉजिटरी होनी चाहिए, जिस पर आप क्लाउड में काम करना चाहते हैं।

### अनुभाग 3: Django के लिए एक Codespace बनाना
अपने Django प्रोजेक्ट के लिए एक Codespace बनाने के लिए निम्नलिखित चरणों का पालन करें:

चरण 1: अपने GitHub रिपॉजिटरी पर जाएँ।
GitHub पर अपने Django प्रोजेक्ट रिपॉजिटरी पर जाएँ।

चरण 2: "Code" पर क्लिक करें और "Codespaces के साथ खोलें" चुनें।
रिपॉजिटरी पेज पर, "Code" ड्रॉपडाउन बटन पर क्लिक करें और विकल्पों में से "Codespaces के साथ खोलें" चुनें।

चरण 3: Codespace सेटिंग्स को कॉन्फ़िगर करें।
GitHub Codespaces आपके प्रोजेक्ट की कॉन्फ़िगरेशन के आधार पर स्वचालित रूप से एक डिफ़ॉल्ट वातावरण सेट करेगा। हालांकि, आप अपने रिपॉजिटरी में एक .devcontainer फ़ोल्डर जोड़कर वातावरण को अनुकूलित कर सकते हैं। इस फ़ोल्डर में, आप अपने Django प्रोजेक्ट के लिए आवश्यक उपकरण, एक्सटेंशन और वातावरण सेटिंग्स निर्दिष्ट कर सकते हैं।

चरण 4: Codespace लॉन्च करें।
अपने Django Codespace को बनाने की प्रक्रिया शुरू करने के लिए "Create Codespace" बटन पर क्लिक करें।

### अनुभाग 4: Django Codespaces में विकास
एक बार आपका Codespace तैयार हो जाने के बाद, आप ब्राउज़र-आधारित वातावरण के भीतर अपने Django एप्लिकेशन का विकास शुरू कर सकते हैं। यहाँ कुछ महत्वपूर्ण बिंदु दिए गए हैं:

IDE तक पहुँच: Codespace वातावरण Visual Studio Code जैसा दिखेगा और महसूस होगा, जिसमें एक परिचित इंटरफ़ेस और सुविधाएँ होंगी। आप Codespace पेज पर "Open in Visual Studio Code" बटन पर क्लिक करके IDE तक पहुँच सकते हैं।

निर्भरताएँ इंस्टॉल करना: यदि आपके Django प्रोजेक्ट के लिए कुछ विशेष निर्भरताएँ आवश्यक हैं, तो आप उन्हें प्रोजेक्ट की requirements.txt फ़ाइल में जोड़ सकते हैं और उन्हें इंस्टॉल करने के लिए एकीकृत टर्मिनल का उपयोग कर सकते हैं।

Django कमांड चलाना: आप Codespaces के भीतर एकीकृत टर्मिनल का उपयोग करके माइग्रेशन, विकास सर्वर शुरू करना, और एप्लिकेशन बनाने जैसी Django कमांड को निष्पादित कर सकते हैं।

संस्करण नियंत्रण: Codespaces GitHub के साथ गहराई से एकीकृत हैं, इसलिए आप क्लाउड-आधारित वातावरण से सीधे कमिट, पुश, और पुल कर सकते हैं।

अन्य लोगों के साथ सहयोग: आप अपने Codespace में सहयोगियों को आमंत्रित कर सकते हैं, जिससे आपके स्थानीय विकास वातावरण को साझा किए बिना परियोजनाओं पर सहयोग करना आसान हो जाता है।

### अनुभाग 5: ऑफ़लाइन कार्य करना
Codespaces का एक बड़ा लाभ यह है कि आप ऑफ़लाइन होते हुए भी विकास कार्य जारी रख सकते हैं। Codespaces आपके कार्य और कॉन्फ़िगरेशन को स्वचालित रूप से GitHub के साथ सिंक कर देता है, जिससे आप इंटरनेट कनेक्शन बहाल होने पर वहीं से काम जारी रख सकते हैं, जहाँ आपने छोड़ा था।

# निष्कर्ष:
GitHub Codespaces बिना स्थानीय सेटअप की आवश्यकता के Django एप्लिकेशन विकसित करने का एक कुशल और सहज तरीका प्रदान करते हैं। इस लेख में उल्लिखित चरणों का पालन करके, आप आसानी से GitHub में Django Codespaces को सेटअप और उपयोग कर सकते हैं, अपने विकास वर्कफ़्लो को सुव्यवस्थित कर सकते हैं और अन्य डेवलपर्स के साथ सहयोग बढ़ा सकते हैं। तो क्यों न इसे आज़माएँ और Django के साथ क्लाउड-आधारित कोडिंग की सुविधा का अनुभव करें!

## GitHub Actions Django Codespaces में

### निरंतर एकीकरण (CI):
अपने रिपॉजिटरी में कोड पुश करते समय एक वर्कफ़्लो सेट करें। इस वर्कफ़्लो में निर्भरताएँ इंस्टॉल करना, परीक्षण चलाना, और कोड कवरेज रिपोर्ट जनरेट करना शामिल हो सकता है।

```
नाम: Django CI

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - नाम: कोड चेकआउट करें
        uses: actions/checkout@v2

      - नाम: Python सेट करें
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - नाम: निर्भरताएँ इंस्टॉल करें
        run: pip install -r requirements.txt

      - नाम: परीक्षण चलाएँ
        run: python manage.py test

      - नाम: कवरेज रिपोर्ट जनरेट करें
        run: coverage run manage.py test && coverage xml

      - नाम: कवरेज रिपोर्ट अपलोड करें
        uses: actions/upload-artifact@v2
        with:
          name: coverage-report
          path: coverage.xml


```

### स्टेजिंग या प्रोडक्शन में तैनाती:
अपने Django एप्लिकेशन को स्टेजिंग या प्रोडक्शन वातावरण में तब स्वचालित रूप से तैनात करें जब आप विशिष्ट शाखाओं में पुश करते हैं।

```
नाम: स्टेजिंग में तैनात करें

on:
  push:
    branches:
      - staging

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - नाम: कोड चेकआउट करें
        uses: actions/checkout@v2

      - नाम: Python सेट करें
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - नाम: निर्भरताएँ इंस्टॉल करें
        run: pip install -r requirements.txt

      - नाम: स्टेजिंग में तैनात करें
        run: ./deploy_script.sh staging


```

### अनुसूचित कार्य:
GitHub Actions का उपयोग करके, डेटाबेस बैकअप या डेटा सिंकिंग जैसे अनुसूचित कार्य सेट करें।

```
नाम: अनुसूचित कार्य

on:
  schedule:
    - cron: '0 0 * * *' # आधी रात को रोज़ाना चलाएँ

jobs:
  backup:
    runs-on: ubuntu-latest

    steps:
      - नाम: कोड चेकआउट करें
        uses: actions/checkout@v2

      - नाम: Python सेट करें
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - नाम: निर्भरताएँ इंस्टॉल करें
        run: pip install -r requirements.txt

      - नाम: बैकअप चलाएँ
        run: python manage.py backup_script


```

याद रखें कि ये उदाहरण आपको GitHub Actions के साथ Django Codespaces में क्या हासिल किया जा सकता है, इसकी एक बुनियादी झलक प्रदान करते हैं। आपको अपनी परियोजना की विशिष्ट आवश्यकताओं और त

ैनाती प्रक्रियाओं के आधार पर इन वर्कफ़्लो को अनुकूलित करने की आवश्यकता हो सकती है। साथ ही, अपने रिपॉजिटरी सेटिंग्स में उपयुक्त पर्यावरण चर और संवेदनशील जानकारी जैसे API कुंजी और डेटाबेस क्रेडेंशियल्स के लिए रहस्यों को कॉन्फ़िगर करना सुनिश्चित करें।