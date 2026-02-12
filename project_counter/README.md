# TIA Portal Motor Kontrol Projesi (Counter ile)

## Uygulama Açıklaması
Bu proje, Siemens TIA Portal kullanılarak geliştirilmiş bir sıralı motor kontrol uygulamasıdır.  
Projede üç motor ve her motor için termik koruma devresi bulunur.  
Motorların sıralı çalışması start butonuna basıldıkça artan bir counter ile kontrol edilir.

---

## Çalışma Mantığı

### Start Butonu ve Counter
- **1. basış (counter = 1):** Motor 1 çalışır  
- **2. basış (counter = 2):** Motor 1 ve Motor 2 çalışır  
- **3. basış (counter = 3):** Motor 1, Motor 2, Motor 3 çalışır  
- **4. basış (counter = 4):** Reset aktif olur, tüm motorlar durur ve counter sıfırlanır  

### Termik Koruma
- Her motorun kendi termiği vardır.  
- Termik attığında sadece ilgili motor durur, diğer motorlar çalışmaya devam eder.  
- Böylece aşırı akım durumunda sistem güvenliği sağlanır.

---

## Kullanım

- Start butonuna basarak motorların sıralı çalışması test edilir.  
- Termikler ile simülasyon da aşırı akım durumları test edilir.