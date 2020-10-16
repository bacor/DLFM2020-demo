DLfM2020 Demo of chant21 and two plainchant corpora
===============================================

A demo for our paper
['Studying Large Plainchant Corpora Using chant21'](https://doi.org/10.1145/3424911.3425514)
presented at the
[Digital Libraries for Musicology 2020](https://dlfm.web.ox.ac.uk/) conference.
In the demo we show how you can work with the
[CantusCorpus](https://github.com/bacor/cantuscorpus), 
[GregobaseCorpus](https://github.com/bacor/gregobasecorpus) 
and the Python package [Chant21](https://github.com/bacor/chant21).

Setup
-----

I'm running these jupyter notebooks in a fresh Python environment; my setup is as follows:
```bash
pyenv local 3.7.6
python -m venv env
source env/bin/activate
```

These are the required packages:

```bash
pip install chant21 music21==5.7.2 jupyterlab matplotlib pandas numpy scipy
```

Note that I haven't tested chant21 with music21 v6 yet, and there seem to be some issues with the HTML previews there.


Next, download the [CantusCorpus](https://github.com/bacor/cantuscorpus/releases/tag/v0.2)
and [GregoBaseCorpus](https://github.com/bacor/gregobasecorpus/releases/tag/v0.4) and unzip these in a directory `data` directory:

```
- data
    - cantuscorpus-v0.2
        - README.md
        - corpus-generation.log
        - csv
            - ...
    - gregobasecorpus-v0.4
        - README.md
        - corpus-generation.log
        - csv
            - ...
        - gabc
            - 00001.gabc
            - 00002.gabc
            - ...
        - html
            - 00001.html
            - 00002.html
            - ...
```

Then:

```bash
jupyter lab
```

And that should be it!
