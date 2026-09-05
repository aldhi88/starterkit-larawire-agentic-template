# Starterkit Larawire Agentic Templates

Repository ini menyimpan archive runtime minimum untuk theme yang didukung oleh
[`aldhi88/starterkit-larawire-agentic`](https://github.com/aldhi88/starterkit-larawire-agentic).

Archive open-source di repository ini dapat diunduh otomatis oleh wizard
`starter:install`; Vuexy adalah archive lokal/privat yang tidak dipublikasikan.
Installer memvalidasi ukuran, SHA-256, keamanan path ZIP, dan kecocokan seluruh
file dengan asset manifest package sebelum melakukan perubahan pada project
Laravel.

## Theme tersedia

| Theme | Archive | Lisensi |
|---|---|---|
| Tabler | `tabler.zip` | MIT |
| DashCode | `dashcode.zip` | Commercial; lisensi dimiliki owner untuk penggunaan internal tim |
| Vuexy 3.0.0 | `vuexy.zip` (lokal/privat, tidak dipublikasikan) | Commercial; penggunaan pribadi/internal owner |

Vuexy menggunakan source lokal berlisensi, bukan downloader publik. Archive
`vuexy.zip` diabaikan Git; verifikasi dengan `shasum -a 256 -c VUEXY_SHA256SUMS`.
Ekstrak archive milik owner ke `theme-intake/vuexy/` pada host lokal sebelum
memilih Vuexy di installer. Archive berisi `runtime/`; installer memvalidasi
hash setiap file sebelum publikasi ke `public/assets/vuexy/`. Archive minimum
ini berisi 10 file, termasuk custom integration pair `css/vuexy.css` dan
`js/vuexy.js`. Integrasi package,
fresh host, kedua layout, dan browser responsive sudah diverifikasi pada
2026-09-05.

Archive hanya berisi dependency runtime minimum. Demo HTML, source build, dan
komponen yang tidak digunakan tidak disertakan. Lisensi repository ini tidak
menggantikan lisensi upstream setiap theme. Archive DashCode disediakan untuk
instalasi project internal tim yang berada di bawah lisensi owner; lihat
`THIRD_PARTY_NOTICES.md`. The Vuexy archive was rebuilt and verified against
the package asset manifest on 2026-09-05; it remains private/local and is not
an installer download URL.

Semua archive theme menyediakan custom integration pair bernama
`css/<theme-key>.css` dan `js/<theme-key>.js`. Pair tersebut hanya mengadaptasi
kosmetik dan runtime vendor; layout, hierarki, inventaris komponen, urutan,
grouping, penempatan, dan density halaman tetap sama lintas theme.
Pemilihan kosmetik wajib memakai varian native theme yang paling sesuai dengan
fungsi komponen. Warna mengikuti arti yang konsisten—primary untuk aksi/fokus,
success untuk status berhasil, info untuk panduan, warning untuk perhatian,
danger untuk aksi merusak/error, dan secondary untuk metadata netral—dengan
foreground yang tetap terbaca pada setiap tint.
