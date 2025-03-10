# مواد کی فہرست

- [GitHub میں C# Codespaces کا استعمال](#github-میں-c-codespaces-کا-استعمال)
    - [ضروریات](#ضروریات)
    - [C# Codespaces کے ساتھ کام کرنا](#c-codespaces-کے-ساتھ-کام-کرنا)
    - [Codespaces کے ذریعے مشترکہ ترقی](#codespaces-کے-ذریعے-مشترکہ-ترقی)
- [C# Codespaces میں GitHub Actions کا استعمال](#c-codespaces-میں-github-actions-کا-استعمال)
    - [Codespace کنفیگریشن فائل بنائیں:](#codespace-کنفیگریشن-فائل-بنائیں)

# GitHub میں C# Codespaces کا استعمال

GitHub Codespaces ایک کلاؤڈ بیسڈ ڈویلپمنٹ ماحول ہے جو ڈویلپرز کو براہ راست GitHub ریپوزیٹری میں کوڈ لکھنے، بنانا، ٹیسٹ کرنے اور ڈیبگ کرنے کی سہولت فراہم کرتا ہے۔ یہ ایک طاقتور اور آسان طریقہ فراہم کرتا ہے تاکہ ٹیم کے اراکین ایک دوسرے کے ساتھ آسانی سے کام کر سکیں اور کسی پیچیدہ سیٹ اپ یا کنفیگریشن کی ضرورت کے بغیر اپنے پروجیکٹس پر کام کر سکیں۔ Codespaces کی مدد سے آپ اپنے براؤزر سے براہ راست ایک مکمل کنفیگرڈ ڈویلپمنٹ ماحول تک رسائی حاصل کر سکتے ہیں، جو کہیں سے بھی آپ کے کوڈ پر کام کرنے کو آسان بناتا ہے۔

اس مضمون میں، ہم GitHub میں C# Codespaces کو سیٹ اپ اور استعمال کرنے کے طریقے کو دریافت کریں گے، تاکہ آپ C# پروجیکٹس کو باآسانی ڈویلپ کر سکیں۔ ہم کچھ عملی مثالوں پر بھی روشنی ڈالیں گے تاکہ آپ کو Codespaces کے حقیقی استعمال کا اندازہ ہو سکے۔

### ضروریات

C# Codespaces کے ساتھ کام شروع کرنے سے پہلے، درج ذیل چیزوں کو یقینی بنائیں:

- **GitHub اکاؤنٹ:** Codespaces کو بنانے اور استعمال کرنے کے لیے آپ کے پاس GitHub پر ایک اکاؤنٹ ہونا ضروری ہے۔
- **C# پروجیکٹ:** آپ کے پاس ایک C# پروجیکٹ ہونا چاہیے جس پر آپ Codespaces میں کام کرنا چاہتے ہیں۔ آپ نیا پروجیکٹ بنا سکتے ہیں یا پہلے سے موجود پروجیکٹ کو استعمال کر سکتے ہیں۔

### C# Codespace بنانا

1. **اپنی GitHub ریپوزیٹری پر جائیں:** سب سے پہلے، اس ریپوزیٹری پر جائیں جہاں آپ کا C# پروجیکٹ موجود ہے۔
2. **"Code" بٹن پر کلک کریں:** ریپوزیٹری کے مرکزی صفحے پر "Code" بٹن (سبز رنگ کا) پر کلک کریں تاکہ ایک ڈراپ ڈاؤن مینو ظاہر ہو۔
3. **"Open with Codespaces" منتخب کریں:** ڈراپ ڈاؤن مینو سے "Open with Codespaces" کا انتخاب کریں۔ اگر آپ نے پہلے اس ریپوزیٹری میں Codespaces استعمال نہیں کیا تو یہ آپ کو ایک Codespace کنفیگریشن فائل بنانے کا کہے گا۔
4. **اپنے Codespace کو کنفیگر کریں (اگر ضروری ہو):** اگر آپ پہلی بار Codespaces سیٹ اپ کر رہے ہیں تو آپ کو ایک `.devcontainer` فولڈر اور `devcontainer.json` فائل بنانے کا کہا جائے گا۔ یہ فائل آپ کے ڈویلپمنٹ ماحول کی ترتیبات، جیسے رن ٹائم، ایکسٹینشنز اور دیگر انحصارات کو بیان کرتی ہے۔

یہاں ایک مثال `devcontainer.json` فائل کی دی گئی ہے جو C# پروجیکٹ کے لیے ہے:

```
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:5.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [5000]
}
```

اس مثال میں، ہم نے .NET SDK 5.0 کا آفیشل امیج استعمال کیا ہے اور C# ایکسٹینشن کو انسٹال کیا ہے۔

### C# Codespaces کے ساتھ کام کرنا

ایک بار جب آپ کا Codespace سیٹ اپ ہو جائے تو آپ اسے اپنے GitHub ریپوزیٹری میں "Codespaces" ٹیب پر جا کر کھول سکتے ہیں۔ اپنی مطلوبہ Codespace کو منتخب کریں اور "Connect" پر کلک کریں تاکہ ڈویلپمنٹ ماحول آپ کے براؤزر میں کھل جائے۔

آپ کو Visual Studio Code جیسا انٹرفیس نظر آئے گا، جو پہلے سے کنفیگرڈ ہوگا تاکہ آپ C# ایپلیکیشنز کو باآسانی ڈویلپ کر سکیں۔

#### مثال: C# کنسول ایپلیکیشن بنانا

آئیے ایک سادہ C# کنسول ایپلیکیشن بنانے کا عمل دیکھتے ہیں۔

1. **Codespace سے جڑیں:** پہلے بتائے گئے طریقے کے مطابق Codespace سے جڑیں۔
2. **ایک نیا ٹرمینل کھولیں:** Visual Studio Code میں "Terminal" مینو پر کلک کریں اور "New Terminal" کو منتخب کریں تاکہ ایک نیا ٹرمینل کھل جائے۔
3. **نئی C# کنسول ایپلیکیشن بنائیں:** نیچے دیے گئے کمانڈز کے ذریعے ایک نئی C# کنسول ایپلیکیشن بنائیں۔

```
dotnet new console -n MyConsoleApp
cd MyConsoleApp
```

4. **کوڈ لکھیں:** `Program.cs` فائل کو کھولیں اور درج ذیل کوڈ لکھیں۔

```
using System;

namespace MyConsoleApp
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hello, Codespaces!");
        }
    }
}
```

5. **ایپلیکیشن کو بنائیں اور چلائیں:** مندرجہ ذیل کمانڈز کے ذریعے اپنی ایپلیکیشن کو کمپائل اور رن کریں۔

```
dotnet build
dotnet run
```

آپ کو ٹرمینل میں آؤٹ پٹ نظر آئے گا: `"Hello, Codespaces!"`۔

### Codespaces کے ذریعے مشترکہ ترقی

Codespaces کا ایک بڑا فائدہ یہ ہے کہ یہ مشترکہ ترقی (collaborative development) کو بہت آسان بناتا ہے۔ ایک ہی پروجیکٹ پر متعدد ٹیم ممبرز بیک وقت کام کر سکتے ہیں، ہر ایک اپنی Codespace میں۔ اس سے تصادم (conflicts) سے بچا جا سکتا ہے اور کوڈ کی ریویو اور مرجنگ کے عمل کو بہتر بنایا جا سکتا ہے۔

جب آپ مشترکہ ترقی کر رہے ہوں تو ہر ڈویلپر اپنی برانچ بنا سکتا ہے، تبدیلیاں کر سکتا ہے، اور روایتی طریقے سے Pull Requests جمع کروا سکتا ہے۔ ریویو کرنے والے براہ راست Codespace میں ان تبدیلیوں کو آزما سکتے ہیں، جس سے پروجیکٹ کا معیار مزید بہتر ہوتا ہے۔

GitHub Codespaces C# ڈویلپرز کے لیے ایک بہترین پلیٹ فارم فراہم کرتا ہے تاکہ وہ بغیر کسی پیچیدہ سیٹ اپ کے، تیزی سے کام کر سکیں۔ یہ پلیٹ فارم خاص طور پر ٹیم کے ساتھ مل کر کام کرنے کے لیے بہترین ہے۔

---

# C# Codespaces میں GitHub Actions کا استعمال

### Codespace کنفیگریشن فائل بنائیں: 

سب سے پہلے، آپ کو `.devcontainer/devcontainer.json` فائل بنانے کی ضرورت ہوگی تاکہ اپنے Codespace ماحول کو کنفیگر کر سکیں۔ ایک مثال یہ ہے:

```
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:6.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [80]
}
```

یہ کنفیگریشن .NET SDK 6.0 امیج اور C# ایکسٹینشن کے ساتھ Codespace کو کنفیگر کرتا ہے۔

### ورک فلو YAML فائل بنائیں

اب آپ کو `.github/workflows/build.yml` فائل بنانی ہوگی تاکہ GitHub Actions خودکار طریقے سے آپ کا پروجیکٹ بلڈ اور ٹیسٹ کرے۔

```
name: Build and Test

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - name: Checkout code
      uses: actions/checkout@v2

    - name: Set up .NET
      uses: actions/setup-dotnet@v2
      with:
        dotnet-version: '6.0.x'

    - name: Restore dependencies
      run: dotnet restore

    - name: Build
      run: dotnet build --configuration Release

    - name: Run tests
      run: dotnet test --configuration Release
```

یہ ورک فلو آپ کی کوڈ میں تبدیلیوں کے ساتھ خودکار بلڈ اور ٹیسٹنگ کا عمل مکمل کرے گا۔

GitHub Actions اور Codespaces کا مجموعہ C# ڈویلپرز کے لیے زبردست کارکردگی فراہم کرتا ہے۔