# 🎮 AI Tabanlı Tic-Tac-Toe (XOX)

Bu proje, klasik Tic-Tac-Toe oyununu farklı yapay zeka algoritmalarıyla (Minimax ve Q-Learning) deneyimlemenizi sağlayan gelişmiş bir Python uygulamasıdır. Sistem, 200.000 maçlık bir eğitim sürecinden geçerek "yenilmez" bir rakibe dönüşebilir.

---

## ✨ Özellikler

* **Q-Learning (Pekişmeli Öğrenme):** Ajan, oyunları oynayarak ödül ve ceza mekanizmasıyla (`Q-Table`) kendi stratejisini geliştirir.
* **Minimax Algoritması:** Tüm olası hamleleri tarayarak en optimal sonucu seçen, kusursuz oyun mantığı.
* **Farklı Oyuncu Tipleri:** * `RandomPlayer`: Rastgele hamle yapar.
  * `MinimaxPlayer`: Kaybetmesi imkansız olan klasik AI.
  * `QLearningPlayer`: Deneyimledikçe akıllanan yapay zeka.
  * `MinimuddledPlayer`: Bazen hata yapan "insansı" AI.
* **Eğitim Modu:** Program başladığında iki yapay zeka ajanı arka planda binlerce maç yaparak strateji öğrenir.

---

## 🛠 Teknik Mimari

Proje, oyun teorisi ve makine öğrenmesi prensiplerini temel alır:



* **Minimax & Alpha-Beta Budama:** Gereksiz hamleleri eleyerek hesaplama süresini optimize eder.
* **Q-Learning Denklemi:** $Q(s, a) \leftarrow Q(s, a) + \alpha [r + \gamma \max Q(s', a') - Q(s, a)]$ formülü kullanılarak hamlelerin değeri (Q-değeri) güncellenir.
* **Epsilon-Greedy Stratejisi:** Ajanın yeni hamleleri keşfetmesi (`exploration`) ve bildiği en iyi hamleyi yapması (`exploitation`) arasındaki dengeyi sağlar.

---

## 🚀 Kurulum ve Çalıştırma

Uygulama herhangi bir harici kütüphane gerektirmez (Standart Python kütüphaneleri yeterlidir).

1. Projeyi bilgisayarınıza indirin.
2. Terminal üzerinden çalıştırın:
   ```bash
   python tictactoe_ai.py
