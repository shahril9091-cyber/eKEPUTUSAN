# eKEPUTUSAN

Aliran: index.html → Firebase Realtime Database. Tiada Firebase Authentication, e-mel, UID atau server tambahan.

## Aktifkan

1. Buka Firebase Console, projek sksj-2026.
2. Kekalkan Rules Firebase sedia ada: { "rules": { ".read": true, ".write": true } }. Tiada Rules tambahan atau perubahan diperlukan.
3. Buka laman sistem melalui HTTP/HTTPS. Pergi Admin dan gunakan kata laluan asal sksj.
4. Tambah rekod atau Import Pukal. Rekod disimpan di ekeputusan/results/{mykid}/{id}.
5. Semak MyKid daripada peranti lain untuk mengesahkan sambungan.

## Akses database

Rules mengekalkan bacaan dan penulisan awam pada root seperti konfigurasi asal projek supaya sistem lain terus berfungsi. Validasi input dibuat dalam HTML; tiada validasi tambahan dalam Firebase Rules. Kata laluan dalam HTML hanya mengawal paparan admin; ia tidak melindungi database daripada bacaan, perubahan atau pemadaman melalui API secara terus.

## Data lama

Data localStorage asal tidak dipadam atau dimigrasi automatik. Eksport CSV daripada versi lama, kemudian import ke versi Firebase.

Rules asal dikekalkan. Ujian sambungan sebenar perlu dibuat melalui sistem.
