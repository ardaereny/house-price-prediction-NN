notlar 

ysa model katmanlarında dropout = aşırı uyumu önler overfitting -> ezberlemeyi önler
Batch size, bir eğitim veri kümesini modelin her bir güncelleme adımında kullanacağı örnek sayısını belirler
Eğitim Kaybı (Train Loss): Modelin eğitim veri kümesine ne kadar iyi uyum sağladığını ölçer. Eğitim sırasında model, veriler üzerindeki hatayı (kaybı) minimize etmeye çalışır. Bu nedenle, eğitim kaybı, modelin eğitim veri kümesine ne kadar iyi uyum sağladığını gösterir.

Doğrulama Kaybı (Validation Loss): Modelin yeni verilere (doğrulama veri kümesi gibi) ne kadar iyi genelleme yaptığını ölçer.
 Doğrulama kaybı, modelin genelleme yeteneğini gösterir. Model eğitildikten sonra, doğrulama veri kümesi üzerindeki performansı değerlendirilir ve bu kayb ölçülür.

Tek Katmanlı YSA (ADELINE): Bu model daha basit ve daha az karmaşık bir yapıya sahip olduğundan, genellikle daha az veri ile daha iyi performans gösterebilir. %80/20 ayırma oranında daha fazla eğitim verisi bulunduğundan, model daha iyi öğrenmiş ve daha doğru tahminler yapmıştır.


Tahmin Edilen Değerlerin Karşılaştırılması:

Bu grafik, her modelin gerçek fiyatlarla karşılaştırıldığında nasıl performans gösterdiğini gösterir.
Eğer her nokta yaklaşık olarak diyagonal bir çizgi boyunca yer alıyorsa, bu demektir ki modelin tahminleri gerçek değerlere oldukça yakın.
Eğer noktalar çizginin etrafında toplanmışsa, bu modelin daha tutarlı tahminler yaptığını gösterir.
Eğer noktalar çizgiden uzaklara dağılmışsa, bu modelin bazı durumlarda yanlış tahminler yaptığını gösterir.
Eğitim ve Doğrulama Kaybının Karşılaştırılması:

Bu grafik, her modelin eğitim sürecindeki performansını gösterir.
Eğitim kaybının (training loss) azalması istenir. Eğer eğitim kaybı düşüyor ve doğrulama kaybı (validation loss) da düşüyorsa, bu modelin iyi bir şekilde genelleştiği anlamına gelir. Ancak eğitim kaybı düşerken doğrulama kaybı artıyorsa, bu modelin aşırı uyum (overfitting) yaşadığını gösterebilir.
Eğer eğitim kaybı ve doğrulama kaybı arasında bir fark varsa (örneğin, eğitim kaybı düşüyor ancak doğrulama kaybı sabit kalıyorsa), bu da modelin genelleme yeteneğinin sınırlı olduğunu gösterebilir.
