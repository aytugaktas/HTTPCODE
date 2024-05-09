# HTTP STATUS CODE DOKÜMANTASYONU
![image](https://github.com/aytugaktas/HTTPCODE/assets/160540290/56f189ed-b932-4ed6-9bda-94e0d2eea4ef)

## HTTP Durum Kodları (Status Codes) Nedir?

Kullanıcılar bir web sitesini ziyaret etmek istediklerinde iki taraflı bir iletişim ortaya çıkar. Bu iletişimin bir tarafında tarayıcı bulunurken diğer tarafta sunucu yer alır. Bu iletişim kullanıcının bir web sayfasına giriş yapmak istemesiyle başlar. Bir web sayfasına giriş yapan kullanıcı aslında tarayıcı aracılığıyla ilgili web sayfasının yer aldığı sunucuya sayfayı görüntülemek için bir istek gönderir. Sunucu ise bu isteğe üç haneli bir durum kodu ile yanıt verir. Sunucunun tarayıcıya verdiği üç haneli cevaplar HTTP durum kodları ya da HTTP status code olarak adlandırılır. İlgili durum kodları bazen bir hata olduğunu bildirirken bazen de sayfanın herhangi bir sorun olmadan açıldığını ifade edebilir. Bu nedenle HTTP durum kodlarının daima hata olarak değerlendirilmesi doğru değildir.

## HTTP Durum Kodları Neden Önemlidir?

HTTP durum kodları hem web siteleri hem de kullanıcılar için önemli bir rol oynay. Web sitenizin sorunsuz açılması, yanıt verme süresi ve durum kodları kullanıcı deneyimini doğrudan etkiler. Her web sitesinin ortak kaygısı da kullanıcı deneyimini pozitif yönde tutmaktır. Eğer siteniz sorunsuz şekilde açılıyor, hızlı bir şekilde yanıt veriyor ve başarılı durum kodu dönüyorsa kullanıcılar sitenizde daha iyi bir deneyim yaşarlar. Ancak siteniz komutlara geç cevap veriyor ve sürekli şekilde hata kodu döndürüyorsa bu sitenizin güvenilirliğini ve kullanıcı memnuniyetini olmusuz etkileyecektir. Bu durum kullanıcı deneyimini etkilerken sitenizin **SEO** (Arama Motoru Optimizasyonu) performansını da etkileyecektir. Arama motoru botları; web sitelerini tarayıp dizine eklerken, sitenizin yanıt verme süresini ve HTTP durum kodlarını dikkate alır. Örneğin sürekli olarak 5xx (sunucu hatası) durum kodlarıyla karşılaşan bir web sitesi, arama motoru botlarının güvenini kaybedebilir ve arama motoru sonuç sayfası sıralamasında düşebilir. Bir başka örnekle, 404 (sayfa bulunamadı) hata koduna sahip sayfalar arama motoru botları tarafından olumsuz değerlendirilir ve indekslenemez. 

![alternatif metin](https://cdnblog.natrocdn.com/wp-content/uploads/2023/05/http-durum-kodlari-4-1024x683.jpg)

## HTTP Durum Kodu Sınıfları 

HTTP Durum Kodları beş ayrı sınıfa ayrılır ve her sınıf belirli bir olayı temsil eder. HTTP durum kodu üç haneli bir sayıdan oluşur. İlk rakam durum kodunun sınıfını belirtir ve genel olarak durum kategorisini temsil eder. Diğer iki rakam ise durumun ayrıntılarının belirtir.

![image](https://sitechecker.pro/wp-content/uploads/2023/09/100-status-code.png)

### **1XX - Bilgi: Bu sınıf, sunucunun isteği aldığını ve işlemeye devam ettiğini bildiren durumları temsil eder.**
  
  **100:** Bu durum kodu, sunucunun isteği hala işlemekte olduğunu vew tamamlanmasını beklediğini belirtir. Bu durumda, sunucu belirli bir süre boyunca işlemi sürdürebilir ve daha sonra sonuç döndürebilir.

  **101:** Bu durum kodu, tarayıcının sunucudan bir protokol değişikliği istediğini ve sunucunun da bu isteği kabul ettiğini ifade eder.

  **103:** Bu durum kodu, sunucunun son istek iletisinden önce bazı yanıt başlıklarını döndürdüğünü ifade eder. Özellikle uzun süren isteklerde veya çeşitli aşamalarla gerçekleşen işlemlerde kullanılır. Sunucu, önemli başlıkları önceden göndererek istemciye bilgi sağlamış olur.
  
![image](https://sitechecker.pro/wp-content/uploads/2023/09/200-status-code.png)

### **2XX - Başarılı: Bu sınıf, isteğin başarıyla tamamlandığını ve sunucunun istenilen kaynağı başarıyla döndürdüğünü gösterir.**
  
  **200:** İsteğin başarıyla işlendiği ve tarayıcı ile sunucu arasında her şeyin yolunda olduğu anlamına gelir. Bu durumda isteğin istenen kaynakla ilgili doğru sonuçlarla döndürüldüğü anlaşılır.

  **201:** Sunucu, isteğin başarılı bir şekilde yerine getirildiğini ve yeni bir kaynağın oluşturulduğunu belirtir.

  **202:** Sunucu, tarayıcının gönderdiği isteği kabul etti ve işleme koydu. Ancak, isteğin olumlu veya olumsuz sonuçlanabileceğini ifade eder. Yani, sonuç henüz tam olarak bilinmiyor olabilir.

  **203:** Bu durum, kaynağın sunucu tarafından başarıyla işlendiği, ancak yanıtın istemci tarafından değiştirildiği anlamına gelir. Örneğin, bir proxy sunucu tarafından içerik filtrelemesi yapılmış olabilir.

  **204:** Sunucunun isteği başarıyla işlediği, ancak herhangi bir içerik döndürmeyeceği anlamına gelir. Yani, istemciye herhangi bir yanıt verilmez. Bu durum genellikle güncelleme veya silme gibi işlemlerde kullanılır.

  **205:** 204 durum kodu gibi isteğin başarıyla işlendiği, ancak herhangi bir içerik döndürülmeyeceği anlamına gelir. Bununla birlikte, tarayıcının belge görünümünü sıfırlaması gerektiği anlaşılır. Yani, tarayıcı, kullanıcının gördüğü içeriği yenilemelidir.

  **206:** Bu durum kodu, tarayıcının durdurulmuş indirmelere devam etmesini ve indirmeleri birden fazla akışa ayırmasını sağlar. Özellikle büyük dosyaların parça parça indirilmesi gerektiğinde kullanılır.

![image](https://sitechecker.pro/wp-content/uploads/2023/09/300-status-code.png)

### **3XX - Yönlendirme: Bu sınıf, tarayıcının istenen kaynağı başka bir yerde bulabileceğini gösterir.**
  
  **300:** Bu durum kodu, sunucunun birden fazla olası kaynağa sahip olduğunu ve tarayıcının seçim yapması gerektiğini ifade eder. Sunucu, farklı kaynakları tarayıcıya sunar ve tarayıcı, hangi kaynağı kullanmak istediğini seçer
  
  **301:** Bu durum kodu, bir web sayfasının veya kaynağın kalıcı olarak farklı bir yere taşındığını belirtir. Tarayıcı, gelecekte bu kaynağı yeni konumunda bulabilir ve isteklerini doğrudan oraya yönlendirebilir.

  **302:** Bu durum kodu, bir web sayfasının veya kaynağın geçici olarak farklı bir yere taşındığını ifade eder. Tarayıcı, bu durumda isteği geçici konuma yönlendirir ve gelecekte tekrar eski konumunu kullanabilir.

  **303:** Bu durum kodu, tarayıcının Post, Put veya Delete yöntemleriyle talep ettiği kaynağın başka bir URL'de bulunduğunu belirtir. Tarayıcı, kaynağı almak için farklı bir URL'ye Get isteği yapmalıdır.

  **304:** Bu durum kodu, tarayıcıya önbelleğinde depolanan bir kaynağın değişmediğini bildirir. Tarayıcı, önbellekteki sürümü kullanarak kaynağı yeniden indirmek yerine yerel önbellekteki veriyi kullanır, bu da bant genişliğinden tasarruf sağlar.

  **307:** Bu durum kodu, bir kaynağın geçici olarak farklı bir yere taşındığını ifade eder. 302 durum kodundan farklı olarak, tarayıcının yönetiminin değişmesine izin vermez. Yani tarayıcı, isteği tekrar aynı yerine yönlendirir.

  **308:** Bu durum kodu, bir kaynağın kalıcı olarak farklı bir yere taşındığını belirtir. 301 durum kodundan farklı olarak, tarayıcının yönetiminin değişmesine izin vermez. Tarayıcı, gelecekteki istekleri doğrudan yeni konuma yönlendirir.

  ![image](https://sitechecker.pro/wp-content/uploads/2023/06/400-status-code.png)

### **4XX - İstemci Hatası: Bu sınıf, isteğin yanlış veya geçersiz olduğunu ve sunucunun isteği yerine getiremediğini gösterir.**
  
  **400:** Bu durum kodu, sunucunun tarayıcının gönderdiği isteği hatalı bulduğunu ve isteği işleyemediğini ifade eder. Genellikle kullanıcı tarafından yapılan yanlış bir istek veya geçersiz veri gönderimi nedeniyle ortaya çıkar.
  
  **401:** Bu durum kodu, kullanıcının erişmek istediği kaynağın güvenlik doğrulaması gerektirdiğini ve kullanıcının geçerli kimlik doğrulama bilgilerine sahip olmadığını belirtir. Kullanıcı, kimlik doğrulama yapmadan kaynağa erişemez.

  **402:** Bu durum kodu, kullanıcının bir kaynağa erişmek için ödeme yapması gerektiğini ve gelecekte kullanılmak üzere rezerve edildiğini ifade eder. Bu genellikle çevrimiçi ödeme gerektiren içeriklerde kullanılır.

  **403:** Bu durum kodu, kullanıcının ilgili kaynağa erişimin yasaklandığını belirtir. Kullanıcı, güvenlik veya izin sorunları nedeniyle kaynağa erişemez.

  **404:** Bu durum kodu, istenen kaynağın sunucuda bulunmadığını ifade eder. En sık karşılaşılan HTTP durum kodlarından biridir ve genellikle "Sayfa Bulunamadı" hatası olarak bilinir.

  **405:** Bu durum kodu, istenen kaynak için kullanılan istek yönteminin desteklenmediğini ifade eder. Örneğin, bir GET isteği yerine POST isteği gerektiren bir kaynağa GET isteği gönderildiğinde bu durum kodu döndürülür.

  **406:** Bu durum kodu, istemcinin Accept Header bölümünde belirtilen özelliklerin sunucu tarafından karşılanamadığını ifade eder. Sunucu, istemciye uygun bir içerik döndüremez.
  
  **407:** Bu durum kodu, bir proxy sunucu ile kimlik doğrulaması ve yetkilendirme gerektiren durumlarda kullanılır. Kullanıcı, geçerli kimlik bilgileriyle kimlik doğrulaması yapmadan kaynağa erişemez.
  
  **408:** Bu durum kodu, sunucunun isteği beklerken zaman aşımına uğradığını ifade eder. Genellikle ağ bağlantısı sorunları veya sunucu yoğunluğu nedeniyle ortaya çıkar.

  **409:**  Bu durum kodu, bir uyuşmazlık veya çakışma durumu olduğunu ve isteğin tamamlanamadığını belirtir. Örneğin, aynı kaynağa aynı anda birden fazla değişiklik isteği gönderildiğinde bu durum kodu döndürülür.

 ![image](https://sitechecker.pro/wp-content/uploads/2023/07/500-status-code.png)

### **5XX - Sunucu Hatası: Bu sınıf, sunucunun isteği yerine getiremediğini ve bir hata oluştuğunu gösterir.**
  
  **500:** Bu durum kodu, sunucudaki bir sorun nedeniyle isteğin tamamlanamadığını ifade eder. Sunucu tarafında bir hata veya başka bir sorun olduğunda bu durum kodu döndürülür.

  **501:** Bu durum kodu, sunucunun isteği yönetemediği veya desteklemediği anlamına gelir. Sunucu, isteği yerine getirmek için gerekli işlevleri desteklemiyor veya uygulamıyor olabilir.

  **502:** Bu durum kodu, sunucunun başka bir sunucuya istek gönderdikten sonra geçersiz bir yanıt aldığını ifade eder. Örneğin, bir proxy sunucusu başka bir sunucudan hatalı bir yanıt alırsa bu durum kodu döndürülür.

  **503:** Bu durum kodu, sunucunun geçici olarak hizmet veremediği ve istekleri işleyemediği durumlarda kullanılır. Genellikle sunucunun aşırı yük altında olduğu veya bakım çalışmalarının yapıldığı zamanlarda görülür.

  **504:** Bu durum kodu, bir isteği işlerken sunucunun beklediği yanıtı zamanında alamaması durumunda kullanılır. Sunucu, başka bir sunucudan beklenen yanıtı zaman aşımına uğradığında bu durum kodu döndürülür.

  **511:** Bu durum kodu, kullanılacak ağın isteği sunucuya iletmek için kimlik doğrulaması gerektirdiği durumlarda kullanılır. Örneğin, bir WiFi ağına bağlanmak için kullanıcı kimlik doğrulaması yapmak zorunda olduğunda bu durum kodu döndürülür.
  
![alternatif metin](https://www.sempeak.com/yuklemeler/blog-gorselleri/http-status-code.png)
  
## En Yaygın Kullanılan HTTP Durum Kodları

- **200 OK:** Bu kod, sunucunun istenen kaynağı başarıyla bulduğunu ve istenen içeriği sağladığını belirtir. Bu, arama motoru botunun sayfanın içeriğini indekslemeye başlayabileceği anlamına gelir.
  
- **301 Moved Permanently:** Bu kod, sunucunun istenen kaynağın URL’sinin değiştiğini ve kalıcı olarak başka bir yere taşındığını belirtir. Arama motoru botu, yeni URL’ye yönlendirilecek ve kaynağı yeniden indeksleyecektir.

- **302 Found:** Bu kod, sunucunun istenen kaynağın URL’sinin geçici olarak başka bir yere taşındığını belirtir. Arama motoru botu, yeni URL’ye yönlendirilecek ve kaynağı geçici olarak indeksleyecektir.

- **403 Forbidden:** Bu kod, sunucunun istenen kaynağa erişime izin vermediğini belirtir. Bu durumda, arama motoru botu kaynağı indeksleyemez.

- **404 Not Found:** Bu kod, sunucunun istenen kaynağı bulamadığını belirtir. Bu durumda, arama motoru botu kaynağı indeksleyemez.

- **500 Internal Server Error:** Bu kod, sunucunun istenen kaynağı gösteremediği bir iç hata nedeniyle oluştuğunu belirtir. Bu durumda, arama motoru botu kaynağı indeksleyemez.

- **503 Service Unavailable:** Bu kod, sunucunun geçici bir süre hizmet dışı olduğunu belirtir. Bu durumda, arama motoru botu kaynağı indeksleyemeyecektir.

## 200 Dışında Durum Kodu Çeviren URL'ler için Yapılması Gerekenler Nelerdir?

200 dışındaki statü kodları alan URL’ler, genellikle bir hata veya sorun olduğunu gösterir. Bu nedenle, bu durumda yapılması gerekenler şunlardır:

- **Hatanın nedenini belirleyin:** İlk olarak, URL'nin aldığı statü kodunun nedenini belirlemek gerekir. Bunun için, ilgili hatanın tanımını ve nedenini anlamak için HTTP statü kodları hakkında bilgi sahibi olmak önemlidir.

- **Hata kaynağını bulun:** Hata kaynağı genellikle web sitesinin kodunda veya sunucu konfigürasyonunda yer alır. Bu nedenle, hata kaynağını belirlemek için web sitesinin kodunu ve sunucu konfigürasyonunu kontrol etmek gerekir.

- **Sorunu çözün:** Hata kaynağı belirlendikten sonra, sorunu çözmek için gerekli adımlar atılmalıdır. Örneğin, bir hata web sitesinin kodundan kaynaklanıyorsa, kodu güncellemek veya değiştirmek gerekebilir. Eğer sorun sunucu konfigürasyonundan kaynaklanıyorsa, sunucu ayarlarını değiştirmek gerekebilir.

- **Test edin:** Sorunun çözümü tamamlandıktan sonra, web sitesini test etmek ve URL’nin artık doğru bir statü kodu aldığından emin olmak önemlidir.

- **Kullanıcıları bilgilendirin:** Eğer URL bir hata sayfasına yönlendiriyorsa, kullanıcıların bu hatayı neden aldığını anlamalarını sağlamak için bir hata mesajı veya yönlendirme sayfası oluşturulmalıdır.

- **SEO etkisini değerlendirin:** URL’lerin SEO değeri, aldığı statü kodu ile değişir. Bu nedenle, URL’lerin 200 dışındaki statü kodlarını çözmeden önce, SEO etkisini değerlendirmek önemlidir. Gerektiğinde, URL’leri yeniden yönlendirmek veya güncellemek gerekir.







        
