# syncdate-openwrt-for-modemhp
Auto sync date openwrt with pick date data from modem hp

- Sebagian source didapat dari @Teguh Surya Mungaran(silahkan bisa kunjungi FB nya)

- Jangan lupa install dahulu adb di openwrt

- Pastikan bahwa modem hp sudah bisa di kontrol dari openwrt via adb. Untuk mengecek nya bisa ketik adb devices,jika tidak ada tulisan unauthorized maka bisa dipastikan script ini sudah bisa berjalan 

- Paste command ini di terminal openwrt anda

wget --no-check-certificate "https://raw.githubusercontent.com/vitoharhari/syncdate-openwrt-for-modemhp/main/syncdate-hp" -O /usr/bin/syncdate-hp && chmod +x /usr/bin/syncdate-hp

- lalu masukkan command ini di Luci, masukkan di system>startup>local startup ,atau jika di terminal di rc.local

/usr/bin/syncdate-hp

- pastikan command diatas di letakkan di atas tulisan exit 0
