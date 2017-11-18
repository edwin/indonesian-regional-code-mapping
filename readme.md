Indonesian Regional Code Mapping, Between Kemendagri - BPS and Kemenkeu 
===================

Explanations
-------------------
(EN)
Indonesia is a unique country, basically it have 3 set of data for regional coding. Code according to Kemendagri (Ministry of Home Affairs), BPS (Indonesian Statistics Agency) and Kemenkeu (Ministry of Finance). This Github project contains MySQL data dump for mapping those 3 codes accordingly.

(ID)
Indonesia adalah negara yang unik, karena memiliki (paling tidak) tiga set pengkodean wilayah, yaitu kode menurut Kemendagri, BPS dan Kemenkeu. Oleh karena itu, dibutuhkan suatu table yang bisa melakukan mapping antara kode di 3 kementrian tersebut. Dump table tersebut tersedia di Project Github ini.

Tools
-------------------
* DB - MySql

Query
--------------------
``` sql
select kode_kemendagri, kode_kemenkeu, kode_bps, nama_wilayah from t_kewilayahan
where nama_wilayah like '%Bolaang%'
```

Disclaimer
-------------------
* Data is taken around 2016, and only until regency level only. Open Issue or do PR if there's any data is wrong or have any updates.
* This application is provided AS-IS and i have no responsibility for any external damage caused indirectly or directly. 