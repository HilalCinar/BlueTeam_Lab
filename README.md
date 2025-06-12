# BlueTeam_Lab

Bu proje, kurumsal sistemlerde karşılaşılabilecek siber tehditlere karşı etkili bir şekilde tespit ve yanıt mekanizmaları geliştirmek amacıyla oluşturulmuştur. Gerçek dünya saldırıları simüle edilerek log analizi, SIEM kullanımı, tehdit tespiti (Sigma/YARA), ve güvenlik operasyon süreçleri üzerine kapsamlı bir laboratuvar ortamı oluşturulmaktadır.

---

## Proje Kapsamı

### 1. MITRE ATT&CK Matrisine Göre Saldırı Senaryoları
- Atomic Red Team framework’ü kullanılarak 14 farklı MITRE ATT&CK Taktiği çerçevesinde toplam **100 adet saldırı senaryosu** uygulanacaktır.
- LOLBAS (Living Off The Land Binaries and Scripts) araçları da senaryolarda aktif olarak kullanılacaktır.
- Her saldırı senaryosunun amacı, adım adım işleyişi, sistem üzerindeki beklenen etkileri ve MITRE ATT&CK matrisindeki yeri detaylı olarak raporlanacaktır.

### 2. Anomali Tespiti ve Log Analizi
- Kurban makinede oluşan olay kayıtları (log kaynakları) incelenerek, saldırgan faaliyetlerinin izleri belirlenecektir.
- Blue Team perspektifinden yapılan gözlemler doğrultusunda, her saldırıya özel en etkili SPL sorguları geliştirilecek ve Splunk üzerinde test edilecektir.
- Hangi log kaynağında hangi Event ID değerlerinin görüldüğü, bu değerlerin ne anlama geldiği ve nasıl tespit edileceği sistematik olarak dokümantasyon altına alınacaktır.

### 3. Kurumsal Kullanıma Uygun Tespit Kuralları Geliştirme
- Her saldırı senaryosuna karşılık gelen kurumsal ortamlarda kullanılabilir bireysel saldırı tespit kural setleri yazılacaktır.
- Bu kurallar, Splunk SPL sorguları, Sigma rule'lar, ve YARA rule'lar şeklinde üç farklı formatta geliştirilecektir.
	- Sigma Rule: Log tabanlı tehditleri tanımlayan genel amaçlı tehdit tespit imzaları.
	- YARA Rule: Binary dosya ve payload temelli tehditleri tespit etmek için IOC (Indicator of Compromise) odaklı kurallar.

### 4. Splunk Dashboard ve Gerçek Zamanlı Alarm Sistemleri
- Saldırıların gerçek zamanlı olarak tespiti için Splunk dashboardları tasarlanacak.
- SPL sorguları alarm motoruna entegre edilerek gerçek zamanlı uyarı sistemleri kurulacak.
  
---

## Raporlama İçeriği

Her saldırı senaryosu için aşağıdaki bilgiler sistematik biçimde raporlanacaktır:

- Saldırı Senaryosu: Senaryonun adı ve kısa açıklaması
- Amaç: Saldırının ana hedefi
- Adım Adım İşleyiş: Saldırının teknik aşamaları
- Beklenen Etkiler: Sistemin saldırı sonrasında gösterdiği davranışlar
- MITRE ATT&CK Yeri: İlgili taktik ve teknik ID’si
- Log Kaynağı & Event ID: Hangi logta hangi event ID’sinde görüleceği
- Tespit Metodu: SPL sorgusu, Sigma kuralı, YARA kuralı
- Savunma Yöntemleri: Nasıl önlenir? Ne yapılmalı?
- Zincirleme Etkiler: Saldırının diğer tekniklerle ilişkisi
- Yan Etkiler: Yanlış pozitif riski, sistem performansı üzerindeki etkisi

---

## Ekstra Değer Katılan Bileşenler

- **Sigma Rule Geliştirme:** Her saldırı senaryosuna karşılık gelen Sigma kuralı yazılacak.
- **YARA Rule Geliştirme:** Atomic Red Team ataklarından binary çalıştıran/dosya oluşturan senaryolar için YARA kuralları geliştirilecek.
- **Detection-as-Code Yaklaşımı:** Tüm kurallar ve sorgular GitHub repo’sunda yönetilecek, CI/CD pipeline ile test edilebilir hale getirilecek.

---

## Kaynaklar
- 
