# CCNA VLAN & Trunking Lab

## 📌 Proje Özeti
Bu çalışma, Cisco Packet Tracer üzerinde temel **VLAN, Access Port, Trunk, Switch IP ve Telnet** yapılandırmalarını kapsayan bir CCNA uygulama labıdır.  
Amaç, aynı VLAN’daki cihazların haberleşmesini sağlamak, farklı VLAN’ların izole olduğunu göstermek ve switch yönetimine **Telnet üzerinden erişimi** test etmektir.

---

## 🔹 Yapılan Konfigürasyonlar

### VLAN Oluşturma ve İsimlendirme
- VLAN 2 → SUNUCULAR  
- VLAN 3 → BILGI_ISLEM  
- VLAN 4 → MISAFIR  

### Access Port Atamaları
- Port 1–10 → VLAN 4 (Misafir)  
- Port 11–20 → VLAN 2 (Sunucular)  
- Port 21–24 → VLAN 3 (Bilgi İşlem)  

### Trunk Yapılandırması
- Switchler arası bağlantılar **trunk** moda alındı.  

### Switch VLAN IP Yapılandırmaları
- SW1 → `192.168.3.11/24`  
- SW2 → `192.168.3.12/24`  
- SW3 → `192.168.3.13/24`  

### Hostname, Enable Secret ve Telnet
- Hostname: **SW1, SW2, SW3**  
- Enable Secret: **cisco**  
- Telnet Password: **cisco**  

---

## 🔹 Testler ve Sonuçlar
- ✅ Sunucular (VLAN2) kendi aralarında **ping başarılı**  
- ✅ Misafirler (VLAN4) kendi aralarında **ping başarılı**  
- ✅ Bilgi İşlem (VLAN3) → hem kendi aralarında hem de SW1–SW3’e **ping başarılı**  
- ✅ VLAN’lar arası iletişim **yok** (tasarım gereği)  
- ✅ `show cdp neighbor` ile switch bağlantıları **doğrulandı**  
- ✅ Telnet üzerinden SW1, SW2, SW3 erişimi **sağlandı**  

---

## 📂 Dosyalar
- `CCNA_VLAN_Lab.pkt` → Packet Tracer proje dosyası  
- `screenshots/` → Test çıktılarının ekran görüntüleri  

---

✍️ **Hazırlayan:** Zeynep  
📅 **Tarih:** 2025
