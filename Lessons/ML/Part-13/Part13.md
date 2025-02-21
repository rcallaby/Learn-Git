## ഉള്ളടക്കസൂചിക

- [GitHub-ൽ C# Codespaces ഉപയോഗിക്കുന്നു](#using-c-codespaces-in-github)  
    - [ആവശ്യമായവ](#prerequisites)  
    - [C# Codespaces ഉപയോഗിച്ച് പ്രവർത്തിക്കൽ](#working-with-c-codespaces)  
    - [Codespaces ഉപയോഗിച്ച് സഹകരണ വികസനം](#collaborative-development-with-codespaces)  
- [C# Codespaces-ൽ GitHub Actions ഉപയോഗിക്കുന്നു](#using-github-actions-in-c-codespaces)  
    - [Codespace കോൺഫിഗറേഷൻ ഫയൽ സൃഷ്ടിക്കുക](#create-a-codespace-configuration-file)  

# GitHub-ൽ C# Codespaces ഉപയോഗിക്കുന്നു

GitHub Codespaces ഒരു ക്ലൗഡ് അടിസ്ഥാനത്തിലുള്ള ഡെവലപ്മെന്റ് എൻവയ്റൺമെന്റാണ്, ഇത് ഡെവലപ്പർമാരെ അവരുടെ GitHub റെപ്പോസിറ്ററിയിൽ നേരിട്ടാണ് കോഡ് എഴുതാൻ, നിർമ്മിക്കാൻ, ടെസ്റ്റ് നടത്താൻ, ഡീബഗ് ചെയ്യാൻ അനുവദിക്കുന്നു. ഇത് സഹപ്രവർത്തകരുമായി ഒത്തുചേരാനുള്ള ശക്തമായതും സൗകര്യപ്രദവുമായ ഒരു മാർഗമാണ്, കൂടാതെ കോംപ്ലക്സായ ക്രമീകരണങ്ങൾ ഇല്ലാതെ തന്നെ പദ്ധതികളിൽ പ്രവർത്തിക്കാൻ കഴിയും. Codespaces ഉപയോഗിച്ച്, നിങ്ങളുടെ ബ്രൗസറിലൂടെ നേരിട്ട് പൂർണ്ണമായി കോൺഫിഗർ ചെയ്ത ഡെവലപ്മെന്റ് എൻവയ്റൺമെന്റ് ആക്സസ് ചെയ്യാം, അതിനാൽ എവിടുനിന്നും നിങ്ങളുടെ കോഡിൽ പ്രവർത്തിക്കാൻ എളുപ്പമാണ്.

ഈ ലേഖനത്തിൽ, GitHub-ൽ C# Codespaces എങ്ങനെ സജ്ജീകരിക്കാം, ഉപയോഗിക്കാം എന്നതിനെക്കുറിച്ച് പരിശോധിക്കും. C# വികസനത്തിൽ Codespaces പ്രായോഗികമായി എങ്ങനെ ഉപയോഗിക്കാം എന്നതിന് ഉദാഹരണങ്ങളും ചേർക്കാം.

### ആവശ്യമായവ

C# Codespaces ഉപയോഗിക്കാനുമുമ്പ്, നിങ്ങൾക്ക് ചുവടെ പറയുന്നവ ആവശ്യമുണ്ട്:

- **GitHub അക്കൗണ്ട്**: Codespaces സൃഷ്ടിക്കാൻ, ഉപയോഗിക്കാൻ നിങ്ങൾക്ക് GitHub-ൽ ഒരു അക്കൗണ്ട് ആവശ്യമാണ്.  
- **C# പ്രോജക്ട്**: Codespaces ഉപയോഗിച്ച് പ്രവർത്തിക്കാൻ നിങ്ങൾക്ക് ഒരു C# പ്രോജക്ട് തയ്യാറാക്കണം. നിങ്ങൾക്ക് പുതിയത് സൃഷ്ടിക്കാമോ അതോ നിലവിലുള്ളതോ ഉപയോഗിക്കാം.  

### C# Codespace സൃഷ്ടിക്കുന്നത്

1. **GitHub റെപ്പോസിറ്ററിയിലേക്ക് പോകുക**: നിങ്ങളുടെ C# പ്രോജക്ട് ഉള്ള റെപ്പോസിറ്ററിയിലേക്ക് നാവിഗേറ്റ് ചെയ്യുക.  
2. **"Code" ബട്ടൺ ക്ലിക്ക് ചെയ്യുക**: റെപ്പോസിറ്ററിയുടെ പ്രധാന പേജിൽ, പച്ച നിറത്തിലുള്ള `"Code"` ബട്ടൺ ക്ലിക്ക് ചെയ്ത് ഡ്രോപ്പ്-ഡൗൺ മെനു തുറക്കുക.  
3. **"Open with Codespaces" തിരഞ്ഞെടുക്കുക**: ഡ്രോപ്പ്-ഡൗൺ മെനുവിൽ നിന്ന് `"Open with Codespaces"` തിരഞ്ഞെടുക്കുക.  
4. **Codespace കോൺഫിഗർ ചെയ്യുക (ആവശ്യമെങ്കിൽ)**: ഈ റെപ്പോസിറ്ററിയിൽ ആദ്യമായി Codespaces ഉപയോഗിക്കുകയാണെങ്കിൽ, `.devcontainer` ഫോൾഡറിലും `devcontainer.json` കോൺഫിഗറേഷൻ ഫയലും സൃഷ്ടിക്കാൻ ആവശ്യപ്പെടും.  

#### C# പ്രോജക്ടിനായുള്ള `devcontainer.json` ഉദാഹരണം:
```json
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
ഇത് .NET SDK 5.0 ഇമേജ് ഉപയോഗിച്ച് C# എക്സ്ററൻഷൻ ഇൻസ്റ്റാൾ ചെയ്യുന്നു.  

### C# Codespaces ഉപയോഗിച്ച് പ്രവർത്തിക്കൽ

Codespace സജ്ജീകരിച്ചുകഴിഞ്ഞാൽ, GitHub റെപ്പോസിറ്ററിയിൽ `"Codespaces"` ടാബ് തുറന്ന് `"Connect"` ക്ലിക്ക് ചെയ്യുക. Visual Studio Code പോലെ തന്നെ പരിചിതമായ ഒരു ഇന്റർഫേസ് ലഭിക്കും.

#### ഉദാഹരണം: C# Console പ്രോഗ്രാം സൃഷ്ടിക്കൽ

1. **Codespace-ലേക്ക് കണക്റ്റ് ചെയ്യുക**  
2. **ടെർമിനൽ തുറക്കുക**: `"Terminal"` മെനുവിൽ `"New Terminal"` തിരഞ്ഞെടുക്കുക.  
3. **C# Console പ്രോഗ്രാം സൃഷ്ടിക്കുക**:  
```sh
dotnet new console -n MyConsoleApp
cd MyConsoleApp
```
4. **`Program.cs` ഫയലിൽ കോഡ് എഴുതുക**  
```csharp
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
5. **പ്രോഗ്രാം നിർമ്മിക്കുകയും പ്രവർത്തിപ്പിക്കുകയും ചെയ്യുക**  
```sh
dotnet build
dotnet run
```
ടെർമിനലിൽ `"Hello, Codespaces!"` എന്ന ഔട്ട്പുട്ട് കാണാം.  

### Codespaces ഉപയോഗിച്ച് സഹകരണ വികസനം

Codespaces-ന്റെ പ്രധാന സവിശേഷതകളിലൊന്ന് അതിന്റെ സഹകരണ പ്രവർത്തനങ്ങളാണ്. ഒരു പ്രോജക്ടിൽ നിരവധി ടീം അംഗങ്ങൾ ഒരേസമയം പ്രവർത്തിക്കാം, കൂടാതെ മാറ്റങ്ങൾ അവലോകനം ചെയ്യാനും സിംപ്ലിഫൈ ചെയ്യാനും Codespaces സഹായിക്കും.  

GitHub Codespaces C# ഡെവലപ്പർമാർക്ക് സഹകരണപരമായി പ്രോജക്ടുകൾ വികസിപ്പിക്കാൻ മികച്ച ഒരു പ്ലാറ്റ്ഫോമാണ്.  

---

# C# Codespaces-ൽ GitHub Actions ഉപയോഗിക്കുന്നു  

### Codespace കോൺഫിഗറേഷൻ ഫയൽ സൃഷ്ടിക്കുക  

`.devcontainer/devcontainer.json` ഫയൽ GitHub Codespaces കോൺഫിഗർ ചെയ്യാൻ ആവശ്യമാണ്. ഉദാഹരണം:  
```json
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
ഇത് .NET SDK 6.0 ഉപയോഗിക്കുകയും C# എക്സ്ററൻഷൻ ഇൻസ്റ്റാൾ ചെയ്യുകയും ചെയ്യുന്നു.  

### GitHub Actions Workflow സൃഷ്ടിക്കുക  

`.github/workflows/build.yml` ഫയലിൽ GitHub Actions workflow നിർവചിക്കുക:  
```yaml
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
      run: dotnet test --configuration Release --no-build
```
ഇത് `main` ബ്രാഞ്ചിലേക്ക് കോഡ് പുഷ് ചെയ്തപ്പോൾ ഓട്ടോമാറ്റിക് ആയി പ്രവർത്തിക്കും.  

### Commit & Push  
`.devcontainer` ഫോൾഡറും `.github/workflows` ഫയലുകളും GitHub-ൽ commit ചെയ്ത് push ചെയ്യുക.  

### GitHub Actions നിർവഹിക്കൽ  
`build.yml` അനുസരിച്ച് GitHub Actions ഓട്ടോമാറ്റിക് ആയി പ്രവർത്തിക്കും. GitHub റെപ്പോസിറ്ററിയുടെ `"Actions"` ടാബിൽ ഇതിന്റെ സ്റ്റാറ്റസ് പരിശോധിക്കാം.  

ഈ workflow കൂടുതൽ കസ്റ്റമൈസ് ചെയ്യാനാകും, ഉദാഹരണത്തിന് ഡിപ്പ്ലോയ്‌മെന്റ്, ഇൻറിഗ്രേഷൻ ടെസ്റ്റുകൾ എന്നിവ ചേർക്കാം.  

