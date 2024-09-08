# CONVOLUTİONAL NEURAL NETWORK

![10462_2024_10721_Fig2_HTML](https://github.com/user-attachments/assets/efc21bf5-dff3-4e77-840e-42c1db90f7ff)


Bu proje de CNN modeli ile akciğer hastalığını tespit edeceğiz. Projeyi Google Colab üzerinden yaptım. Veri setini de Kaggle üzerinden çektim. Bu bağlantıyı nasıl yaptığımı aşağıda komutlarını yazacağım.

Veri setimiz de 3 sınıf vardır. Bu sınıflar sayesinde hastalık hakkında tespit yapabiliyoruz.

Normal: Bu görüntüler sağlıklı akciğer durumlarını temsil eder ve tanı prosedürlerinde karşılaştırma için referans görevi görür.

Lung Opacity: Bu sınıf, çeşitli düzeylerde akciğer anormalliklerini gösteren ve analiz için çeşitli vakalar sağlayan X-ışını görüntülerini içerir.

Viral Pneumonia: Bu sınıftaki görseller viral zatüre vakalarıyla ilişkilendirilmiş olup, bu spesifik akciğer enfeksiyonunun anlaşılmasına ve tanımlanmasına katkıda bulunmaktadır.

<p align="center">
  <img src="https://github.com/user-attachments/assets/939423f1-08ff-4a9d-bdba-85e824a097ed" width="30%" />
  <img src="https://github.com/user-attachments/assets/6f843129-8253-41eb-9965-f58fe11157be" width="30%" />
  <img src="https://github.com/user-attachments/assets/b287c3c0-1430-411a-8eb3-b298ca4d40cd" width="30%" />
</p>


# Model Doğruluk Grafikleri

<p align="center">
  <img src="https://github.com/user-attachments/assets/f6456a7f-4861-4328-b0b0-74ee6b19bce8" width="45%" />
  <img src="https://github.com/user-attachments/assets/057ef19e-70b7-44ca-a4cd-eb0f0f18e2a2" width="45%" />
</p>

# Lung Disease Veri Seti:

Veri setine aşağıdaki linkten ulaşabilirsiniz. 

[https://www.kaggle.com/datasets/fatemehmehrparvar/lung-disease](url)

# KAGGLE VE GOOGLE COLAB BAĞLANTISI

1- Önce Drive'mıza bağlanacağız.
         from google.colab import drive
         drive.mount("/content/gdrive")

2- Drive da veri setimiz için bir dosya oluşturacağız.

         os.environ["KAGGLE_CONFIG_DIR"] = "/content/gdrive/MyDrive/Colab Notebooks"
         %cd "/content/gdrive/MyDrive/Colab Notebooks/veri3akciğer"

3- Kaggle' da proje api'sini kopyalıyoruz.

         !kaggle datasets download -d fatemehmehrparvar/lung-disease

4- Zip dosyası olarak inen veri setini zipten çıkartıyoruz.

         !unzip \*.zip && rm *.zip

5- Dosya yolunu gösterecek.

         !ls

