---
description: >-
  C++ dilinde değişkenler, bir veri tipini ve bir ad (değişken adı) belirterek
  tanımlanır. Değişkenler, belirli bir değeri depolamak ve bu değeri programın
  çeşitli yerlerinde kullanmak için kullanılır.
---

# 1.4 C++ Değişkenleri

## C++ Değişkenleri Oluşturma

Değişken tanımlamak için önce veri tipini, ardından değişken adını ve isteğe bağlı olarak başlangıç değerini belirtmelisiniz.

```
#include <iostream>

int main() {
    std::string name = "Hüseyin Tazegül"; // Metin (string) tipi değişken
    int age = 26; // Sayısal (integer) tipi değişken
    
    std::cout << "Ad: " << name << std::endl; // Ad: Hüseyin Tazegül
    std::cout << "Yaş: " << age << std::endl; // Yaş: 26

    return 0;
}
```

>
>
> * **Değişkenlerin Veri Tipi:**
>   * C++ dilinde, değişken tanımlarken veri tipi (`int`, `float`, `double`, `string` vb.) belirtilmelidir.
>   * Örneğin: `int age = 26;` ifadesinde `int` veri tipini, `age` ise değişken adını temsil eder.
> * **Büyük/Küçük Harf Duyarlılığı:**
>   * C++’ta değişken adları büyük/küçük harf duyarlıdır. Yani `age` ve `Age` farklı değişkenlerdir.
> * **Değişken İsimlendirme Kuralları:**
>   * Değişken adı bir harf veya alt çizgi (\_) ile başlamalıdır.
>   * Değişken adı bir sayı ile başlayamaz.
>   * Değişken adı yalnızca alfasayısal karakterler (A-Z, a-z, 0-9) ve alt çizgi (\_) içerebilir.
>   * Değişken adı bir fonksiyon adı veya özel bir kod adı olamaz.
>   * Özel karakterler (örneğin `@`, `#`, `$`, vb.) kullanılamaz.

```
int age = 23; // Bu "age" değişkenidir.
int Age = 45; // Bu ise "Age" değişkenidir ve farklı bir değişkendir.
```

> **Geçersiz Değişken Adları**

```
int 1age = 30; // Hata: Değişken bir sayı ile başlayamaz.
int age@ = 20; // Hata: Özel karakter kullanılamaz.
int function = 10; // Hata: Bu bir fonksiyon adı olarak kullanılamaz.
```

**Çıktı Değişkenleri**

C++ dilinde `std::cout` (console output) ifadesi ekrana veri çıkışı yapmak için kullanılır. Aşağıdaki örnek, metin ve değişkenin çıktısının nasıl alınacağını gösterir:

```
#include <iostream>

int main() {
    std::string txt = "Yavuzlar";
    std::cout << "I love " << txt << "!" << std::endl; // I love Yavuzlar!
    
    return 0;
}
```

