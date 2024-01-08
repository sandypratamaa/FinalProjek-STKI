**Dataset**:  dataset yang digunakan bisa diakses melalui link https://github.com/ksnugroho/klasifikasi-spam-sms/blame/master/data/dataset_sms_spam_v1.csv  


**Permasalahan dan Tujuan** : 
Permasalahan terjadi akibat pesan masuk yang kita tidak mengetahui apakah pesan tersebut termasuk penipuan/spam, pesan normal atau pesan promo, adanya aplikasi klasifikasi sms spam memiliki tujuan untuk mengklasifikasi pesan di SMS apakah termasuk dalam kategori Spam, normal, atau promo. Jadi dapat memudahkan pengguna untuk dapat mengklasifikasi pesan masuk mereka.

**Langkah-langkah penyelesaian kasus klasifikasi SMS spam meliputi**:  
1. Data Acquisition : penggunaan dataset

2. Exploratory Data Analysis (EDA) : melakukan eksplorasi pada dataset yang digunakan

3. Pre-processing, tahap preprocessingnya meliputi :

Case Folding : Mengubah semua huruf dalam teks menjadi huruf kecil atau huruf besar untuk konsistensi. Misalnya, mengubah "TeKs" menjadi "teks" atau "TEKS" untuk memastikan bahwa perbedaan huruf besar/kecil tidak memengaruhi analisis atau pencarian teks.

Filtering :Menghilangkan atau menyaring elemen yang tidak diinginkan dari teks. Ini dapat mencakup menghapus karakter khusus, tanda baca, atau simbol tertentu yang tidak relevan untuk analisis atau pemrosesan yang sedang dilakukan.

Stopword :Menghilangkan kata-kata umum atau kata-kata penghubung yang tidak memberikan kontribusi signifikan pada pemahaman konten. Stopwords seperti "dan", "atau", "saya", dll., sering diabaikan dalam analisis teks karena kemunculannya yang tinggi dan kontribusinya yang rendah terhadap makna inti.

Stemming :Mengubah kata-kata menjadi bentuk dasar atau akar kata mereka. Ini dilakukan dengan menghapus akhiran atau awalan kata, sehingga kata-kata dengan bentuk yang berbeda tetapi memiliki makna yang mirip dapat dianggap sama. Tujuan utamanya adalah untuk mengurangi variasi kata dan meningkatkan efisiensi dalam pemrosesan dan analisis teks.

4. Feature Engineering terbagi 2 tahap yaitu :

   Feature Extraction - TF IDF

   Feature Selection - Chi-Square

5. Modelling (Machine Learning) yaitu dengan Memisihkan data training dan data testing dengan perbandingan 80:20, training Model dengan algorithm  MultinomialNB

6. Prediction : melihat hasil prediksi dari data uji dan data latih

7. Model Evaluation : melihat perhitungan akurasi model yaitu mendapatkan akurasi sebesar 95% untuk data train dan 91% untuk data test


**Performa Model** : Uji performa model mendapatkan akurasi sebesar 95% untuk data train dan 91% untuk data test  


**Proses Deployment** : Proses deployment menggunakan Streamlit, jadi langkah yang perlu dilakukan adalah membuat file .py dan juga requirement.txt kemudian membuka web streamlit dan menyambungkan ke github, dan jalankan proses deploy, apabila tidak ada error maka web akan berjalan dan dapat digunakan.
