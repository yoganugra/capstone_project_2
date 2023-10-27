# SaaS Sales

Dalam capstone project ini, saya akan memposisikan diri saya sebagai data analis di sebuah perusahaan. Berdasarkan data yang diperoleh, saya akan membuat serangkaian pertanyaan berdasarkan kebutuhan bisnis dan masalah yang mungkin dihadapi perusahaan. Saya akan menjawab pertanyaan bisnis yang saya buat, membuat cerita dan visualisasi, serta menyajikan wawasan dari analitis yang ditemukan agar dapat digunakan oleh pemangku kepentingan dalam pengambilan keputusan bisnis.

Tableau Story Link : [Disini](https://public.tableau.com/shared/QXJ9JNRC9?:display_count=n&:origin=viz_share_link)

## Latar Belakang

Sebuah perusahaan yang bergerak di bidang penjualan produk perangkat lunak kepada perusahaan lain (B2B) bekerja sama dengan seorang *data analyst* untuk menganalisa data yang perusahaan miliki. Perusahaan menemukan adanya penurunan nilai *profit* ketika nilai *sales* mengalami kenaikan, atau sebaliknya. Perusahaan juga ingin mengetahui efektifitasnya dalam pengelolaan biaya untuk mendapatkan *profit* atas *sales* saat ini, dan upaya untuk meningkatan keefektifitasannya di masa mendatang.

## Pernyataan Masalah

Perusahaan ingin mengetahui **seberapa efektif perusahaan dalam mengelola biaya dan menghasilkan laba bersih (profit) yang lebih tinggi atas pendapatannya (sales) melalui nilai net profit margin**.

Analisis ini nantinya dapat membantu perusahaan untuk meningkatkan kinerja perusahaan berdasarkan besarnya persentase laba bersih atas penjualan bersih, yang nantinya, perusahaan dapat mengetahui posisi perusahaan tersebut dibandingkan dengan rata-rata industrinya ketika sudah mengetahui nilai rata-rata industrinya.

Sebagai seorang *data analyst*, kita akan mencoba membantu perusahaan dengan menjawab pertanyaan berikut:

1. Bagaimana kondisi nilai *net profit margin* perusahaan saat ini?
    - Berapa nilai *net profit margin* perusahaan saat ini?
    - Berapa proporsi perbandingan, dan jumlah *profit*, *neutral* dan *loss* berdasarkan transaksi perusahaan saat ini?
    - Bagaimana perkembangan *sales* dan *profit* perusahaan sampai ini?
<br><br>
2. Apa hal yang mempengaruhi nilai *net profit margin*?
    - Bagaimana pengaruh kolom numerik terhadap nilai profit?
    - Kolom apa yang menyebabkan penurunan nilai profit dan bagaimana kolom tersebut memengaruhi nilai net profit margin?
<br><br>
3. Apa upaya yang bisa dilakukan untuk meningkatkan nilai *profit*?
    - Berapa jumlah sales dan profit berdasarkan produknya?
        - Produk mana yang memberikan margin profit tertinggi dan terendah?
        - Bagaimana kondisi pemberian discount terhadap product dengan margin tertinggi dan terendah?
    - Berapa jumlah sales dan profit berdasarkan industri customer tergabung?
        - Industri customer tergabung mana yang menyumbangkan profit terendah?
        - Produk apa yang memberikan margin terendah pada industri customer tergabung dengan penyumbang profit terebdah tersebut?
    - Berapa jumlah sales dan profit berdasarkan region?
        - Region mana yang menyumbangkan profit tertinggi dan terendah?
        - Kota mana yang merupakan kota terprofitable dan tidak profitable pada region penyumbang profit terendah?
        - Berapa jumlah profit dan loss produk terjual berdasarkan region?
<br><br>
4. Bagaimana kondisi dan persebaran kolom numerikal pada setiap negara?
    - Negara mana yang memberikan total sales terbesar?
    - Negara mana yang memberikan total profit terbesar?
    - Negara mana yang diberikan discount profit terbesar?
    - Negara mana yang membeli produk dengan quantity terbanyak?
<br><br>
5. Bagimana engagement dari pembeli dari waktu ke waktu?
<br><br>
6. Hal apa yang perlu dipertimbangkan dalam pemberian discount?
    - Bagaimana karakteristik customer loyal?
    - Siapa customer dengan total pembelian dan pengulangan pembelian terbanyak?

  ## Kesimpulan
  
1. Kondisi nilai *net profit margin* perusahaan.
    - Nilai *Net Profit Margin* didapatkan dari hasil bagi total nilai *Sales* dan total nilai *Profit*. Pada perusahaan ini, nilai *Net Profit Margin* sebesar 12.47%. Maknanya, dalam $1 atas *sales*, perusahaan ini memperoleh *profit* sebesar $0.12. 
    - Dari 9994 transaksi tercatat, sebanyak 8058 atau 80.63% memberikan keuntungan (Profit), sebanyak 1871 atau 0.65% tidak memberikan keuntungan maupun kerugian (Neutral) dan sisanya sebanyak 65 atau 18.72% memberikan kerugian (loss).
    - Fluktuasi *Sales* dan *Profit* terjadi sepanjang tahun selama 4 tahun berjalan. Terdapat beberapa kali penurunan *profit* ketika *sales* mengalami peningkatan seperti pada bulan Maret 2020, dan kondisi dimana *sales* turun, namun *profit* naik seperti pada bulan April 2020. Selain itu, terlihat pada bulan Juli 2020 dan Januari 2021, nilai *profit* turun bahkan sampai bernilai negatif dan menyebabkan kerugian (loss) sebesar -841.4826 dan -3281.0070.
<br><br>
2. Hal-hal yang memengaruhi nilai *net profit margin*.
    - *Sales* dan *Profit* menunjukkan hubungan positif moderat, semakin tinggi nilai *Sales*, maka semakin tinggi juga *Profit*-nya. *Quantity* dan *Profit* menunjukkan hubungan positif weak, semakin tinggi nilai *Quantity*, maka semakin tinggi juga *Profit*-nya. *Discount* dan *Profit* menunjukkan hubungan negatif lemah, semakin tinggi nilai *Discount*, maka semakin rendah *Profit*-nya. Maka, *Discount* menjadi satu-satunya variabel yang berpengaruh negatif terhadap *profit* (-0,22).
    - Secara keseluruhan, pemberian diskon kurang dari 30% masih memberikan keuntungan (profit), namun, pemberian diskon lebih dari itu memberikan kerugian (loss). Dari total 14 produk yang dijual, hanya ada 8 produk yang diberikan diskon lebih dari sama dengan 30%. Dari 8 produk dengan pemberian diskon lebih dari sama dengan 30%, hanya Big Ol Database (pemberian diskon 30%) dan Alchemy (pemberian diskon 40%) yang memberikan keuntungan (profit). Sisanya, memberikan kerugian (loss).
<br><br>
3. Analisis upaya peningkatan nilai *profit*.
    - Produk yang memberikan *total sales terbesar* adalah ContactMacher (410378.2650), sedangkan produk yang memberikan *total sales terendah* adalah Storage (3024.2800). Produk yang memberikan *total profit terbesar* adalah Alchemy (55617.8249), sedangkan produk yang memberikan *total profit terendah* (loss) adalah Marketing Suite (-3472.5560).
    - SaaS Connector Pack - Gold memberikan margin profit paling besar terhadap perusahaan, sedangkan Marketing Suite memberikan kerugian.
        - Nilai profit margin SaaS Connector Pack - Gold sebesar 42.27% artinya dalam $1 atas penjualan produk Marketting Suite, perusahaan memperoleh keuntungan sebesar $0.42. Produk SaaS Connector Pack - Gold hanya diberikan diskon 0 - 20%, sehingga masih bisa menghasilkan profit.
        - Nilai profit margin Marketing Suite sebesar -3.02% artinya dalam $1 atas penjualan produk Marketting Suite, perusahaan memperoleh kerugian sebesar $0.03. Produk Marketing Suite yang diberikan diskon 0 - 20% juga memberikan profit, namun, pemberian diskon lebih dari itu menyebabkan kerugian (loss).
    - Communications merupakan industri dimana customer tergabung dengan penyumbang nilai profit terkecil. 
        - Hal tersebut disebabkan karena nilai profit yang negatif atas penjualan produk marketing suite (-451.5362).
    - Region dengan Profit tertinggi adalah EMEA sedangkan region dengan profit terenda adalah APJ.
        - Pada region EMA, dari 14 produk yang dijual, hanya satu produk yang memberikan kerugian bagi perusahaan, yaitu Marketing Suite.
        - Pada region AMER, dari 14 produk yang dijual, terdapat lima produk yang memberikan kerugian bagi perusahaan, yaitu Marketing Suite, Contach Matcher, Saas Connector Pack, Oneview dan Big Ol Database.
<br><br>
4. Kondisi dan persebaran kolom numerikal pada setiap negara.
    - Nilai *sales* dan *profit* memiliki warna yang kurang lebih mirip di seluruh negara, dengan United States sebagai negara dengan total *sales* dan *profit* tertinggi.
    - Pemberian *discount* secara umum lebih didominasi oleh Prancis, Japan, dan Australia.
    - Negara dengan jumlah pembelian dengan *quantity* tertinggi adalah United States 
<br><br> 
5. Engagement pembeli dari waktu ke waktu
    - Secara garis besar, uktuk setiap cohort, persentase customer dari bulan ke bulan cukup fluktuatif, namun retensi pembelian dapat dikatakan bagus.
    - Customer yang melakukan transaksi pertama pada bulan Januari 2020 sampai bulan September 2020 cenderung terus melakukan pembelian ulang, bahkan di bulan Desember 2023 semua customer masih melakukan pembelian dengan persentase yang tinggi dan warna yang pekat.
    - Namun, dari gambar ini dapat ketahui bahwa customer baru hanya terdapat pada bulan Januari 2020 sampai September 2020. Artinya, dari bulan Oktober 2020 sampai Desember 2023 tidak ada customer baru.
    - Hal ini mungkin karena perusahaan menganggap bahwa biaya untuk retensi lebih murah dibandingkan dengan akuisi. Namun tetap saja terasa aneh apabila selama 3 tahun lebih tidak terdapat customer baru.
<br><br>
6. Efisiensi Pemberian Discount
    - Discount yang besar sebaiknya diberikan kepada customer yang loyal dengan syarat melakukan jumlah pembelian banyak dan pengulangan pembelian terbanyak juga.
    - Lima customer penyumbang sales terbanyak adalah Anthem (55719.2100), Ford Motor (43893.0424), Allianz (42904.1670), Bank of America Corp. (41255.9471), dan Valero Energy (41220.4188).
    - Lima customer dengan pengulangan pembelian terbanyak adalah Allianz (96), Ford Motor (95), Siemens (83), Tyson Foods (82), dan BNP Paribas (76).

  ## Saran

Saran-saran di bawah diharapkan dapat membantu perusahaan untuk meningkatkan nilai net profit margin dengan menurunkan nilai kerugian (loss).

1. Untuk meningkatan nilai Net Profit Margin, bisa dengan memperbesar proporsi keuntungan (profit) atau memperkecil proporsi kerugian (loss). Namun sebaiknya memperkecil proporsi kerugian agar tidak terdapat nilai negatif pada profit.
2. Profit bernilai negatif diasumsikan karena nilai sales yang didapatkan lebih kecil dari pada cost yang dikeluarkan. Pada data ini, tidak disediakan rincian cost untuk setiap transaksinya. Namun, setelah dianalisis, discount termasuk ke dalam cost dan berpengaruh negatif terhadap nilai profit.
3. Discount tentu dapat mendorong minat beli customer terhadap sebuah produk. Namun, setelah dianalisis, pemberian discount yang efektif hanya sampai 20%. Lebih dari itu, akan menyebabkan kerugian (loss). Maka, sebaiknya perusahaan lebih bijak dalam memberikan discount lebih dari 20%.
4. United States merupakan negara dengan total sales dan total profit tertinggi, sejalan dengan kuantitas pembelian. Namun berbanding terbalik dengan pemberian discount. Negara yang diberikan discount terbanyak adalah Prancis, Jepang, dan Australia. Jadi, sebaiknya perusahaan memberikan discount yang lebih rendah untuk nagara Prancis, Jepang, dan Australia dan discount yang lebih tinggi untuk pembelian dari United States.
5. Sepertinya perusahaan mementingkan retensi daripada akuisisi. Namun, dalam tiga tahun terakhir tidak ada customer baru akan menutup kesempatan untuk mendapatkan nilai profit yang lebih tinggi. Maka sebaiknya perusahaan juga mulai berusaha untuk mendapatkan customer baru sambil tetap mempertahankan customer lama.
6. Discount yang besar juga sebaiknya diberikan kepada customer yang loyal saja dengan syarat melakukan jumlah pembelian banyak dan pengulangan pembelian terbanyak juga. Perusahaan dapat memberikan diskon kepada Anthem, Food Motor, Allianz, Bank of America Corps., Valero Energy, Siemens, Tyson Foods dan BNP Paribas
