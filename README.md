# Pertemuan 07 Fungsi Python
# Nama: Nada Syifa Kamilia
# NIM: 2225250089
# Kelas: 3B

# 1. TUJUAN
# Menggunakan fungsi, parameter, return value, dan scope
# untuk membuat program modular.


# 2. CARA MENJALANKAN
# Jalankan pada terminal:
# python3 praktik/utilitas_matematika.py


# 3. STRUKTUR FUNGSI

def luas_persegi(sisi):
    return sisi * sisi


def luas_persegi_panjang(p, l):
    return p * l


def luas_segitiga(alas, tinggi):
    return 0.5 * alas * tinggi


def keliling_persegi(sisi):
    return 4 * sisi


def volume_kubus(sisi):
    return sisi ** 3


# 4. HASIL PENGUJIAN

def pengujian():
    data_uji = [
        ("Luas persegi", "sisi=4", luas_persegi(4), 16),
        ("Luas persegi panjang", "p=8, l=5",
         luas_persegi_panjang(8, 5), 40),
        ("Luas segitiga", "alas=10, tinggi=6",
         luas_segitiga(10, 6), 30),
        ("Keliling persegi", "sisi=5",
         keliling_persegi(5), 20),
        ("Volume kubus", "sisi=3",
         volume_kubus(3), 27),
    ]

    print("HASIL PENGUJIAN")
    print("-" * 75)
    print(f"{'Fungsi':25} {'Input':20} {'Harapan':10} {'Aktual':10} Status")

    for nama, input_data, aktual, harapan in data_uji:
        status = "LULUS" if aktual == harapan else "GAGAL"
        print(
            f"{nama:25} {input_data:20} "
            f"{harapan:<10} {aktual:<10} {status}"
        )


# 5. REFLEKSI
# Program lebih sederhana karena rumus matematika
# dipisahkan menjadi fungsi yang dapat digunakan kembali.


if __name__ == "__main__":
    print("PROGRAM UTILITAS MATEMATIKA")
    print("=" * 35)

    print("Luas persegi:", luas_persegi(4))
    print("Luas persegi panjang:", luas_persegi_panjang(8, 5))
    print("Luas segitiga:", luas_segitiga(10, 6))
    print("Keliling persegi:", keliling_persegi(5))
    print("Volume kubus:", volume_kubus(3))

    print()
    pengujian()

    print("\nREFLEKSI")
    print(
        "Program menjadi lebih sederhana karena setiap rumus "
        "dibuat dalam fungsi tersendiri sehingga dapat digunakan "
        "kembali tanpa menulis ulang rumus."
    )