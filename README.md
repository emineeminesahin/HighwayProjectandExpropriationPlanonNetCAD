PROJE YAPIM AŞAMALARI

Yol projesi tasarıma başlamadan önce, bölgeye ait altlık haritalar indirildi. Föyde yol projesinde istenen tüm özellikler okundu ve incelendi. 1/2000 ölçeği ve projeksiyon ayarlandı. Her biri[çalışma bölgesine ait 3 boyutlu arazi verisi, havza verileri, bölgenin iklim koşullları, yağış verileri,imar-kadastral durum haritaları, bitki örtüsü haritası, mevcut ulaşım ağı] için her öğrenciye farklı verilen dönüşüm parametreleri kullanılarak dönüşüm yapıldı.[hesap-dönüşümler-helmert dönüşüm matrisinden objeleri dönüştür- ekran][tasarım projesi öğrenci veri listesindeki dönüşüm matris elemanları; a:1.0000020 b:0.0000000 cy:1.7827500 cx:1.4771700] 
Her veri bir projede toplandı.
Arazi verisi(3D_Arazi_Verisi.ncn) üzerinde Başlangıç_Bitis_Noktalari dosyası da alınarak üçgenleme (netsurf-üçgen oluştur )yapıldı. Oluşan üçgen modelden eğri geçirildi. Bozuk üçgenler silindi. 1, 2, 5, 10 m ve ara eğriler oluşturuldu, kota göre renklendirildi ve üzerlerine kotları yazdırıldı. Sonra bu şekilde sıkıntı çıktığı için önce arazi verisi üzerinde üçgen oluşturuldu ve eğri geçirildi. Daha sonra başlangıç ve bitiş noktaları projeye eklendi. Kotların küsüratlı çıkmaması için Başlangıç ve bitiiş noktaları en yakın eğrinin üzerine taşındı. Başlangıç noktası 398 kotlu eğriye, bitiş noktası  444 kotlu eğriye taşındı. İki nokta bir doğru ile birleştirilip gidilecek yön, başlangıç-bitiş noktasının kotları arasındaki farkı ve Sab=L mesafesi belirlendi. Sıfır poligonu hesabı yapıldı ve pergel açıklıkları bulundu.

L=98,52

L/2=49,26

L/4=27,63

