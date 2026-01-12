# Olio-ohjelmointi
Olio-ohjelmoinnin C++- tehtävät
#include <iostream>

#include <ctime>

/*

Satluku = 17

? 10

suurempi

? 15

suurempi

? 18

pienempi

? 17

oikein !!!

--

satunnaisluku

arvaus

*/
 
    using namespace std;

// funktion prototyypit

    int game(int maxnum);
 
    int main()

    {

    int lkm = game(50);

    cout << "Arvausten lukumaara on " << lkm << endl;

    /*

    int arvaus = 0;

    int arvausten_lkm = 0;

    // Arvotaan satunnainen luku

    srand(time(NULL));

    int satunnaisluku = (rand() % 20) + 1;

    // Kysytään pelaajalta arvaus
 
    while (arvaus != satunnaisluku) {

    cout << "Anna arvaus? " << endl;

    cin >> arvaus;

    // cout << "Pelaajan arvaus on " << arvaus << endl;

    arvausten_lkm++;

    cout << "lkm nyt " << arvausten_lkm << endl;

    // Tarkistetaan onko arvaus pienempi, suurempi tai yhtäsuuri kuin luku

    // Kerrotaan tarkistuksen tulos tyyliin ”luku on pienempi/suurempi” tai ”oikea vastaus”
 
    if (arvaus == satunnaisluku) {

        cout << " Oikein!!" << endl;

        cout << " Arvausten lukumaara on " << arvausten_lkm << endl;

    } else if (arvaus < satunnaisluku){

         cout << "Luku on suurempi!" << endl;

    } else if (arvaus > satunnaisluku) {

         cout << "Luku on pienempi!" << endl;

    }

    }

    // Jos pelaajan vastaus ei ollut oikein, niin palataan kohtaan 2.

    */
 
    return 0;

}
 
    int game(int maxnum) {

    int arvaus = 0;

    int arvausten_lkm = 0;

    // Arvotaan satunnainen luku

    srand(time(NULL));

    int satunnaisluku = (rand() % maxnum) + 1;

    // cout << "satunnaisluku on " << satunnaisluku << " maxnum on " << maxnum << endl;

    // Kysytään pelaajalta arvaus
 
    while (arvaus != satunnaisluku) {

    cout << "Anna arvaus? " << endl;

    cin >> arvaus;

    //    cout << "Pelaajan arvaus on " << arvaus << endl;

    arvausten_lkm++;

    //cout << "arvausten lkm on " << arvausten_lkm << endl;

    // Tarkistetaan onko arvaus pienempi, suurempi tai yhtäsuuri kuin luku

    // Kerrotaan tarkistuksen tulos tyyliin ”luku on pienempi/suurempi” tai ”oikea vastaus”
 
    if (arvaus == satunnaisluku) {

        cout << "Oikein!!" << endl;

    } else if (arvaus < satunnaisluku){

        cout << "Luku on suurempi!" << endl;

    } else if (arvaus > satunnaisluku) {

        cout << "Luku on pienempi!" << endl;

    }

}

    // Jos pelaajan vastaus ei ollut oikein, niin palataan kohtaan 2.
 
 
    return arvausten_lkm;

}
 
