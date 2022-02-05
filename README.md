# Al-quran

Wrapper Javascript for API Fathimah Bot - alQuran. For more information about the API Fathimah Bot, please visit the [Fathimah](https://fathimah.docs.apiary.io/#reference/alquran) documentation.

# Instalation

```cli
npm i al-quran
```
# Usage

```javascript
const alQuran = require('al-quran')
```

## Methods

```javascript
alQuran.surat()
alQuran.nomorSurat(nomor)
alQuran.tampilAyat(surat, ayat)
alQuran.bahasaAyat(surat, ayat, bahasa)
alQuran.daftarBahasa()
alQuran.pencarian(kata, mulai, limit, bahasa)
alQuran.catatanDepag(nomor)
alQuran.quranAcak()
```

about parameter see [Fathimah](https://fathimah.docs.apiary.io/#reference/alquran)


## Example Request

```javascript
const alQuran = require('al-quran')

alQuran.surat()
  .then(data => {
    console.log(data)
  })
  .catch(error => {
    console.log(error)
  })
```
