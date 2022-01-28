# Azure Iot Hub Nedir ?
Internet veya diğer iletişim ağı üzerinden diğer cihazlara ve hizmetlere sağlanan ve veri 
alışverişi yapılan fiziksel cihazlar ağı olarak tanımlanır. IoT Hub, IoT cihazlarından buluta 
depolama veya işleme amacıyla yüksek hacimlerde telemetri almanızı sağlayan bir Azure 
hizmetidir.
IoT hub, bir IoT ugulaması ile bağlı cihazlar arasında iletişim için central message hub görevi 
görür.
• Cihazdan buluta telemetri
• Cihazlardan dosya yükleme
• Cihazları buluttan kontrol etmek için istek-cevap yöntemlerini
destekler.
***Örneğin ⇒ *** Bir kimyasal tesiste reaktörleri takibe alan ve sıcaklık belirli bir değeri aştığında uyarı gönderen bir cihaz.

![iothub](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/b8c5ee53-3b02-44f5-b89c-c8c6cff374c3/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220128%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220128T124657Z&X-Amz-Expires=86400&X-Amz-Signature=85883ae375d569565b31d9346974a0042ef0886cab5090c1f0f99edd6c6146e5&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

## Cihaz Telemetrisi
Cihazdan alınan telemetri örnekleri arasında, hız veya sıcaklık gibi algılayıcı verileri, 
atlanmış olay, bir hata iletisi cihaz durumu belirten bilgi iletisi yer alır. IoT cihazları içgörü 
elde etmek için uygulamaya olaylar gönderir.
IoT Hub verileri birden çok aboneye iletmenizi sağlayan Event Grid ile tümleşir. Event Grid, 
birçok farklı Azure hizmeti ve uygulamasında olayları kolayca yönetmemizi sağlar.
Iot Hub, IoT uygulamanız ve cihazları arasında çift yönlü iletişim için merkezi mesajlaşma 
Hub'ı olarak çalışır.

**Telemetry:** Telemetri, bir IoT cihazı tarafından alınan değerleri kaydetme ve iletme 
işlemidir. Telemetri, bir IoT çözümünün temel bir işlevidir.
**Routing:** Mesaj yönlendirme, cihazlarınızdan bulut hizmetlerine otomatik, ölçeklenebilir ve 
güvenilir bir şekilde mesaj göndermenizi sağlar. Cihaz telemetri mesajlarını veya olaylarını 
(örneğin cihaz yaşam döngüsü olayları) gönderebilirsiniz.
**Integrate with other services:** Uçtan uca bir çözüm oluşturmak için IoT Hub'ı diğer Azure 
hizmetleriyle sorunsuz bir şekilde tümleştirebilirsiniz. Örneğin, iş süreçlerini 
otomatikleştirmek için IoT Hub'ı Azure Logic Apps ve Event Grid ile birleştirebilirsiniz.
**Device Identity Registry:** IoT Hub bir Identity Registry tutar. Identity Registry defteri, IoT 
Hub'a bağlanmasına izin verilen cihazlar ve modüller hakkındaki bilgileri depolar. Varlığın 
IoT Hub'a bağlanabilmesi için cihaz veya modül için bir kimlik kayıt defteri girişi 
bulunmalıdır. Bir cihaz veya modül, kimlik kayıt defterinde depolanan kimlik bilgilerine 
dayalı olarak IoT Hub ile kimlik doğrulaması da yapmalıdır.
**Device twins:** Device Twins, meta veriler, yapılandırmalar ve koşullar dahil olmak üzere 
cihaz durumu bilgilerini depolayan JSON belgeleridir. Azure IoT Hub, IoT Hub'a 
bağladığınız her cihaz için bir Device Twins tutar. Device Twins, Cihaz ve arka uçların cihaz 
koşullarını ve yapılandırmasını senkronize etmek için kullanabileceği cihazla ilgili bilgileri 
depolar.

```
Basic tier cihazlardan veri toplamak ve analiz etmek için seçilmelidir. Tek yönlü iletişim 
sağlar.
Standard tier ise tüm IoT hub özelliklerini aktif eder ve çift yönlü iletişim sağlar.
```