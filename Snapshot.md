 ![Ekran görüntüsü 2025-01-18 020223](https://github.com/user-attachments/assets/f37c4065-cc00-44c4-bcfd-09474ec17ba0)



🚀 Snapshot Loader Humanode ağı için kolay, hızlı ve güvenli bir şekilde yedek ```(snapshot)``` indirme ve kurulum işlemlerini gerçekleştiren bir bash scriptidir. Bu araç, Humanode düğümünüzü ```(node)``` belirli bir bloktan başlatmanızı sağlar ve kurulum sürecini basitleştirir.

### Özellikler 
- 🌟 **Kolay Kurulum**: Tek bir komut ile yedek dosyasını indirin, yükleyin ve düğümünüzü başlatın.
- 📦 **Gereksinim Kontrolü**: İhtiyaç duyulan tüm bağımlılıkları otomatik kontrol eder ve yükler.
- ⏱️ **Modern İlerleme Çubuğu**: İndirme hızını, geçen süreyi görselleştirir.
- 🛡️ **Güvenilirlik**: Özel tasarımıyla Humanode ağı için optimize edilmiştir.

### Nasıl Çalışır? 
İster yeni kurulum yapın, ister taşıma yapın farketmez ilk önce düğümünüzü kurun normal bir şekilde. Humanode uygulamasında ```(launcher)``` bulunan ```log``` kısmına gidin. Bir kaç blok geçtikten sonra uygulamada ki ```stop``` butonuna basarak düğümünüzü durdurun. Humanode'nun kurulu olduğu sunucuya giriş yapın terminal üzerinden. Yedek kurulumuna aşağıda ki komutlarla devam edin...

### Katkı
Bu projeye katkıda bulunmak isterseniz, lütfen bir pull request gönderin veya bir issue oluşturun.

------

# Yedek Kurulum Adımları

1- Eski düğümün dosyalarını silin.
```4D
rm -rf /root/.humanode/workspaces/default/substrate-data/chains/humanode_mainnet/db/full
```

2- Aşağıda ki komut ile kurulumu başlatın.

```Sieve
curl -s http://humanodesnapshot.lorentochain.online/Humanode-Snapshot-Loader.sh | bash
```

3- Kurulum tamamlandıktan sonra tekrardan Humanode uygulamasına giriş yapın ve ```Start The Node``` butonuna basın. 

> [!CAUTION]
> :warning: Yedek dosyasının kurulum sistemi güncellendi. Daha önce, dosya indirilirken aynı anda kurulum gerçekleşiyordu. Ancak, yeni versiyonda işlem iki aşamaya ayrıldı: Önce dosya indiriliyor, ardından kurulum tamamlanıyor. Bu, işlem sırasında biraz daha fazla beklemeniz gerekebileceği anlamına geliyor. Ayrıca, bekleme süresi sunucunuzun internet hızına bağlı olarak değişiklik gösterebilir. Eğer indirme hızı çok düşükse, ```sudo reboot``` komutunu kullanarak sunucunuzu yeniden başlatabilir ve işlemi tekrar deneyebilirsiniz.
>
> :warning: Dikkat: Yedek kurulumu tamamlanmadan terminali kapatmayın! Aksi takdirde işlem yarım kalacaktır!
> 
> :warning: Eğer uygulama çalışmazsa o zaman ```Node Validator Key``` yeşil olana kadar uygulamayı bir kaç kere kapatıp geri açın. Genelde uygulamayı 2-3 kere katıp açtıktan sonra düzeliyor.

![Ekran görüntüsü 2024-11-09 053456](https://github.com/user-attachments/assets/15d1ae14-4eeb-4afc-bf3e-159fb12ec4a1)![gggg](https://github.com/user-attachments/assets/03814192-f9d3-43bc-bd65-47558ad7c4af)


---



