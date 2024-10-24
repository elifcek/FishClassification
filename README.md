**PROJE ÖZETİ**
Bu projede, kullanılan veri seti başarıyla yüklenmiş ve veriler kaynağından alınarak işlenmiştir. Veri seti, CSV formatında hazırlanmış ve gerekli kütüphaneler yüklenmiştir. Yüklenen veriler üzerinde gerekli ön işleme adımları uygulanmıştır; eksik veriler, fillna yöntemiyle tamamlanmış, kategorik veriler ise LabelEncoder yardımıyla sayısal verilere dönüştürülmüştür. Veriler, modelin eğitimi ve test edilmesi amacıyla train_test_split fonksiyonu ile %80 eğitim ve %20 test oranında ikiye ayrılmıştır.

Keras kütüphanesi kullanılarak derin öğrenme modeli inşa edilmiş, model çeşitli katmanlar eklenerek yapay sinir ağı mimarisi doğrultusunda derinleştirilmiştir. Modelin derlenmesi esnasında kayıp fonksiyonu ve optimizasyon yöntemi belirlenmiş, performansı artırmak için Adam optimizasyon algoritması kullanılmıştır (model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])). Model, fit fonksiyonu ile eğitim verileri üzerinde eğitilmiş, eğitimin süresi ve batch boyutu ayarlanmıştır.

Eğitilen model, test verileri üzerinde evaluate fonksiyonu ile test edilmiş ve doğruluk oranı hesaplanmıştır (test_loss, test_accuracy = model.evaluate(X_test, y_test)). Elde edilen sonuçlar detaylı bir şekilde analiz edilip modelin performansı değerlendirilmiştir. Sonuçlar grafikler aracılığıyla görselleştirilmiş ve performans metrikleri yorumlanmıştır.

Her adımda kullanılan terimler: Eğitim (Training): Modelin verilerle öğrenme süreci. Test (Testing): Modelin öğrenilen bilgileri yeni verilere uygulama süreci. Katman (Layer): Yapay sinir ağındaki bilgi işleme birimi. Optimizasyon (Optimization): Modelin kayıp fonksiyonunu minimize etme süreci. Aktivasyon Fonksiyonu (Activation Function): Katmanların çıktısını belirleyen matematiksel fonksiyonlar.

**Proje Linki:** https://www.kaggle.com/code/atahankarata/fish-classification

**Bu projeyi Atahan Karataş ile birlikte tamamladık.**
