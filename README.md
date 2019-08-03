# qq-tr-free

Qq translate for free -- local cache plus throttling (1.5 calls/s from 1001st call on). Let's hope it lasts.

### Installation
``` pip install qq-tr-free -U```

or
* Install (pip or whatever) necessary requirements, e.g. ```
pip install requests_cache jmespath
fuzzywuzzy``` or ```
pip install -r requirements.txt```
* Drop the file qq_tr.py in any folder in your PYTHONPATH (check with import sys; print(sys.path)
* or clone the repo (e.g., ```git clone https://github.com/ffreemt/qq-tr-free.git``` or download https://github.com/ffreemt/qq-tr-free/archive/master.zip and unzip) and change to the qq-tr-free folder and do a ```
python setup.py develop``` or ```
python setup.py install```

### Usage

```
from qq_tr import qq_tr
print(qq_tr('hello world'))  # -> '你好世界'
print(qq_tr('hello world', to_lang='de'))  # ->'Hallo Welt'
print(qq_tr('hello world', to_lang='fr'))  # ->'Salut tout le monde'
print(qq_tr('hello world', to_lang='ja'))  # ->'ハローワールド'
```

### Acknowledgments

* Thanks to everyone whose code was used