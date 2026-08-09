# BuatQris QRIS Tester — FIXED

Mengikuti contoh integrasi pada dokumentasi BuatQris:
- Endpoint: https://api.buatqris.site
- Create: action=qris_create
- Check: action=qris_check_status
- QR method default: qris_two
- Webhook: /api/payment/webhook

Deploy seluruh folder ke GitHub lalu import ke Vercel.

Setelah deploy, masukkan:
https://DOMAIN-KAMU/api/payment/webhook
ke menu Webhook / Callback BuatQris.

Untuk signature verification, buat Vercel Environment Variable:
BUATQRIS_SIGNING_SECRET=whsec_...

Jangan commit Secret Token atau Signing Secret ke GitHub.
