# ഉള്ളടക്ക പട്ടിക
- [GitHubൽ Django Codespace](#githubൽ-django-codespace)
  - [വിഭാഗം 1: GitHub Codespaceഎന്താണ്?](#വിഭാഗം-1-github-codespaceഎന്താണ്)
  - [വിഭാഗം 2: മുൻകൂർ ആവശ്യകതകൾ](#വിഭാഗം-2-മുൻകൂർ-ആവശ്യകതകൾ)
  - [വിഭാഗം 3: Djangoക്ക് Codespace സൃഷ്ടിക്കുന്നത്](#വിഭാഗം-3-djangoക്ക്-codespace-സൃഷ്ടിക്കുന്നത്)
  - [വിഭാഗം 4: Django Codespaces-ൽ വികസിപ്പിക്കൽ](#വിഭാഗം-4-django-codespaces-ൽ-വികസിപ്പിക്കൽ)
  - [വിഭാഗം 5: ഓഫ്‌ലൈൻ പ്രവർത്തനം](#വിഭാഗം-5-ഓഫ്‌ലൈൻ-പ്രവർത്തനം)
- [സമാപനം](#സമാപനം)
- [GitHub Actions in Django Codespaces](#github-actions-in-django-codespaces)
  - [നിരന്തര സംയോജനം (CI)](#നിരന്തര-സംയോജനം-ci)
  - [സ്റ്റേജിംഗിലേക്ക് അല്ലെങ്കിൽ പ്രൊഡക്ഷൻ ദിശയിൽ നിക്ഷേപം](#സ്റ്റേജിംഗിലേക്ക്-അല്ലെങ്കിൽ-പ്രൊഡക്ഷൻ-ദിശയിൽ-നിക്ഷേപം)
  - [ക്രമീകരിച്ച ജോലി](#ക്രമീകരിച്ച-ജോലി)

# GitHubൽ Django Codespace

GitHub Codespaces ഒരു ശക്തമായ ക്ലൗഡ് അടിസ്ഥാനത്തിലുളള വികസന പരിസ്ഥിതിയാണ്, ഇത് ഡെവലപ്പർമാർക്ക് അവരുടെ ബ്രൗസറിൽ നേരിട്ട് കോഡ് ചെയ്യാൻ, നിർമിക്കാൻ, ടെസ്റ്റ് ചെയ്യാൻ കഴിയും. ഇത് ലോക്കൽ വികസന ക്രമീകരണങ്ങളുടെ ആവശ്യകത ഇല്ലാതാക്കുന്നതിലൂടെ എളുപ്പമുള്ള ഒരു സുതാര്യമായ കോഡിംഗ് അനുഭവം നൽകുന്നു. ഈ ലേഖനം GitHubൽ Django Codespace സജ്ജമാക്കുന്നതും ഉപയോഗിക്കുന്നതും വഴി Django അപ്ലിക്കേഷനുകൾ എളുപ്പത്തിൽ വികസിപ്പിക്കാനുളള മാർഗ്ഗങ്ങൾ വിവരിക്കുന്നു.

### വിഭാഗം 1: GitHub Codespaceഎന്താണ്?

GitHub Codespaces ഡെവലപ്പർമാർക്ക് ക്ലൗഡിൽ ഹോസ്റ്റുചെയ്ത ഒരു പൂർണ്ണമായുള്ള ക്രമീകരിതമായ വികസന പരിസ്ഥിതി സൃഷ്ടിക്കാൻ അനുവദിക്കുന്നു. ഇത് Visual Studio Code-ന്റെ പരിചിതമായ ഇന്റർഫേസ്, സവിശേഷതകളെ അടിസ്ഥാനമാക്കുന്നു, ലോക്കൽ വികസന പരിസ്ഥിതിയിൽ നിന്നും ക്ലൗഡിലേക്ക് എളുപ്പത്തിൽ മാറാൻ സാധിക്കുന്നു.

### വിഭാഗം 2: മുൻകൂർ ആവശ്യകതകൾ

GitHubൽ Django Codespaces ഉപയോഗിക്കുന്നതിന്, നിങ്ങൾക്ക് താഴെപ്പറയുന്നവ വേണ്ടിവരും:

- GitHub അക്കൗണ്ട്: GitHub Codespaces ഉപയോഗിക്കാൻ GitHub അക്കൗണ്ട്.
- Django പ്രോജക്ട്: GitHubൽ ഹോസ്റ്റുചെയ്യപ്പെട്ട Django പ്രോജക്ട്, നിങ്ങൾ ക്ലൗഡിൽ പ്രവർത്തിപ്പിക്കാൻ ആഗ്രഹിക്കുന്നു.

### വിഭാഗം 3: Djangoക്ക് Codespace സൃഷ്ടിക്കുന്നത്

നിങ്ങളുടെ Django പ്രോജക്റ്റിനായി Codespace സൃഷ്ടിക്കുന്നതിനുള്ള ചുവടുകൾ:

**ചുവടുവയ്പ്പ് 1**: GitHub രെപ്പോസിറ്ററിലേയ്ക്ക് പോകുക  
Django പ്രോജക്റ്റ് രെപ്പോസിറ്ററിയിലേക്ക് GitHubയിൽ പോകുക.

**ചുവടുവയ്പ്പ് 2**: "Code" ഒപ്പം "Open with Codespaces" ക്ലിക്ക് ചെയ്യുക  
രെപ്പോസിറ്ററി പേജിൽ, "Code" ഡ്രോപ്പ് ഡൗൺ ബട്ടണിൽ ക്ലിക്ക് ചെയ്ത് "Open with Codespaces" എന്ന ഓപ്ഷൻ തിരഞ്ഞെടുക്കുക.

**ചുവടുവയ്പ്പ് 3**: Codespace ക്രമീകരണങ്ങൾ കോൺഫിഗർ ചെയ്യുക  
GitHub Codespaces നിങ്ങളുടെ പ്രോജക്റ്റ് ക്രമീകരണത്തിന് അനുയോജ്യമായ ഡീഫാൾട്ട് പരിസ്ഥിതി ക്രമീകരിക്കും. എന്നിരുന്നാലും, .devcontainer ഫോൾഡർ ചേർത്ത് ഇത് ഇഷ്ടാനുസൃതമാക്കാവുന്നതാണ്.

**ചുവടുവയ്പ്പ് 4**: Codespace ആരംഭിക്കുക  
"Django Codespace സൃഷ്ടിക്കുക" ബട്ടണിൽ ക്ലിക്ക് ചെയ്ത് Codespace സൃഷ്ടിക്കുന്ന പ്രക്രിയ ആരംഭിക്കുക.

### വിഭാഗം 4: Django Codespaces-ൽ വികസിപ്പിക്കൽ

നിങ്ങളുടെ Codespace സജ്ജമായുകഴിഞ്ഞാൽ, ബ്രൗസർ-അടിസ്ഥാനത്തിലുള്ള പരിസ്ഥിതിയിലാണ് നിങ്ങൾ Django അപ്ലിക്കേഷൻ വികസിപ്പിക്കാൻ തുടങ്ങുക.

**പ്രധാനമായ ചിട്ടകൾ**:

- **IDE-യിൽ പ്രവേശനം**: Codespace പരിസ്ഥിതി Visual Studio Code പോലെയായിരിക്കും.
- **ആവശ്യമായ ഡിപ്പൻഡൻസികൾ ഇൻസ്റ്റാൾ ചെയ്യുക**: `requirements.txt` ഫയലിൽ സ്പെസിഫൈ ചെയ്തിരിക്കുന്ന ഡിപ്പൻഡൻസികൾ ഇൻസ്റ്റാൾ ചെയ്യാം.
- **Django കമാൻഡുകൾ ഓടിക്കുക**: മൈഗ്രേഷനുകൾ, ഡെവലപ്മെന്റ് സെർവർ തുടങ്ങിയ കമാൻഡുകൾ ഓടിക്കാൻ Codespace ടെർമിനൽ ഉപയോഗിക്കുക.
- **വർഷൻ കൺട്രോൾ**: GitHub ഉം Codespaces ഉം ഒരുമിച്ച് പ്രവർത്തിക്കുന്നു.
- **പങ്കിടൽ**: നിങ്ങളുടെ Codespace-ൽ സഹപ്രവർത്തകരെ ക്ഷണിക്കാം.

### വിഭാഗം 5: ഓഫ്‌ലൈൻ പ്രവർത്തനം

Codespaces-ന്റെ ഒരു പ്രധാന സവിശേഷത ഓഫ്‌ലൈൻ പ്രവർത്തന ശേഷിയാണിത്. GitHub-യിലേക്ക് പ്രവർത്തനങ്ങൾ സമന്വയിപ്പിക്കപ്പെടുകയും വീണ്ടും ഓൺലൈൻ ആയപ്പോൾ അവ പ്രവർത്തനക്ഷമമായി തുടരുകയും ചെയ്യാം.

# സമാപനം:
GitHub Codespaces Django അപ്ലിക്കേഷനുകൾ സൃഷ്ടിക്കാൻ വളരെ എളുപ്പമുള്ള രീതിയാണ്. ഈ ലേഖനത്തിൽ നൽകിയിരിക്കുന്ന ചുവടുവയ്പ്പുകൾ പിന്തുടർന്നുകൊണ്ട് GitHub-ൽ Django Codespaces എളുപ്പത്തിൽ സജ്ജമാക്കുകയും ഉപയോഗിക്കയും ചെയ്യാം.

## GitHub Actions in Django Codespaces

### നിരന്തര സംയോജനം (CI):

GitHub-ൽ കോഡ് പുഷ് ചെയ്താൽ ഓരോ തവണയും പ്രവർത്തിക്കുന്ന ഒരു വർക്ക്‌ഫ്ലോ സജ്ജമാക്കുക. ഡിപ്പൻഡൻസികൾ ഇൻസ്റ്റാൾ ചെയ്യുക, ടെസ്റ്റുകൾ പ്രവർത്തിപ്പിക്കുക, കോഡ് കവർേജ് റിപ്പോർട്ട് സൃഷ്ടിക്കുക എന്നിവ ഉൾപ്പെടുത്താം.

```yaml
name: Django CI

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

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - name: Install dependencies
        run: pip install -r requirements.txt

      - name: Run tests
        run: python manage.py test

      - name: Generate coverage report
        run: coverage run manage.py test && coverage xml

      - name: Upload coverage report
        uses: actions/upload-artifact@v2
        with:
          name: coverage-report
          path: coverage.xml
name: Deploy to Staging

on:
  push:
    branches:
      - staging

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - name: Install dependencies
        run: pip install -r requirements.txt

      - name: Deploy to Staging
        run: ./deploy_script.sh staging
name: Scheduled Tasks

on:
  schedule:
    - cron: '0 0 * * *' # മധ്യരാത്രി ദിവസവും പ്രവർത്തിപ്പിക്കുക

jobs:
  backup:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: 3.x

      - name: Install dependencies
        run: pip install -r requirements.txt

      - name: Run backup
        run: python manage.py backup_script
