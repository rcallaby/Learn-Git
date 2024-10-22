**Git کی تاریخ اور بنیادیں**
تعارف  
Git کس نے بنایا؟  
Git کیوں بنایا گیا؟  
Git کے متبادلات  
کہاں پر اپنے repositories مفت میں محفوظ کریں؟  

**تعارف**  
Git ایک distributed version control system ہے جسے Linus Torvalds نے 2005 میں بنایا تھا۔ Git تاریخ کو centralized version control systems (CVCS) جیسے کہ Team Foundation Version Control, Perforce، یا Subversion سے بالکل مختلف طریقے سے محفوظ کرتا ہے۔ Centralized systems میں ہر فائل کی الگ تاریخ محفوظ کی جاتی ہے، جب کہ Git پورے repository کی snapshots کو محفوظ کرتا ہے۔ یہ snapshots Git میں "commits" کہلاتے ہیں، اور ان کے کئی والدین ہو سکتے ہیں، جس سے تاریخ ایک سیدھی لائن کے بجائے گراف کی شکل میں بنتی ہے۔ CVCS استعمال کرنے والے اکثر صارفین Git کو اسی فرق کی وجہ سے پیچیدہ سمجھتے ہیں۔

Git آج کے دور میں سیکھنا ضروری ہے کیونکہ یہ دنیا بھر کے developers اور کمپنیوں میں وسیع پیمانے پر استعمال ہوتا ہے۔ یہ کوڈ میں تبدیلیاں سنبھالنے اور دوسرے developers کے ساتھ مل کر کام کرنے کے لیے ایک اہم ٹول ہے۔ Git developers کو کوڈ پر آزادانہ طور پر کام کرنے اور پھر اپنی تبدیلیاں ایک ساتھ merge کرنے کی اجازت دیتا ہے۔

**Git کس نے بنایا؟**  
Git کو اصل میں Linus Torvalds نے 2005 میں Linux kernel کی ترقی کے لیے بنایا تھا۔ اس کے بعد دوسرے kernel developers نے اس کی ابتدائی ترقی میں اپنا حصہ ڈالا۔ Junio Hamano 2005 سے اس کے core maintainer ہیں۔

**Git کیوں بنایا گیا؟**  
اصل ٹیم BitKeeper، ایک پچھلا version control system، استعمال نہیں کر سکتی تھی کیونکہ انہیں اسے مفت استعمال کرنے کا لائسنس کھو دیا گیا تھا۔ اس وقت کوئی اور Source Control Management (SCM) ایسا نہیں تھا جو distributed system کے لیے ان کی مخصوص ضروریات کو پورا کرتا۔ نئے system کے کچھ مقاصد تیز رفتار، سادہ ڈیزائن، غیر لکیری ترقی کی مضبوط حمایت (ہزاروں parallel branches)، مکمل طور پر distributed اور Linux kernel جیسے بڑے projects کو مؤثر طریقے سے سنبھالنے کے قابل ہونا تھا۔

**Git کے متبادلات**  
Git کے کئی متبادلات موجود ہیں، جن میں شامل ہیں: Subversion (SVN), Mercurial (Hg), اور Perforce۔

Subversion ایک centralized version control system ہے جو CVS سے مشابہت رکھتا ہے۔ یہ اکثر enterprise environments میں استعمال ہوتا ہے کیونکہ اسے استعمال کرنا آسان ہے اور دوسرے tools کے ساتھ اچھی integration فراہم کرتا ہے۔

Mercurial ایک distributed version control system ہے جو Git سے مشابہت رکھتا ہے۔ یہ اکثر چھوٹے projects میں استعمال ہوتا ہے کیونکہ اسے سیکھنا Git کے مقابلے میں آسان ہے۔

Perforce ایک centralized version control system ہے جو اکثر enterprise environments میں استعمال ہوتا ہے۔ یہ بڑی فائلوں اور binary files کے لیے اچھا support فراہم کرتا ہے۔

ان میں سے ہر ایک system کے اپنے فوائد اور نقصانات ہیں، اور کس کا انتخاب کرنا ہے یہ project کی مخصوص ضروریات پر منحصر ہوتا ہے۔ Git دنیا بھر میں developers اور کمپنیوں میں وسیع پیمانے پر استعمال ہوتا ہے کیونکہ یہ کوڈ کی تبدیلیوں کو سنبھالنے اور دوسرے developers کے ساتھ مل کر کام کرنے کا ایک اہم tool ہے۔

**کہاں پر اپنے repositories مفت میں محفوظ کریں؟**  
انٹرنیٹ پر کئی ایسی جگہیں ہیں جہاں آپ اپنے Git repositories کو مفت میں محفوظ کر سکتے ہیں۔ یہاں کچھ مشہور خدمات ہیں:

- GitHub  
- GitLab  
- Bitbucket  
- SourceForge  

ان میں سے ہر ایک کی اپنی خوبیاں اور خامیاں ہیں، اور project کی مخصوص ضروریات کے مطابق انتخاب کیا جاتا ہے۔ GitHub سب سے زیادہ مقبول سروس ہے اور دنیا بھر میں developers اور کمپنیوں کے ذریعے وسیع پیمانے پر استعمال ہوتی ہے۔ یہ مفت میں public repositories کی لامحدود تعداد اور private repositories کی محدود تعداد فراہم کرتی ہے۔

GitLab ایک اور مقبول سروس ہے جو مفت میں unlimited private repositories فراہم کرتی ہے۔ Bitbucket ایک سروس ہے جو اکثر چھوٹی ٹیموں کے ذریعے استعمال کی جاتی ہے کیونکہ یہ پانچ users تک کے لیے مفت میں unlimited private repositories فراہم کرتی ہے۔ SourceForge ایک پرانی سروس ہے جو اکثر open source projects کے لیے استعمال ہوتی ہے۔