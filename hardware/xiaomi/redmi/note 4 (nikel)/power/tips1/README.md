## issue : janda, dicharger nggak ada respon sama sekali. Tapi dilihat dari usb tester, arus pengisian naik.
## step
1. Cek portUSB ok.
2. cek batre ok.
3. Coba ganti ic charger bq24196, masih sama. 
4. Buka skema, ternyata hilang Resistor R616
5. Ganti dengan yang nilainya 1k ( bawaan 1k5 ohm), masih sama. 
6. Cek hambatan dalam pada titik atas R tersebut, yang mengarah ke pmic, terukur 0.010.
7. Coba angkat pmic mt6351v, ukur hambatan dalam pada titik tadi, terukur tanpa hambatan dalam. 
8. Ganti ic power dengan yang baru, ukur lagi pada titik R tadi, terukur 0.400. 
9. Coba dicharger pada posisi mati maupun dinyalakan, alhamdulillah pengisian masuk, indikator normal, arus pengisian juga stabil. 
10. Karena penasaran, ganti ic charger pakai yang lama, barangkali masih bisa dipakai. Eh ternyata memang harus ganti juga, arus pengisian masuk, tapi tertahan pada ic charger, tidak keluar ke Vbatt.