Sıfır poligonu, eğrileri kesmiyecek bir şekilde geçirildi ve kesme durumlarında L/2+L/2, L/2+L/4+L/4, L/4+L/4+L/4+L/4 kombinasyonları yapıldı. Kesme durumlarına göre L uzunluğu 2m L/2 uzunluğu 1m L/4 uzunluğu 0.5m eğrilerinde kullanıldı.
Sıfır poligonu geçirildikten sonra ona yakın olacak şekilde ve kuru ve sulu dere gibi verilerin konumu dikkate alınarak güzergah çizildi. En az 3 yatay kurp istendiği için bu koşula uyuldu  ve 3 tane some noktası atıldı. Köşeleri yuvarlatıldı 450 m çaplı daireye göre, güzergah editöründen güzergah oluşturuldu. Varsayılan yarıçap 450 ve min r için proje hızı 90 seçildi. Otomatik dever uygulandı.Kurp asal elemanları(R,D,t,b,Δ ) hesaplandı. Geçki boyunca her kurp için dever değeri ve rakortman boyu hesaplandı Maksimum dever %8 , aliymandaki çatı eğimi -%2, şerit genişliği 3,5, şerit sayısı 4, tasarım aracı ve kaplama genişliği de seçildi.  ve spiral uygulaması seçildi. R ler 450 olarak değiştirildi ve güzergah tanımlandı.
Birinci kurbun spiral bilgilerininin giriş çıkış spiraldeki L boyları 88,89 girilerek klotoid uygulandı.
Daha sonra araçlar-krokiler bölümünden yatay kurp çakışma kontrolü, dever kontrolü, minimum aliyman uzunluk kontrolü, minimum kurp uzunluk kontrolü, yatay ve düşey elemanlar çakışma kontrolüne bakılarak hata olup olamadığına bakıldı.
Bunlar yapıldıktan sonra en kesit değerlerinin projede gösterilmesi için öncelikle güzergah, enkesit ve editor dosyaları netcad komutuyla oluşturuldu. Bizden istendiği şekilde en kesit değerleri geçki eksenine dik doğrultuda eksenin sol tarafına enkesit numaraları, sağ tarafına cm mertebesinde olmak üzere, kilometreler yani başlangıca olan uzaklıklar yazıldı. Enkesitler, başlangıç (A) ve bitiş (B) noktalarında, yatay kurbun, başlangıç (TO), bitiş (TF) ve bisektris (B) noktalarında, geçiş eğrisinin başlangıç (ÜA) ve bitiş (ÜE) noktalarında, geçki ekseninin yükseklik eğrilerini kestiği her noktada 25 m aralıklarla çizildi.Çiziminden sonra güzergahta gösterilen özel noktaların km değerleri ile hesaplanan km değerlerinin doğruluğu karşılaştırıldı.
Boy kesit işlemi için öncelikle boy kesit tablosu netcad komutuyla oluşturuldu.Tablo üzerinde yatay geçki boyunca oluşturduğumuz her en kesitin eksendeki arazi kotu okunarak boy kesitte de siyah kot olarak işaretlenerek ve bu siyah kotlar birleştirilerek siyah çizgi elde edilmiş oldu. Some noktalarinin koordınatı değiştirmeyecek şekilde yukarı aşağı sadece kotu değiştirerek kazı-dolgu ayarları yapıldı. en önemlisi olan kazı olabildiğince az tutulmaya çalışıldı. Tablo üzerinden başlangıç ve bitiş noktasını da kesecek şekilde kırmızı kot çizildi. En az üç farklı eğim gerektiği için üç tane düşey kurp oluşturuldu. İki eğim arasındaki farkın (gi-gi+1≥ 0,5) olmasına dikkat edildi. Eğim farkına göre tepe düşey kurp ya da açık düşey kurplar tespit edildi ve ona göre hesaplar yapıldı. Tepe düşey kurp için S değeri L ile bulundu. S‹L ve S›L'ye göre L değeri bulundu. Açık düşey kurp için konform kriteri, estetik kriteri, drenaj kriteri için L değeri ayrı ayrı hesaplandı ve drenaj kriteri dikkate alınarak L değeri bulundu. Açık ve tepe kurplar için bulunan L değerleri netcad'de düşey tanım editörü komutuyla girildi. Kapalı düşey kurplar için de emniyetli geçiş için görüş mesafeleri hesaplandı. Bu hesaplanan değerlerden sonra karar verilen kurp boyları düşey tanım editöründe kurplara girildi. Kurp çakışması kontrol edildi. Föyde belirtildiği şekilde boy kesit tablosunun alt kısmında eksik olan kilometraj değerleri, yatay kroki, düşey kroki ve dever krokisi oluşturuldu ve profile satır ekle komundan seçilerek kırmızı kot ile beraber tabloya eklendi. 〖(T_1)〗_km ve〖(T_1)〗_kot hesaplanan değerleri ile tabloda yazan değerlerin aynı olup olmadığı kotrol edildi.
Doğal arazi ile yarma ve dolgu şevlerinin yol ekseninden itibaren 15 metrede kesişmemesi halinde istinat ve iksa duvarları uygulandı ve çizildi. Kaplama kalınlığı; 8 cm, temel kalınlığı; 12 cm, alttemel kalınlığı; 30 cm alınarak 1/100 ölçeğinde tip enkesit oluşturuldu. Enkesit oluşturulurken de kaplama, temel ve alt temel tabakaları kapatıldı.
En kesitler çizdirilmeden önce tip kesit tanımları yapıldı ve şevli kotlu plan oluşturuldu. 
Enkesitler çizildikten sonra alanlar Cross yöntemine göre hesaplandı ve sağ üst köşelerine enkesit çizimi enkesit tablolarından dolgu ve yarma alanları yazıldırıldı.
Hacim hesapları NetCAD üzerimden yapıldı. Hesaplar tabloda gösterildi, Excel e kaydedildi.
Kesin yatay hat ekseni boyunca, eksenden itibaren sağa 20 m ve sola 20 m olmak üzere toplam 40 m’ lik bir koridor genişliği kamulaştırma genişliği olarak alındı.Kamulaştırma sınırına giren her bir parsel için m^2 biriminde kamulaştırma ve parsel alanları hesaplandı.Projenin maliyet hesapları yapıldı.

HACİM HESAPLARI

TOPLAM KAZI ALANI-TOPLAM DOLGU ALANI		=	2421.251	 m^2 kazı artar.

TOPLAM KAZI HACMİ-TOPLAM DOLGU HACMİ		=	63312.76967	m^3  kazı artar.

![image](https://user-images.githubusercontent.com/114474881/223502969-23fcd811-e613-452b-a4c1-03feedb1ba3e.png)
![image](https://user-images.githubusercontent.com/114474881/223503086-c112b872-8dfe-4142-b6c2-5ce642904e38.png)
![image](https://user-images.githubusercontent.com/114474881/223503135-cca59034-223c-4a2c-a38d-b968c3bbe16c.png)
![image](https://user-images.githubusercontent.com/114474881/223503191-27a8733b-4092-4a3b-afa5-307cc801d3ff.png)
![image](https://user-images.githubusercontent.com/114474881/223503224-d6cf6771-1fe8-4bf7-8360-a6cb25c8d9f6.png)
![image](https://user-images.githubusercontent.com/114474881/223503352-e2e3297d-6043-439c-a2ac-8010a05c4a6e.png)
ŞEVLİ KOTLU PLAN
![image](https://user-images.githubusercontent.com/114474881/223503583-d865b292-81d1-4bfd-95e7-660dfcaa74fe.png)
KAMULAŞTIRMA PLANI
![image](https://user-images.githubusercontent.com/114474881/223503762-3ae526be-3570-4e36-9bf3-c05977f68de9.png)
BOYKESİT
![image](https://user-images.githubusercontent.com/114474881/223503965-2b11c9de-5a8c-4c62-befa-94e7ca6b109e.png)
KARIŞIK ENKESİT
![image](https://user-images.githubusercontent.com/114474881/223504229-76093aa0-379d-4eb4-8082-26cd34bc458f.png)





