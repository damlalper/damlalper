# JSON'dan CSV'ye Dönüştürme Programı

Bu C programı, JSON dosyasındaki verileri okuyarak bu verileri CSV dosyasına dönüştürmek için kullanılır.

## Kullanım


Programı çalıştırmak için terminal veya komut istemcisinde komutu şu şekilde kullanacağız:

$ ./programadı <JSON dosya adı> <CSV dosya adı> <header=ON|OFF>


<JSON dosya adı>: Dönüştürmek istediğimiz JSON dosyası </br>
<CSV dosya adı>: Dönüştürülen verilerin kaydedileceği CSV dosyası </br>
<header=ON|OFF>: ON kullanarak başlıkları yazarız, kullanmak istemiyorsak OFF. </br> 


## *Örneğin* 

 
$ ./Odev1.c test.json cikti.csv header=ON 


Bu komut, 'test.json' adlı JSON dosyasını okuyarak verileri 'cikti.csv' adlı CSV dosyasına dönüştürecek ve başlığı CSV dosyasına ekleyecektir.

## Programın Çalışma Mantığı
Program, JSON dosyasındaki verileri okuyarak öğrenci bilgilerini içeren bir yapı oluşturur. JSON dosyasındaki öğrenci verileri şu şekilde:
```
[
    {
        "id": 1, 
        "name": "Ahmet Yilmaz", 
        "grades": { 
            "midterm": 75, 
            "final": 85 
        }, 
        "course": "BIL 203" 
    },
    {
        "id": 2,
        "name": "Ayse Kaya",
        "grades": {
            "midterm": 80,
            "final": 88
        },
        "course": "BIL 203" 
    },
    {
        "id": 3,
        "name": "Mehmet Demir",
        "grades": {
            "midterm": 70,
            "final": 82
        },
        "course": "BIL 203"
    }
]
```

Program, JSON dosyasını okuyarak öğrenci bilgilerini alır, bunları bir CSV dosyasına dönüştürür ve isteğe bağlı olarak başlığı ekler.

## Geliştirme ve Katkı
Eğer bu projeye katkıda bulunmak isterseniz pull request açınız. 
