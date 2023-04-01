![bu yerda rasm bor](https://realpython.com/cdn-cgi/image/width=960,format=auto/https://files.realpython.com/media/Python-Imports_Watermarked.ae72c8a00197.jpg)
# Python import: Ilg'or Texnikalar va Maslahatlar
## Mundarija jadvali
* [Asosiy Python import](https://github.com/ShodmonovZafar/import_python#asosiy-python-import)
    + [Modullar](https://github.com/ShodmonovZafar/import_python#modullar)
    + Paketlar
    + Mutloq va Nisbiy Import
    + Python Import Yo'li
    + 5
    + 6
    + 7
    + 8
* [Resurs Importi](https://github.com/ShodmonovZafar/import_python#resurs-importi)
    + 1
    + 2
    + 3
* [Dinamik Import](https://github.com/ShodmonovZafar/import_python#dinamik-import)
    + 1
    + 2
    + 3
* [Python Import Tizimi](https://github.com/ShodmonovZafar/import_python#python-import-tizimi)
    + 1
    + 2
    + 3
    + 4
    + 5
    + 6
* [Import bo'yicha Maslahatlar va Fokuslar](https://github.com/ShodmonovZafar/import_python#import-boyicha-maslahatlar-va-fokuslar)
    + 1
    + 2
    + 3
    + 4
    + 5
    + 6
    + 7
* [Xulosa](https://github.com/ShodmonovZafar/import_python#xulosa)

Pythonda siz bir **modul**dagi kodni boshqa modulda mavjud qilish uchun `import` kalit so'zidan foydalanasiz. Pythonda import qilish **kodingizni samarali tarzda tuzish** uchun muhimdir. Importdan to'g'ri foydalanish sizni yanada samaraliroq qiladi, bu sizning loyihalaringizni saqlab turishda kodni qayta ishlatishga imkon beradi.

Ushbu qo'llanma Pythonning `import` bayonoti va uning qanday ishlashi haqida to'liq ma'lumot beradi. Import tizimi kuchli va siz bu quvvatdan qanday foydalanishni o'rganasiz. Pythonning import tizimi ortidagi ko'plab tushunchalarni qamrab olgan bo'lsangizda, ushbu qo'llanma asosan misol uchun asoslangan. Siz bir nechta kod misollaridan o'rganasiz.

**Ushbu qo'llanmada siz qanday qilishni o'rganasiz:**
* **Modullar**, **paketlar** va **nomlar maydoni paketlar**idan foydalaning
* Paketlaringiz ichidagi **resurslar** va **ma'lumotlar fayllar**ini ishlating
* Ish vaqtida modullarni **dinamik** ravishda import qiling
* Python import tizimini **moslashtiring**

<!-- https://realpython.com/bonus/python-import/ -->
O'quv qo'llanmasida siz Python import uskunalari bilan samarali ishlash uchun qanday o'ynash haqida misollarni ko'rasiz. Barcha kodlar o'quv qo'llanmasida ko'rsatilgan bo'lsada, siz uni quyidagi katakchani bosish orqali ham yuklab olishingiz mumkin:
> Manba kodini oling: Ushbu qo'llanmada Python import tizimi haqida ma'lumot olish uchun foydalanadigan manba kodini olish uchun [shu yerni bosing](https://realpython.com/bonus/python-import/).

## Asosiy Python import
Python kodi [ham modullarga, ham paketlar](https://github.com/ShodmonovZafar/modules_and_packages#modules_and_packages)ga ajratilgan. Ushbu bo'limda ular qanday farq qilishlari va ular bilan qanday ishlashingiz mumkinligi tushuntiriladi.

Keyinchalik qo'llanmada siz Python import tizimining ba'zi ilg'or va kam ma'lum bo'lgan foydalanishlarini ko'rasiz. Biroq, keling, asosiy narsalardan boshlaylik: modullar va paketlarni import qilish.

### Modullar

[Python.org glossary](https://docs.python.org/glossary.html) **modul**ni quyidagicha belgilaydi(ta'riflaydi):
> Python kodining tashkiliy birligi bo'lib xizmat qiladigan ob'ekt. Modullar ixtiyoriy Python obyektlarini o'z ichiga olgan nom maydoniga ega. Modullar Python-ga import qilish orqali yuklanadi. ([Manba](https://docs.python.org/glossary.html#term-module))

Amalda, modul odatda Python kodini o'z ichiga olgan bitta `.py` fayliga mos keladi.

Modullarning haqiqiy kuchi shundaki, ularni import qilish va boshqa kodlarda qayta ishlatish mumkin. Quyidagi misolni ko'rib chiqing:
```
>>> import math
>>> math.pi
3.141592653589793
```
Birinchi qatorda `import math` qiling, siz [**math**](https://realpython.com/python-math-module/) moduldagi kodni **import** qilasiz va undan foydalanishga ruxsat berasiz. Ikkinchi qatorda siz `math` moduldagi `pi` [o'zgaruvchi](https://realpython.com/python-variables/)siga kirasiz. `math` **Python standart kutubxona**sining bir qismidir, ya'ni Python bilan ishlayotganingizda uni import qilish har doim mavjud.

E'tibor bering, siz shunchaki `pi` emas, balki `math.pi` yozasiz. `math` modul bo'lishdan tashqari, `math` modulning barcha atributlarini birga saqlaydigan **nommaydoni** vazifasini bajaradi. **Nommaydoni** kodingizni o'qilishi va tartibli saqlash uchun foydalidir. Tim Peters so'zlari bilan aytganda:

> Nommaydonlari - bu ajoyib g'oya - keling, ulardan ko'proq narsani qilaylik! ([Manba](https://www.python.org/dev/peps/pep-0020/))

Siz `dir()` yordamida nomlar maydoni tarkibini ro'yxatga olishingiz mumkin:
```
>>> import math
>>> dir()
['__annotations__', '__builtins__', ..., 'math']

>>> dir(math)
['__doc__', ..., 'nan', 'pi', 'pow', ...]
```


## Resurs Importi
## Dinamik Import
## Python Import Tizimi
## Import bo'yicha Maslahatlar va Fokuslar
## Xulosa
