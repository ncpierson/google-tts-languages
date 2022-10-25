# Playdown Suara Google Text to Speech

> :warning: This repo is deprecated and replaced by [google-translate-tts](https://github.com/ncpierson/google-translate-tts)

Untuk membuat suara Google, kamu juga bisa menggunakan Playdown.id yang di dalamnya tersedia berbagai bahasa. Untuk memanfaatkan situs ini, berikut tutorial selengkapnya:

- Aktifkan data di smartphone lalu akses browser yang di install di smartphone.
- Jika pakai Google, kamu bisa akses situs berikut https://www.playdown.id/ 
- Ketikkan kata-kata di bagian kolom teks yang ada di bagian atas.
- Pilihlah bahasa di bagian voice sesuai kata yang diketikkan. 
- Kamu bisa klik play lalu dengarkan hasil suaranya.
- Jika sudah sesuai kamu bisa klik download lalu simpan di smartphone. 

Untuk suara Google yang ada di situs ini hanya wanita saja dan tidak bisa memilih. Hanya saja varian bahasanya sangat lengkap mulai dari bahasa Indonesia, Jawa dan bahasa asing seperti India, Jerman, Italy, Korea, dan Jepang. 

You can find a list of Google text to speech engine at https://suaragoogle.readthedocs.io

# Install

```
yarn add google-tts-languages
```

# Usage

```js
const languages = require('google-tts-languages');

console.log(languages);

/*
[ { code: 'af-ZA', name: 'Afrikaans' },
  { code: 'sq', name: 'Albanian' },
  { code: 'ar-AE', name: 'Arabic' },
  ...
  ]
 */

const name = languages.findByCode('es-MX').name;            // Spanish (Mexico)
const code = languages.findByName('Spanish (Mexico)').code; // es-MX
```

I highly recommend just looking at `index.js`. It is very easy to understand.
