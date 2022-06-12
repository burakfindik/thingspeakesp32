# HAVA KALİTESİ ÖLÇÜMÜ VE NESNELERİN İNTERNETİ UYGULAMASI
##ESP32s kullanarak ThingSpeak.com'a veri gönderme ve alarm oluşturma


<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_3.png" width="800" height="500">  
  
  

Ek Devre Kartları URL'leri kısmına https://dl.espressif.com/dl/package_esp32_index.json linkini kopyalarak tamam diyoruz.
    
<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_4.png" width="400" height="250"> 
  
Kart Yöneticisi kısmından ESP32 yazarak esp32 by espressif systems versiyon 1.0.6'yı IDE'mize kuruyoruz.
  
<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_5.png" width="600" height="350"> 
 
Böylelikle Arduino IDE'mize tanımlı olan Nodemcu-32s kartını seçebiliriz.
  
<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_6.png" width="600" height="350">   
  


ESP32s'i USB portuna bağladıktan sonra [ESP32s Kodu ile](https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/ESP32s) Arduino IDE'den ESP32'yi programlıyoruz.
 

 
**ThingSpeak.com üzerinde gerekli ayarların yapılması**
 <p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_8.png" width="1000" height="750">
  
 Yukarıdaki resimde gösterildiği gibi proje ismini, açıklamasını yazıp ve kanal aktivasyonlarını yaptıktan sonra konfigirasyonu kaydediyoruz.
 Böylelikle gerekli parametleri kodların içine yazarak ThingSpeak.com'a veri göndermeye başlayabiliriz.
  
 <p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_9.png" width="1000" height="750">
  
Veriler Thingspeak.com üzeriinde MATLAB / Mathwork altyapısını kullarak grafiksel olarak gösteriliyor.
  
Son olarak veriler eğer ayarladığımız aralığın dışına çıkarsa **REACT** oluşturarak mail ile bilgilendirilmeyi sağlıyoruz.
  
  
<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_10.png" width="400" height="600">
 
Parametleri belirledikten sonra **save** butonuna tıklıyoruz.[Matlab Kodu ile](https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/matlab_analysis)
Matlab Analysis kısmını programlıyoruz.
<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_11.png" width="600" height="500">

 **Save and Run** butonuna bastığımızda veriler belirttiğimiz aralığın dışına çıkarsa Thingspeak.com'a kaydolduğumuz e-posta hesabına bilgilendirme maili gönderelicektir.

<p align=center>
<img src= "https://github.com/burakfindik/raspberrythingspeakesp32/blob/main/Images/Screenshot_12.png" width="1200" height="500">
 
Thingspeak.com her 30 dakika içerisinde mail ile yalnızca 2 defa bilgilendirme sağlamaktadır.
 
