Xiaomi redmi note 4 mediatek nikel 
dicharger nggak ada respon sama sekali. Tapi dilihat dari usb tester, arus pengisian naik. 
eks janda. 
Cek portUSB ok. 
cek batre ok. 
Coba ganti ic charger bq24196, masih sama. 
Buka skema, ternyata hilang Resistor R616
Ganti dengan yang nilainya 1k ( bawaan 1k5 ohm), masih sama. 
Cek hambatan dalam pada titik atas R tersebut, yang mengarah ke pmic, terukur 0.010.
Coba angkat pmic mt6351v, ukur hambatan dalam pada titik tadi, terukur tanpa hambatan dalam. 
Ganti ic power dengan yang baru, ukur lagi pada titik R tadi, terukur 0.400. 
Coba dicharger pada posisi mati maupun dinyalakan, alhamdulillah pengisian masuk, indikator normal, arus pengisian juga stabil. 
Karena penasaran, ganti ic charger pakai yang lama, barangkali masih bisa dipakai. Eh ternyata memang harus ganti juga, arus pengisian masuk, tapi tertahan pada ic charger, tidak keluar ke Vbatt.