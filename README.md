Pertanyaan 5.2
1. bagian if berfungsi sebagai base case untuk menghentikan rekursi ketika nilai sudah mencapai kondisi tertentu (misalnya n = 1). Sedangkan bagian else berfungsi sebagai recursive case yang digunakan untuk memecah masalah dengan memanggil fungsi kembali menggunakan nilai yang lebih kecil (n-1).
2. modifikasi.
3. fakto *= i; digunakan pada metode iteratif (Brute Force) dengan perulangan, di mana nilai fakto dikalikan secara bertahap dengan nilai i dalam loop. Sedangkan int fakto = n * faktorialDC(n-1); digunakan pada metode rekursif (Divide and Conquer), di mana nilai faktorial dihitung dengan memanggil fungsi itu sendiri dengan nilai yang lebih kecil (n-1) hingga mencapai kondisi dasar.
4. faktorialBF() menggunakan pendekatan iteratif (Brute Force) dengan perulangan untuk menghitung faktorial secara bertahap dari 1 hingga n. Sedangkan faktorialDC() menggunakan pendekatan rekursif (Divide and Conquer) dengan memanggil fungsi itu sendiri menggunakan nilai yang lebih kecil hingga mencapai kondisi dasar. Dengan demikian, faktorialBF() bekerja dengan loop, sedangkan faktorialDC() bekerja dengan rekursi.

Pertanyaan 5.3
1. method pangkatBF() menggunakan pendekatan iteratif (Brute Force) dengan perulangan, yaitu mengalikan nilai secara berulang sebanyak n kali hingga menghasilkan nilai pangkat. Sedangkan method pangkatDC() menggunakan pendekatan rekursif (Divide and Conquer), yaitu memecah perhitungan menjadi bagian lebih kecil dengan membagi pangkat menjadi dua, kemudian memanggil fungsi secara berulang hingga mencapai kondisi dasar.
2. sudah. return (pangkatDC(a, n/2)*pangkatDC(a, n/2)*a); return (pangkatDC(a, n/2)*pangkatDC(a, n/2));
3. method pangkatBF() tidak harus memiliki parameter karena class Pangkat sudah memiliki atribut nilai dan pangkat. Oleh karena itu, method tetap dapat berjalan tanpa parameter dengan langsung menggunakan atribut tersebut. Method tanpa parameter bisa dibuat seperti berikut:
int pangkatBF() {
    int hasil = 1;
    for(int i = 0; i < pangkat; i++){
        hasil = hasil * nilai;
    }
    return hasil;
}
method menjadi lebih sederhana karena tidak perlu menerima input lagi, cukup menggunakan data yang sudah ada di dalam objek.
4. pangkatBF() menggunakan pendekatan iteratif (Brute Force) dengan melakukan perkalian berulang sebanyak nilai pangkat. Sedangkan pangkatDC() menggunakan pendekatan rekursif (Divide and Conquer), yaitu dengan membagi pangkat menjadi dua bagian lalu menggabungkan hasilnya kembali. Dengan demikian, pangkatBF() bekerja secara sederhana dengan perulangan, sedangkan pangkatDC() lebih efisien karena mengurangi jumlah operasi melalui rekursi.
