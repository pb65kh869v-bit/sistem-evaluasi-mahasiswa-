# Program python: Sistem Evaluasi Mahasiswa

# 1. Input nilai tugas, Uts, Uas, dan kehadiran mahasiswa
tugas = float(input("Masukkan nilai Tugas (0-100): "))
uts = float(input("Masukkan nilai UTS (0-100): "))
uas = float(input("Masukkan nilai UAS (0-100): "))
kehadiran = float(input("Masukkan persentase kehadiran (0-100): "))

# 2. Hitung Nilai Akhir - menggunakan operator aritmatika
nilai_akhir = (0.20 * tugas) + (0.30* uts) + (0.50 * uas)

#Tampilkan nilai akhir 
print(f"/nNilai Akhir:{nilai_akhir:.2f}")
pront(f"Kehadiran: {kehadiran}%")

# 3, 4, 5, 6. Evaluasi kelulusan dan predikat menggunakan percabangan (if,elif,else)
if nilai_akhir >= 85 and kehadiran >= 90 and nilai_akhir % 2 == 0:
    status = "LULUS DENGAN PREDIKAT"
elif nilai_akhir >= 75 and kehadiran >= 80:
    status = "LULUS"
else:
    status = "BELUM LULUS"

# Tampilkan hasil akhir
print(f"Status: {status}")
