# 1.13 While Döngüsü

C++ dilinde **while** döngüsü, belirli bir koşul sağlandığı sürece bir kod bloğunu tekrar tekrar çalıştırmak için kullanılır. Bu döngü, koşulun doğru olduğu sürece çalışmaya devam eder. Eğer koşul başlangıçta yanlışsa, döngü gövdesi bir kez bile çalıştırılmayabilir.

**Temel Yapı**

**while** döngüsünün temel yapısı şu şekildedir:

```cpp
while (koşul) {
    // Çalıştırılacak kod bloğu
}
```

**Örnek: Basit Bir Sayma**

Aşağıdaki örnekte, bir değişkenin değeri 1'den başlayarak 5'e kadar sayan bir while döngüsü gösterilmektedir:

```cpp
#include <iostream>
using namespace std;

int main() {
    int sayi = 1;

    while (sayi <= 5) {
        cout << "Sayi: " << sayi << endl;
        sayi++;  // Değişkeni artır
    }

    return 0;
}
```

**Önemli Noktalar**

1. **Koşul Kontrolü**: Döngünün her yinelemesinde koşul kontrol edilir. Eğer koşul doğruysa, döngü gövdesi çalıştırılır.
2. **Değişken Güncelleme**: Döngü içinde kullanılan değişkenlerin güncellenmesi önemlidir. Aksi takdirde, döngü sonsuz döngüye girebilir.
3. **Sonsuz Döngü**: Eğer koşul hiçbir zaman yanlış olmazsa (örneğin, `while (true)` şeklinde bir ifade), döngü sonsuz döngüye girer. Bu durumda döngüyü kırmak için `break` ifadesi kullanılabilir.

**Örnek: Kullanıcıdan Girdi Alma**

Aşağıdaki örnekte, kullanıcıdan sürekli olarak bir sayı alıp, kullanıcı 0 girdiğinde döngüyü kıran bir while döngüsü gösterilmektedir:

```cpp
#include <iostream>
using namespace std;

int main() {
    int girdi;

    cout << "Bir sayi girin (0 ile çıkış yapar): ";

    while (true) { // Sonsuz döngü
        cin >> girdi;

        if (girdi == 0) {
            break; // Döngüyü kır
        }

        cout << "Girdiğiniz sayı: " << girdi << endl;
    }

    return 0;
}
```
