def dress_up_game():
    # Senarai barangan baju
    barangan_baju = ["tudung", "baju kurung putih", "kain biru", "kasut sekolah"]
    
    # Pakaian yang sesuai untuk ke sekolah
    pakaian_sekolah = ["tudung", "baju kurung putih", "kain biru", "kasut sekolah"]
    
    # Pakaian yang dipilih oleh pemain
    pilihan_pemain = []
    
    print("Selamat datang ke permainan Dress Up!")
    print("Anda perlu memilih pakaian yang sesuai untuk ke sekolah.")
    print("Barangan baju yang tersedia adalah:")
    
    # Memaparkan barangan baju
    for baju in barangan_baju:
        print(f"- {baju}")
    
    # Pemain memilih pakaian
    for item in barangan_baju:
        pilihan = input(f"Adakah anda ingin memakai {item}? (ya/tidak): ").lower()
        if pilihan == "ya":
            pilihan_pemain.append(item)
    
    # Memeriksa pilihan pemain
    if set(pilihan_pemain) == set(pakaian_sekolah):
        print("Tahniah! Anda telah memilih pakaian yang sesuai untuk ke sekolah. Anda boleh pergi ke sekolah!")
    else:
        print("Maaf, anda telah memilih pakaian yang tidak sesuai untuk ke sekolah. Anda tidak boleh pergi ke sekolah.")

if __name__ == "__main__":
    dress_up_game()
