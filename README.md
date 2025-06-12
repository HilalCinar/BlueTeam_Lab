# BlueTeam_Lab

Kurumsal sistemlerde karşılaşılan siber tehditlere karşı tespit ve yanıt mekanizmaları geliştirmek amacıyla oluşturduğum kapsamlı blue team laboratuvarı.

---

## Proje İçeriği

- Atomic Red Team frameworkü kullanılarak 14 MITRE ATT&CK taktiği çerçevesinde 100 adet saldırı senaryosu çalıştırılacak. LOLBAS araçlar da senaryolara dahil edilecek.
- Kurban sisteminde oluşan olay logları incelenerek anomali tespiti gerçekleştirilecek.
- Blue Team analizlerine göre her saldırıya özel en etkili Splunk SPL sorguları geliştirilecek.
- Kurumsal ortamlarda doğrudan kullanılabilecek tehdit tespit kuralları oluşturulacak.
- Saldırıların gerçek zamanlı izlenmesi için Splunk dashboardları tasarlanacak.

### Raporda Bulunacak Bilgiler

- Saldırı senaryosu  
- Saldırı senaryosunun amacı  
- Saldırı senaryosunun adım adım işleyişi  
- Saldırı senaryosunun sistem üzerinde beklenen etkileri  
- MITRE ATT&CK matrisindeki taktik ve teknik bazında yeri  
- İlgili log kaynağı ve event ID değerleri  
- Tespit edilmesi için kullanılan SPL sorgusu  
- İlgili saldırı senaryosundan savunma stratejileri ve tespit yöntemleri  
- Zincirleme etkileri ve olası yan etkiler  

### Ekstra Bileşenler

- Her saldırı senaryosuna karşılık gelen Sigma kuralı yazılacak.  
- Binary çalıştıran veya dosya oluşturan Atomic Red Team senaryoları için YARA kuralı geliştirilecek.
