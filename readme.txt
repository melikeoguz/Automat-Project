EN AZ SAYIDA BOZUK PARA VERME PROBLEMI

�eyma Nur MUTLU		-	170201004
Melike O�UZ		-	170201028

Bu readme.txt dosyas�, En Az Say�da Bozuk Para Problemi projesine aittir.
Bu paket, kaynak kodu ile ayn� dizin i�erisinde bulunacakt�r.

1-PAKET�N ��ER���:
----------
170201004-170201028.txt - Projenin tek dosyaya indirgenmi� salt kaynak kodu.
readme.txt - Bu dosya.
170201004-170201028.zip - Projenin kaynak kodunun ve yard�mc� dosyalar�n ziplenmi� hali.
rapor.pdf - Proje raporu.
----------

2-S�STEM GEREKS�N�MLER�:
-------------------
Oracle VM virtualbox - https://www.virtualbox.org/
Sanal Makine �maj�   - https://github.com/KOU-Embedded-System-Lab/os-base-image/releases
-------------------

3-PROJEY� �ALI�TIRMAK:
-------------------
Paket i�eri�ini yukar�da g�rebilirsiniz.

Bu kod, �nceden tan�mlanm�� sanal makinede �al��t�r�ld�.

Sanal makineyi indirmek i�in;
https://github.com/KOU-Embedded-System-Lab/os-base-image/releases
adresini ziyaret edebilirsiniz.

Kod, herhangi bir hata vermeksizin, daha �nceden
belirlenen kriterlere uygun �al��t�.
-------------------

4-KODU DERLEMEK:
------------------
Art�k bilgisayar�m�zda kurulu olan sanal makine ile kodu kolayca derleyebiliriz.

Projeyi geli�tirim kart�nda �al��t�rmak i�in kodu daha �nceden olu�turulmu� Tiva C
projesinde yer alan "main.c"ye yap��t�r�p build butonuna t�klad�ktan sonra debug 
butonuna t�klaman�z yeterli.

E�er kart, sanal makine taraf�ndan bulunamad�ysa (OpenOCD hatas�) sanal makineye
ba�l� olan bir kart olmayabilir. Sa� alt k�s�mdan usb ikonuna sa� t�klayarak 
Texas Instruments'� se�ip sanal makineye ba�laman�z gerekmektedir.

Ana Makinesi GNU/Linux olan makinelerde VirtualBox, kullan�c� izinlerine sahip
olmayabiliyor. E�er tak�l� olan USB ayg�tlar� tan�m�yorsa, 
'sudo usermod -G vboxusers -a $USER'
kodunu �al��t�rman�z ve sisteminizi yeniden ba�latman�z gerekmektedir. 
------------------

5- PARAMETRELER
---------------------------
Kodun �al��mas� i�in ba�lang��ta herhangi bir parametre gerekmiyor.
---------------------------

6- PROGRAMIN KULLANIMI
-----------------------------
En Az Say�da Bozuk Para Problemi projesi, program i�ersindeki katardan �r�n ile ilgili olan ID bilgisi, ad bilgisi, stok say�s� ve fiyat bilgisi al�nacakt�r.
Daha sonra butonlar yard�m� ile yirmi be��kuru�, elli kuru�, bir tl olarak para miktar� girdisi al�n�r, biti� butonuna bas�l�nca para girme i�lemi bitirilir.
Para girme i�leminden sonra �r�n se�im i�lemi yap�lacakt�r butonlara go�re hangi u�ru�nu�n sec�ileceg�i belirlenecektir. 
Kullan�c� yanl���se�im yapt���nda Reset butonuna basabilir. Aksi taktirde otomat, kasada bulunan bozuk paralardan en az�n� kullanarak kullan�c�ya bozuk para 
verecektir.Kasada yeterli para olmamas� durumunda LCD ekranda "Kasada yeterli para yoktur" uyar�s� g�r�necektir.