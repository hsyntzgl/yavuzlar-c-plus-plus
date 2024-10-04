# 2.0 Fonksiyonlar

C++ dilinde fonksiyonlar, belirli bir işlevi yerine getirmek üzere tanımlanmış kod bloklarıdır. Fonksiyonlar, kodun tekrar kullanılabilirliğini artırır, modüler yapıyı destekler ve programın okunabilirliğini sağlar.

**Fonksiyon Tanımlama**

Bir fonksiyon tanımlarken, dönüş tipi, fonksiyon adı ve parametre listesi belirtilir. Aşağıda bir fonksiyonun genel yapısı yer almaktadır:

```cpp
return_type function_name(parameter_type parameter_name) {
    // Fonksiyonun gövdesi
    // İşlemler
    return value; // Dönüş tipi varsa
}
```

**Örnek: Basit Bir Fonksiyon**

```cpp
#include <iostream>
using namespace std;

// Fonksiyon tanımı
void greet() {
    cout << "Merhaba, C++ Dünyası!" << endl;
}

int main() {
    greet(); // Fonksiyonu çağırma
    return 0;
}
```

Bu örnekte, `greet` isimli bir fonksiyon tanımlanmış ve çağrılmıştır. Bu fonksiyon, ekrana bir mesaj yazdırır.

**Parametreli Fonksiyonlar**

Fonksiyonlar, parametre alarak daha dinamik hale getirilebilir. Fonksiyon tanımında parametreler belirtilir ve fonksiyon çağrılırken bu parametrelere değerler atanır.

**Örnek: Parametreli Fonksiyon**

```cpp
#include <iostream>
using namespace std;

// Fonksiyon tanımı
void add(int a, int b) {
    cout << "Toplam: " << (a + b) << endl;
}

int main() {
    add(5, 10); // 5 ve 10 değerlerini parametre olarak gönderme
    return 0;
}
```

Bu örnekte, `add` fonksiyonu iki tam sayıyı toplar ve sonucu ekrana yazdırır.

**Dönüş Değeri Olan Fonksiyonlar**

Fonksiyonlar, belirli bir veri tipinde değer döndürebilir. Dönüş tipi, fonksiyonun tanımında belirtilir.

**Örnek: Dönüş Değeri Olan Fonksiyon**

```cpp
#include <iostream>
using namespace std;

// Fonksiyon tanımı
int multiply(int a, int b) {
    return a * b; // Çarpım sonucunu döndürme
}

int main() {
    int result = multiply(4, 5); // Fonksiyonu çağırma
    cout << "Çarpım: " << result << endl; // Sonucu yazdırma
    return 0;
}
```

Bu örnekte, `multiply` fonksiyonu iki sayıyı çarpar ve sonucu döndürür.

**Fonksiyon Aşırı Yükleme (Function Overloading)**

C++ dilinde, aynı isimde birden fazla fonksiyon tanımlanabilir. Bu durum, fonksiyonun parametre sayısı veya türü farklı olduğunda mümkündür.

**Örnek: Fonksiyon Aşırı Yükleme**

```cpp
#include <iostream>
using namespace std;

// Fonksiyon tanımları
int add(int a, int b) {
    return a + b; // Tam sayı toplama
}

double add(double a, double b) {
    return a + b; // Ondalık toplama
}

int main() {
    cout << "Tam Sayı Toplama: " << add(5, 10) << endl; // 15
    cout << "Ondalık Toplama: " << add(5.5, 10.2) << endl; // 15.7
    return 0;
}
```

Bu örnekte, `add` fonksiyonu tam sayı ve ondalık sayılar için iki ayrı tanımda yer almıştır.
