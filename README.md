# scummvm-bra-engine

Modifiche al motore [ScummVM](https://github.com/scummvm/scummvm) (motore *parallaction*) per un progetto
amatoriale e non ufficiale su *The Big Red Adventure*, firmato Marketto: grafica HD e 16:9, testi HD, voci, aiuti, manuale, salvataggi e altro.

Questo repository contiene **solo il codice del motore**, sotto licenza GPL v3 come ScummVM (vedi `COPYING`).
Non contiene file del gioco né contenuti derivati: per giocare serve una copia originale del gioco.

## Come si applica

```sh
git clone https://github.com/scummvm/scummvm.git
cd scummvm
git checkout 0b24b9b5b0caa395a68bde42e7508a3544d34533   # commit in SCUMMVM_COMMIT
git apply ../scummvm-bra-engine/patches/*.patch
```

Poi si compila come ScummVM (`./configure --enable-engine=parallaction && make`).
