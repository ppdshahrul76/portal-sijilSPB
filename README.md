# Portal Sijil Digital PPDHS

## Fail GitHub

Upload `index.html` dan `README.md` ke repository GitHub. Jangan upload `Code.gs` ke repository public.

## Backend Google Apps Script

1. Gantikan Code.gs lama dengan fail `Code.gs` yang disediakan.
2. Apps Script > Project Settings > Script Properties, tambah:

   * `ADMIN\_EMAIL` = email admin anda
   * `ADMIN\_PASSWORD` = kata laluan admin baharu
3. Deploy > New deployment > Web app.
4. Execute as: Me.
5. Who has access: Anyone (diperlukan supaya GitHub Pages boleh memanggil API).
6. Authorize dan salin URL yang berakhir `/exec`.
7. Dalam `index.html`, cari `PASTE\_APPS\_SCRIPT\_WEB\_APP\_URL\_HERE` dan gantikan dengan URL `/exec` tadi.

## GitHub Pages

1. Cipta repository baharu.
2. Upload `index.html` dan `README.md`.
3. Settings > Pages.
4. Source: Deploy from a branch.
5. Branch: `main`, folder `/ (root)`.
6. Save dan tunggu GitHub Pages diterbitkan.

## Nota keselamatan

* Jangan letak kata laluan admin di `index.html` atau repository GitHub.
* Backend menggunakan Script Properties untuk semakan admin.
* Fungsi padam memerlukan ID dan kata laluan admin.

