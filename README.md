if nama in data.keys():
      data_mahasiswa.hapus(nama)
  else:
      print("DATA TIDAK DI TEMUKAN ".format(nama))

 if data.items():
      data_mahasiswa.tampilkan()
  else:
      print("=" * 69)
      print("|" + "\t" * 3 + "DAFTAR NILAI MAHASISWA" + "\t" * 3 +
          "    |")
      print("=" * 69)
      print("| NO |   \tNAMA\t   |\tNIM \t| TUGAS | UTS | UAS | AKHIR |")
      print("=" * 69)
      print("|    " + "\t" * 3 + "TIDAK ADA DATA!" + "\t" * 4 + "    |")
      print("=" * 69)
 elif (lanjut.lower() == '4'):
    nama = str(input("Masukan Nama : "))
    data_mahasiswa.ubah(nama)
elif (lanjut.lower() == '3'):
    nama = str(input("Masukan Nama : "))
    if nama in data.keys():
        data_mahasiswa.hapus(nama)
    else:
        print("DATA TIDAK DI TEMUKAN ".format(nama))
elif (lanjut.lower() == '2'):
    if data.items():
        data_mahasiswa.tampilkan()
    else:
        print("=" * 69)
        print("|" + "\t" * 3 + "DAFTAR NILAI MAHASISWA" + "\t" * 3 +
            "    |")
        print("=" * 69)
        print("| NO |   \tNAMA\t   |\tNIM \t| TUGAS | UTS | UAS | AKHIR |")
        print("=" * 69)
        print("|    " + "\t" * 3 + "TIDAK ADA DATA!" + "\t" * 4 + "    |")
        print("=" * 69)
elif (lanjut.lower() == '5'):
    print("\nTERIMA KASIH! \n")
    exit()
else:
    print("PILIHAN MENU TIDAK ADA!")          