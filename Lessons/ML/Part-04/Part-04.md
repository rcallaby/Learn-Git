# ദൂരസ്ഥ റിപ്പോസിറ്ററികളുമായി സഹകരിക്കുക

- [ദൂരസ്ഥ റിപ്പോസിറ്ററികൾ സജ്ജീകരിക്കൽ (GitHub, GitLab, Bitbucket)](#setting-up-remote-repositories-github-gitlab-bitbucket)
- [GitHub](#github)
- [GitLab](#gitlab)
- [Bitbucket](#bitbucket)
- [ദൂരസ്ഥ റിപ്പോസിറ്ററികളിൽ മാറ്റങ്ങൾ പുഷ് ചെയ്യുകയും_pull ചെയ്യുകയും ചെയ്യുക](#pushing-and-pulling-changes-from-remote-repositories)
- [മേർജ് സംഘർഷങ്ങൾ കൈകാര്യം ചെയ്യൽ](#handling-merge-conflicts)
- [മികച്ച ശീലങ്ങൾ](#best-practices)

## ദൂരസ്ഥ റിപ്പോസിറ്ററികൾ സജ്ജീകരിക്കൽ (GitHub, GitLab, Bitbucket)

സോഫ്റ്റ്‌വെയർ വികസന ലോകത്ത്, പതിപ്പുചട്ട സംവിധാനങ്ങൾ (Version Control Systems) കോഡ് സംഗ്രഹങ്ങൾ നിയന്ത്രിക്കാൻ, സഹകരണത്തെ സുഗമമാക്കാൻ, ടീമംഗങ്ങൾക്കിടയിൽ കാര്യക്ഷമമായ പ്രവാഹം ഉറപ്പാക്കാൻ വളരെ പ്രധാനമാണ്. GitHub, GitLab, Bitbucket പോലുള്ള പ്ലാറ്റ്‌ഫോമുകളിൽ ഹോസ്റ്റുചെയ്‌തിരിക്കുന്ന ദൂരസ്ഥ റിപ്പോസിറ്ററികൾ വികസകരുടെ കോഡ് സംഭരിക്കാൻ, കൈകാര്യം ചെയ്യാൻ, പങ്കുവയ്ക്കാൻ കേന്ദ്രഭാഗം വഹിക്കുന്നു. ഈ ലേഖനത്തിൽ, ഓരോ പ്ലാറ്റ്‌ഫോമിലും ദൂരസ്ഥ റിപ്പോസിറ്ററികൾ സജ്ജീകരിക്കുന്ന നടപടിക്രമം വിശദമായി പഠിക്കാം.

### GitHub
GitHub, Git അടിസ്ഥാനമാക്കിയുള്ള ഏറ്റവും പ്രശസ്തമായ വെബ് ഹോസ്റ്റിംഗ് പ്ലാറ്റ്‌ഫോമുകളിൽ ഒന്നാണ്. GitHub-ൽ ഒരു ദൂരസ്ഥ റിപ്പോസിറ്ററി സജ്ജീകരിക്കുന്നതിന്റെ വിശദമായ ഗൈഡ് ചുവടെ:

#### പടി 1: GitHub അക്കൗണ്ട് സൃഷ്ടിക്കുക
നിങ്ങൾക്ക് അക്കൗണ്ട് ഇല്ലെങ്കിൽ, [github.com](https://github.com) സന്ദർശിച്ച് രജിസ്റ്റർ ചെയ്യുക.

#### പടി 2: പുതിയ റിപ്പോസിറ്ററി സൃഷ്ടിക്കുക
ലോഗിൻ ചെയ്ത ശേഷം, GitHub ഡാഷ്ബോർഡിലെ "+ New" ബട്ടൺ ക്ലിക്ക് ചെയ്യുക. റിപ്പോസിറ്ററിക്ക് ഒരു പേര് നൽകുക, ഐച്ഛികമായ വിവരണം ചേർക്കുക, പബ്ലിക് അല്ലെങ്കിൽ പ്രൈവറ്റ് ആണോ എന്നത് നിർദിഷ്ടമാക്കുക.

#### പടി 3: റിപ്പോസിറ്ററി ഇൻിഷ്യലൈസ് ചെയ്യുക
README ഫയൽ ചേർത്ത് റിപ്പോസിറ്ററി ആരംഭിക്കുന്നതും (initialize) നല്ല ശീലമാണ്. ഇത് പ്രോജക്റ്റിന്റെ അടിസ്ഥാന വിവരങ്ങൾ നൽകുന്നു.

#### പടി 4: റിപ്പോസിറ്ററി ക്ലോൺ ചെയ്യുക (ഐച്ഛികം)
ലോകൽ ആയി പ്രവർത്തിക്കണമെങ്കിൽ, താഴെയുള്ള Git കമാൻഡ് ഉപയോഗിച്ച് റിപ്പോസിറ്ററി ക്ലോൺ ചെയ്യാം:
```bash
git clone <repository_url>
```

### GitLab
GitLab, വിപുലമായ സവിശേഷതകൾ നൽകുന്ന മറ്റൊരു ജനപ്രിയ Git റിപ്പോസിറ്ററി മാനേജർ ആണ്. GitLab-ൽ ദൂരസ്ഥ റിപ്പോസിറ്ററി സജ്ജീകരിക്കുന്നതിനുള്ള ഘട്ടങ്ങൾ ചുവടെ:

#### പടി 1: GitLab അക്കൗണ്ട് സൃഷ്ടിക്കുക
[gitlab.com](https://gitlab.com) സന്ദർശിച്ച് ഒരു അക്കൗണ്ട് ഉണ്ടാക്കുക.

#### പടി 2: പുതിയ പ്രോജക്റ്റ് സൃഷ്ടിക്കുക
ഡാഷ്ബോർഡിൽ "New Project" ബട്ടൺ ക്ലിക്ക് ചെയ്ത്, ഒരു പേര് നൽകുക, ഐച്ഛികമായ വിവരണം ചേർക്കുക, പ്രോജക്റ്റ് ദൃശ്യപരത (visibility) സജ്ജമാക്കുക.

#### പടി 3: റിപ്പോസിറ്ററി ഇൻിഷ്യലൈസ് ചെയ്യുക
README ഫയൽ ഉൾപ്പെടുത്തുക, ഇത് നല്ല ശീലമാണ്.

#### പടി 4: റിപ്പോസിറ്ററി ക്ലോൺ ചെയ്യുക (ഐച്ഛികം)
```bash
git clone <repository_url>
```

### Bitbucket
Bitbucket, Atlassian-ന്റെ ഉടമസ്ഥതയിലുള്ള Git റിപ്പോസിറ്ററി ഹോസ്റ്റിംഗ് സേവനമാണ്.

#### പടി 1: Bitbucket അക്കൗണ്ട് സൃഷ്ടിക്കുക
[bitbucket.org](https://bitbucket.org) സന്ദർശിച്ച് രജിസ്റ്റർ ചെയ്യുക.

#### പടി 2: പുതിയ റിപ്പോസിറ്ററി സൃഷ്ടിക്കുക
"Create repository" ബട്ടൺ ക്ലിക്ക് ചെയ്ത്, പേര് നൽകുക, വിവരണം ചേർക്കുക, പബ്ലിക് അല്ലെങ്കിൽ പ്രൈവറ്റ് ആണോ എന്നത് നിർദിഷ്ടമാക്കുക.

#### പടി 3: റിപ്പോസിറ്ററി തരം തിരഞ്ഞെടുക്കുക
Git അല്ലെങ്കിൽ Mercurial ആയിരിക്കും ദൂരസ്ഥ റിപ്പോസിറ്ററികൾക്കുള്ള ഓപ്ഷനുകൾ. "Git" തിരഞ്ഞെടുക്കുക.

#### പടി 4: റിപ്പോസിറ്ററി ഇൻിഷ്യലൈസ് ചെയ്യുക
README ഫയൽ ചേർക്കുക.

#### പടി 5: റിപ്പോസിറ്ററി ക്ലോൺ ചെയ്യുക (ഐച്ഛികം)
```bash
git clone <repository_url>
```

### ദൂരസ്ഥ റിപ്പോസിറ്ററികളിൽ മാറ്റങ്ങൾ പുഷ് ചെയ്യുകയും_pull ചെയ്യുകയും ചെയ്യുക

Git ഉപയോഗിച്ച്, വിവിധ വികസകർ ഒരേ പ്രോജക്റ്റിൽ ഒരേസമയം പ്രവർത്തിക്കാൻ കഴിയും. അതിനായി പുഷ് (push) ചെയ്ത്_PULL (pull) ചെയ്യാനുള്ള പ്രക്രിയ മനസ്സിലാക്കേണ്ടതുണ്ട്.

#### പുഷ് ചെയ്യുന്നതിനുള്ള നടപടികൾ
##### 1. ലോക്കൽ മാറ്റങ്ങൾ_commit ചെയ്യുക
```bash
git commit -m "Commit message"
```
##### 2. റിമോട്ട് റിപ്പോസിറ്ററി പരിശോധിക്കുക
```bash
git remote -v
```
##### 3. മാറ്റങ്ങൾ പുഷ് ചെയ്യുക
```bash
git push <remote_name> <branch_name>
```
ഉദാഹരണം:
```bash
git push origin main
```

####_PULL ചെയ്യുന്നതിനുള്ള നടപടികൾ
##### 1. ലോക്കൽ മാറ്റങ്ങൾ_commit ചെയ്യുക
##### 2. മാറ്റങ്ങൾ ഫെച്ചുചെയ്യുക
```bash
git fetch origin
```
##### 3. മാറ്റങ്ങൾ മെർജ് ചെയ്യുക
```bash
git merge origin/main
```

### മേർജ് സംഘർഷങ്ങൾ കൈകാര്യം ചെയ്യൽ
മറ്റൊരു ഡെവലപ്പർ അതേ ഫയൽ തിരുത്തിയിട്ടുണ്ടെങ്കിൽ, Git-ന് സ്വയം പരിഹരിക്കാനാകാത്ത സംഘർഷങ്ങൾ ഉണ്ടാകാം. ഈ പ്രശ്നങ്ങൾ പരിഹരിക്കാൻ:
1. സംഘർഷമുള്ള ഫയലുകൾ തുറക്കുക.
2. ആവശ്യമായ മാറ്റങ്ങൾ കൈവശമാക്കി, സംഘർഷ ചിഹ്നങ്ങൾ നീക്കം ചെയ്യുക.
3. പരിഹരിച്ച മാറ്റങ്ങൾ commit ചെയ്യുക.
```bash
git add <conflicted_file>
git commit -m "Resolved merge conflict"
```

### മികച്ച ശീലങ്ങൾ
- **Push ചെയ്യുന്നതിന് മുമ്പ്_PULL ചെയ്യുക:** സംഘർഷങ്ങൾ ഒഴിവാക്കാൻ.
- **അവസാന commit-ന് സാർവത്രികമായ commit message നൽകുക.**
- **Feature branches ഉപയോഗിക്കുക:** പുതിയ സവിശേഷതകൾ വികസിപ്പിക്കുമ്പോൾ.
- **Code review നിർബന്ധമാക്കുക:** ടീം അംഗങ്ങൾ തമ്മിൽ തിരുത്തലുകൾ പങ്കിടാൻ.
- **CI/CD ഉപയോഗിക്കുക:** കോഡ് ടെസ്റ്റിംഗ്, ഇൻറഗ്രേഷൻ ഓട്ടോമേറ്റുചെയ്യാനായി.

GitHub, GitLab, Bitbucket എന്നിവ ഉപയോഗിച്ച് ദൂരസ്ഥ റിപ്പോസിറ്ററികൾ ക്രമീകരിക്കാനും അവയിൽ മാറ്റങ്ങൾ കൈകാര്യം ചെയ്യാനും ഈ മാർഗ്ഗനിർദ്ദേശങ്ങൾ ഉപകാരപ്രദമായിരിക്കും.

