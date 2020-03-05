EN AZ SAYIDA BOZUK PARA VERME PROBLEMI

Þeyma Nur MUTLU		-	170201004
Melike OÐUZ		-	170201028

Bu readme.txt dosyasý, En Az Sayýda Bozuk Para Problemi projesine aittir.
Bu paket, kaynak kodu ile ayný dizin içerisinde bulunacaktýr.

1-PAKETÝN ÝÇERÝÐÝ:
----------
170201004-170201028.txt - Projenin tek dosyaya indirgenmiþ salt kaynak kodu.
readme.txt - Bu dosya.
170201004-170201028.zip - Projenin kaynak kodunun ve yardýmcý dosyalarýn ziplenmiþ hali.
rapor.pdf - Proje raporu.
----------

2-SÝSTEM GEREKSÝNÝMLERÝ:
-------------------
Oracle VM virtualbox - https://www.virtualbox.org/
Sanal Makine Ýmajý   - https://github.com/KOU-Embedded-System-Lab/os-base-image/releases
-------------------

3-PROJEYÝ ÇALIÞTIRMAK:
-------------------
Paket içeriðini yukarýda görebilirsiniz.

Bu kod, önceden tanýmlanmýþ sanal makinede çalýþtýrýldý.

Sanal makineyi indirmek için;
https://github.com/KOU-Embedded-System-Lab/os-base-image/releases
adresini ziyaret edebilirsiniz.

Kod, herhangi bir hata vermeksizin, daha önceden
belirlenen kriterlere uygun çalýþtý.
-------------------

4-KODU DERLEMEK:
------------------
Artýk bilgisayarýmýzda kurulu olan sanal makine ile kodu kolayca derleyebiliriz.

Projeyi geliþtirim kartýnda çalýþtýrmak için kodu daha önceden oluþturulmuþ Tiva C
projesinde yer alan "main.c"ye yapýþtýrýp build butonuna týkladýktan sonra debug 
butonuna týklamanýz yeterli.

Eðer kart, sanal makine tarafýndan bulunamadýysa (OpenOCD hatasý) sanal makineye
baðlý olan bir kart olmayabilir. Sað alt kýsýmdan usb ikonuna sað týklayarak 
Texas Instruments'ý seçip sanal makineye baðlamanýz gerekmektedir.

Ana Makinesi GNU/Linux olan makinelerde VirtualBox, kullanýcý izinlerine sahip
olmayabiliyor. Eðer takýlý olan USB aygýtlarý tanýmýyorsa, 
'sudo usermod -G vboxusers -a $USER'
kodunu çalýþtýrmanýz ve sisteminizi yeniden baþlatmanýz gerekmektedir. 
------------------

5- PARAMETRELER
---------------------------
Kodun çalýþmasý için baþlangýçta herhangi bir parametre gerekmiyor.
---------------------------

6- PROGRAMIN KULLANIMI
-----------------------------
En Az Sayýda Bozuk Para Problemi projesi, program içersindeki katardan ürün ile ilgili olan ID bilgisi, ad bilgisi, stok sayýsý ve fiyat bilgisi alýnacaktýr.
Daha sonra butonlar yardýmý ile yirmi beþ kuruþ, elli kuruþ, bir tl olarak para miktarý girdisi alýnýr, bitiþ butonuna basýlýnca para girme iþlemi bitirilir.
Para girme iþleminden sonra ürün seçim iþlemi yapýlacaktýr butonlara go¨re hangi u¨ru¨nu¨n sec¸ilecegˆi belirlenecektir. 
Kullanýcý yanlýþ seçim yaptýðýnda Reset butonuna basabilir. Aksi taktirde otomat, kasada bulunan bozuk paralardan en azýný kullanarak kullanýcýya bozuk para 
verecektir.Kasada yeterli para olmamasý durumunda LCD ekranda "Kasada yeterli para yoktur" uyarýsý görünecektir.