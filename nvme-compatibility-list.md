### NVMe compatibility list

Before launching our board we concluded extensive testing to ensure compatibility with the most popular drives. If you want to use a different drive it will mostly likely work without any issues. Our compatibility list also includes performance benchmarks made with the tool provided by [pibenchmarks.com](https://pibenchmarks.com)

When purchasing a drive please make sure that you purchase a NVMe drive, not a SATA drive!

### Compatible drives

|Name|DD Write|HDParam(disk)|Score (pibenchmarks)|
|---|---|---|---|
|Western Digital SN530|441 MB/s|845.35 MB/s|45,735|
|Samsung 970 EVO Plus|314 MB/s|776.7 MB/s|27,960|
|Sabrent Rocket 4.0|350 MB/s|773.9 MB/s|47,002|
|Crucial P3 Plus M.2 Series|441 MB/s|798.97 MB/s|40,118|
|PNY CS1030|444 MB/s|744.15 MB/s|42,203|
|Samsung 980|426 MB/s|791.31 MB/s|42,230|
|Lexar NM620|444 MB/s|849.2 MB/s|44,542|
|Crucial P3 Plus|359 MB/s|777.5 MB/s|26,163|
|KIOXIA EXCERIA|394 MB/s|802.09 MB/sec|43030|
|Lexar NM710|393 MB/s|849.91 MB/sec|40542|
|Kingston KC3000|393 MB/s |832.70 MB/sec|44203|
|XPG GAMMIX S70 BLADE|403 MB/s |829.90 MB/sec |41316|


### Not compatible drives

WD SN530 has been problematic for some users when it comes to NVMe boot, especially in the 2242 variant. Our test drive was a 2280 SKU and it worked OK but we generally recommend staying away from Western Digital drives completely. 

- WD SN740
- WD SN350
- WD SN770
- WD SN850 [possibly](https://github.com/raspberrypi/linux/issues/5217)

Those three drives also do not work on the Compute Module 4 and they share the same PCB layout. 
