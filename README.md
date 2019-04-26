**MiniRHex: Açık Erişimli Altı Ayaklı Robot**

![MiniRHex Yürüyüş](Images/miniOnStumpScaled.jpg)
İletişim: nflowers@andrew.cmu.edu

MiniRHex, RHex'in tasarımına dayanan Robomechanics Lab tarafından tasarlanan minyatür ölçekli bir hexapod'dur. Dikkate değer özellikler arasında lazer kesim çerçevesi ve düşük maliyetli yapı için 3 boyutlu baskı ayakları ve robotun davranışı üzerinde yüksek düzeyde özelleştirilebilir kontrol sağlayan sezgisel bir yazılım paketi bulunuyor. MiniRHex, öğrencilerin tamamen işlevsel bir yürüyüş robotuyla çok daha düşük bir maliyetle deneme yapmalarını sağlayan bir eğitim ve tanıtım aracı olarak tasarlanmıştır. Düşük fiyat etiketi, araştırma gruplarının bir makine filosuna sahip olmalarını sağlayarak her öğrencinin donanım ile daha fazla etkileşime girmesini sağlar. Muhtemel eğitim ilkeleri arasında yürüyüş tasarımı ve optimizasyonu, bacak tasarımı ve kontrolü ve mobil robot sensörü kullanımı bulunur.

![Yük Gösterisi](Images/Brick_carrying.png)

# Kurum talimatları

Bir MiniRhex inşa etmek bir 3D yazıcıya ve lazer kesiciye erişim gerektirir. Raf dışı parçalar için bağlantılar aşağıda bulunabilir.

![MiniRHex Prototip](Images/mini1.jpg)

### Parçalar edinin

Sipariş listesine ve sipariş bağlantılarına buradan ulaşabilirsiniz. [Parça Listesi](https://github.com/robomechanics/MiniRHex/tree/master/HardwareList).

### Robotu birleştirin

Montaj talimatları mevcuttur. [Montaj Talimatları](https://github.com/robomechanics/MiniRHex/tree/master/Assembly).

![Ayak Montaj - Yakından](Images/1.jpg)

### Yazılımı yükleyin
1. OpenCM IDE' yi buradan indirebilirsiniz.  [http://www.robotis.us/opencmide/](http://www.robotis.us/opencmide/)
2. Adresindeki birincil depoyu klonlayınız. [https://github.com/robomechanics/MiniRHex.git](https://github.com/robomechanics/MiniRHex.git)

### Servo ID' lerini yapılandırın
1. OpenCM IDE'de, Dosya> Örnekler> Dynamixel Easy> b_setID öğesine gidin.
2. NEW_ID değişkenini aşağıdaki şemaya göre ID numarasına değiştirin.
3. Sadece ilgili servoyu karta bağlayın. (diğer servoların bağlantısını kesin)
4. Kodu yükleyin.
5. Her servo için tekrarlayın.

Yapılandırma başarılı olursa, yapılandırmakta olduğunuz servo ileri geri hareket etmelidir.

### Ayakların sıfırlarını ayarlayın
1. Klon desteği deposu bu adrestedir. [https://github.com/nikolaif399/zero_finder.git](https://github.com/nikolaif399/zero_finder.git)
2. Her bacağını olabildiğince düz aşağıya yakın olacak şekilde elle döndürün.
3. Zero_finder.ino dosyasını OpenCM'ye indirin.
4. IDE'deki Araçlar> Seri Monitör'e giderek seri monitörü açın ve sıfırları (yazdırma) leg_info.cpp içindeki sıfır dizisine kopyalayın.

![MiniRHex CAD](Images/RHex_Mini_IDS.JPG)

# Kullanma talimatları
1. MiniRHex'i bilgisayarınıza Micro USB portu üzerinden bağlayın.
2. OpenCM IDE'de MiniRHex.ino dosyasını açın ve "Araçlar" altında kontrol edin:
   - "Board" ROBOTIS OpenCM9.04 olarak ayarlayın.
   - "Port" doğru COM portuna ayarlayın. (MiniRHex takılıyken hangi COM portu eklenmişse)
3. Leg_info.cpp içindeki motor sıfırlarının doğru olduğundan emin olunuz.
4. İstenilen yürüyüş parametrelerini gait_parameters.cpp olarak ayarlayın.
5. OpenCM IDE'nin sol üst köşesindeki indirme simgesine tıklayın. ("İndirme Tamamlandı" yazana kadar bekleyin)
6. Mikro USB kablosunu çıkarın ve pili takın.
7. OpenCM kartındaki güç anahtarını çevirin.
8. "RESET" düğmesine basın, tüm motor LED'lerinin yeşil olduğundan emin olun.
9. Kodu çalıştırmak için "USER SW" tuşuna basın!
10. Ayakta durma davranışına geri dönmek için tekrar "RESET" düğmesine basın.

# Robot özellikleri
![MiniRHex Özellikleri](Images/Spec_Chart.png)

# Kullanışlı bağlantılar
### Parça listesi
Parça listesine buradan ulaşabilirsiniz. [Parça Lstesi](https://github.com/robomechanics/MiniRHex/tree/master/HardwareList).
### MiniRHex deposu
MiniRHex deposuna bu adresten ulaşılabilir. [MiniRHex Deposu](https://github.com/robomechanics/MiniRHex.git).
### Alıntı MiniRHex
Bir makalede MiniRHex'e gönderme yapıyorsanız lütfen alıntı yapın. [Özet](http://www.andrew.cmu.edu/user/amj1/papers/RSS2018ws_MiniRHex.pdf).
Alıntı için bunu kullanın. [BibTeX](https://github.com/robomechanics/MiniRHex/blob/master/citation.txt):
> M. Barragan, N. Flowers, and A. M. Johnson. "MiniRHex: A Small, Open-source, Fully Programmable Walking Hexapod". In *Robotics: Science and Systems Workshop on ``Design and Control of Small Legged Robots''*, Pittsburgh, PA, June 2018. 
 
### Resimler
Daha fazla MiniRHex resmi için. [Resim Galerisi](https://robomechanics.github.io/MiniRHex/Images/)

![MiniRHex Yürüyüş](Images/miniOnRock.bmp)
### Videolar

Robomechanics Lab'a  göz atın. [YouTube sayfası](https://www.youtube.com/watch?v=ldLXVDNCCzc&list=PLxHmBiQi0bD2aFgPKIrXhYXCCOGhTQmmk)

# Katkıda bulunanlar
MiniRHex aşağıdaki kişiler tarafından tasarlanmıştır. [Robomechanics Lab](https://www.cmu.edu/me/robomechanicslab/)
* Nikolai Flowers (BS ME '20)
* Barrett Werner (MS ME '19)
* Monica Barragan (BS ME '19)
* Cameron Selby (MS ME '18)
* Scott Phillips (BS ME '20)
* John Payne (Ph.D ME)
* Joe Norby (Ph.D ME)
* Aaron Johnson (Advisor)





