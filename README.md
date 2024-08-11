# Capstone-project-3-Telco-Customer-Churn
<h1> Capstone Project 3 </h1>
Context :
Telco Customer Churn merupakan salah satu segmen terbesar di perusahaan kami, Platform jaringan moratelindo dibangun, dioperasi dan layananan diperluas sesuai kebutuhan telcom. dengan adanya  **Dampak Jenis Kontrak pada Loyalitas Pelanggan** ada beberapa Jenis kontrak (misalnya, Month-to-month, One year, Two year) bisa berpengaruh pada keputusan pelanggan untuk bertahan atau churn. Kontrak jangka panjang mungkin mengurangi kemungkinan churn.


Permasalahan :
 jenis kontrak mempengaruhi tingkat churn pelanggan dalam perusahaan telekomunikasi ada korelasi atau pengaruh signifikan antara jenis kontrak yang dipilih oleh pelanggan (seperti Month-to-month, One year, Two year) terhadap keputusan mereka untuk tetap bertahan atau berhenti (churn) dari layanan sedikit peningkatan dalam retensi klien meningkatan penjualan dan keuntungan secara dramatis
 

Goals :  Menganalisis Korelasi antara Jenis **Kontrak** dan **Churn**: Menentukan bagaimana berbagai jenis **kontrak** (Month-to-month, One year, Two year) berkorelasi dengan tingkat **churn**  pelanggan sehingga mengoptimalkan pesaingan menggunakan data ini.

Metrik Evaluation
Type 1 error : False Positive 
Konsekuensi: sia-sianya biaya perekrutan, waktu dan sumber daya
Type 2 error : False Negative 
Konsekuensi kehilangan pelanggan dan harus membayar semua biaya untuk memperoleh pelanggan pengganti 

Mengoptimalkan Penawaran Kontrak: Berdasarkan hasil analisis, mengembangkan strategi untuk menyesuaikan penawaran kontrak kepada pelanggan.

<b>Concusion</b>:
Berdasarkan analisis yang telah dilakukan, model yang paling sesuai untuk kasus ini adalah Regresi Logistik dengan penyetelan hiperparameter yang optimal.
Hiperparameter terbaik yang ditemukan adalah: {C: 0.1, penalty: 12}.
Model ini menunjukkan performa yang cukup baik dengan nilai Recall dan Precision masing-masing sebesar 81% dan 52% (berdasarkan kelas recall(+)).
Dalam skenario yang telah dirancang, implementasi model ini dapat menghemat biaya hingga 50% dibandingkan dengan jika model tidak digunakan sama sekali.
<br/>

<b>Recommendation</b> :
Implementasi model ini terbatas pada situasi di mana biaya churn pelanggan sekitar 5 kali lebih besar daripada biaya retensi. Di luar kondisi ini, keandalan model (dengan p-value rendah) akan berbeda, karena kinerja model sangat bergantung pada metrik evaluasi yang digunakan dalam perhitungan biaya.
Disarankan untuk menambahkan fitur-fitur tambahan dalam pemilihan fitur, seperti metode pembayaran yang digunakan, layanan streaming, atau aspek lain yang relevan dengan domain layanan telekomunikasi.
Cobalah berbagai kombinasi rekayasa fitur dan eksplorasi algoritma Pembelajaran Mesin lainnya untuk meningkatkan kinerja model.
