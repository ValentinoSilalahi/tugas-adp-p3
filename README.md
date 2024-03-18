#include <iostream>

using namespace std;

int main()
{
    string tujuan,kelas;
    int htujuan,hkelas,tiket,total,total_akhir,diskon;

    cout << " Nama : Valentino Silalahi "<<endl;
    cout << " Nim  : 2310431015 "<<endl;
    cout << " Program Bus PT.ANS Lintas Sumatera "<<endl;

    cout <<endl<< " Tujuan Bus PT.ANS : "<<endl;
    cout << " 1. Medan   ( Rp300.000 ) "<<endl;
    cout << " 2. Padang  ( Rp50.000  ) "<<endl;
    cout << " 3. Jambi   ( Rp250.000 ) "<<endl;
    cout << " 4. Sibolga ( Rp100.000 ) "<<endl;
    cout << " 5. Pakkat  ( Rp200.000 ) "<<endl;
    cout << " 6. Solok   ( Rp70.000  ) "<<endl;

    cout << " Masukkan tujuan anda : ";
    cin >> tujuan;

    if ( tujuan == "Medan" ) { htujuan=300000; }
    else { if ( tujuan == "Padang" ) { htujuan=50000; }
    else { if ( tujuan == "Jambi" ) { htujuan=250000; }
    else { if ( tujuan == "Sibolga" ) { htujuan=100000; }
    else { if ( tujuan == "Pakkat" ) { htujuan=200000; }
    else { if ( tujuan == "Solok" ) { htujuan=70000; }
    else { cout << " Tujuan anda tidak terdaftar "; } } } } } }

    cout << " Tujuan anda adalah = " << tujuan << " || Dengan harga = Rp" << htujuan << endl;
    cout <<endl<< " ----------------------------------- "<<endl;

    cout <<endl<< " Kelas Bus PT.ANS : " <<endl;
    cout << " 1. Ekonomi ( Rp10.000 ) " <<endl;
    cout << " 2. Bisnis  ( Rp20.000 ) " <<endl;
    cout << " 3. First   ( Rp30.000 ) " <<endl;

    cout << " Masukkan kelas anda : ";
    cin >> kelas;

    if ( kelas == "Ekonomi" ) { hkelas=10000; }
    else { if ( kelas == "Bisnis" ) { hkelas=20000; }
    else { if ( kelas == "First" ) { hkelas=30000; }
    else { " Kelas anda tidak terdaftar "; } } }

    cout << " Kelas anda adalah = " << kelas << " || Dengan harga = Rp" << hkelas << endl;
    cout << " Jumlah tiket anda = "; cin >> tiket;
    cout <<endl<< " ----------------------------------- "<<endl;

    total = ( htujuan+hkelas )*tiket;

    if ( tiket > 5 ) { diskon=0.10*total; }
    else { if ( tiket >= 3 ) { diskon=0.05*total; }
    else { diskon=0*total; } }

    total_akhir = total-diskon;

    cout <<endl<< " Tujuan : " << tujuan <<endl;
    cout << " Kelas : " << kelas <<endl;
    cout << " Jumlah tiket : " << tiket <<endl;
    cout << " Total harga tiket anda = Rp" << total <<endl;
    cout << " Diskon yang didapat = Rp" << diskon <<endl;
    cout << " Total harga setelah diskon = Rp" << total_akhir <<endl;
}

