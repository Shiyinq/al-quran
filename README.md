# Al-quran

Wrapper Javascript for API Fatimah Bot - alQuran. For more information about the API Fatimah, please visit the [Fatimah](https://fathimah.docs.apiary.io/#reference/alquran) documentation.

# Instalation

```cli
npm i al-quran
```
# Usage

```javascript
const alquran = require('al-quran')
```

## Methods

```javascript
alquran.surat()
alquran.nomorSurat(nomor)
alquran.tampilAya(surat, ayat)
alquran.bahasaAyat(surat, ayat, bahasa)
alquran.daftarBahasa()
alquran.pencarian(kata, mulai, limit, bahasa)
alquran.catatanDepag(nomor)
alquran.quranAcak()
```

about parameter see [Fatimah](https://fathimah.docs.apiary.io/#reference/alquran)


## Example Request

```javascript
const alquran = require('al-quran')

alquran.surat()
  .then(data => {
    console.log(data)
  })
  .catch(error => {
    console.log(error)
  })
```
