# Pertemuan 07 Fungsi Python
# Nama: Nada Syifa Kamilia
# NIM: 2225250089
# Kelas: 3B

# =========================
# 1. STRUKTUR FUNGSI
# =========================

def luas_persegi(sisi):
    return sisi * sisi


def luas_persegi_panjang(p, l):
    return p * l


def luas_segitiga(alas, tinggi):
    return 0.5 * alas * tinggi


def keliling_persegi(sisi):
    return 4 * sisi


# =========================
# 2. HASIL PENGUJIAN
# =========================

print("=== HASIL PENGUJIAN ===")

# Pengujian 1
hasil1 = luas_persegi(5)
harapan1 = 25
print("\nPengujian 1: Luas Persegi")
print("Input: sisi = 5")
print("Hasil yang diharapkan:", harapan1)
print("Hasil aktual:", hasil1)
print("Status:", "Berhasil" if hasil1 == harapan1 else "Gagal")

# Pengujian 2
hasil2 = luas_persegi_panjang(8, 5)
harapan2 = 40
print("\nPengujian 2: Luas Persegi Panjang")
print("Input: panjang = 8, lebar = 5")
print("Hasil yang diharapkan:", harapan2)
print("Hasil aktual:", hasil2)
print("Status:", "Berhasil" if hasil2 == harapan2 else "Gagal")

# Pengujian 3
hasil3 = luas_segitiga(6, 4)
harapan3 = 12
print("\nPengujian 3: Luas Segitiga")
print("Input: alas = 6, tinggi = 4")
print("Hasil yang diharapkan:", harapan3)
print("Hasil aktual:", hasil3)
print("Status:", "Berhasil" if hasil3 == harapan3 else "Gagal")

# Pengujian 4
hasil4 = keliling_persegi(5)
harapan4 = 20
print("\nPengujian 4: Keliling Persegi")
print("Input: sisi = 5")
print("Hasil yang diharapkan:", harapan4)
print("Hasil aktual:", hasil4)
print("Status:", "Berhasil" if hasil4 == harapan4 else "Gagal")


# =========================
# 3. REFLEKSI
# =========================

print("\n=== REFLEKSI ===")
print(
    "Program menjadi lebih sederhana karena setiap perhitungan "
    "dipisahkan ke dalam fungsi. Fungsi dapat dipanggil kembali "
    "tanpa menulis ulang rumus sehingga kode lebih rapi."
)