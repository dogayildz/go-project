Go PostgreSQL Projesi

Bu proje, Go programlama dili kullanılarak PostgreSQL veritabanı ile entegre çalışan  bir API sunmaktadır.

Başlangıç

Bu talimatlar, projeyi yerel makinenizde çalıştırmak ve geliştirmek için bir kopyasını almanıza yardımcı olacaktır.

Gereksinimler

Bu projenin çalışması için aşağıdaki gereksinimlere ihtiyacınız vardır:

- Go (versiyon 1.16 veya üstü)
- PostgreSQL
- Postman (isteği test etmek için isteğe bağlı)

Kurulum

1. Bu depoyu yerel makinenize klonlayın:

git clone https://github.com/kullanici/go-postgresql-proje.git

2. Proje dizinine gidin:

cd go-postgresql-proje

3. PostgreSQL veritabanını oluşturun:

# Örneğin, psql komutunu kullanarak
psql -U postgres -c "CREATE DATABASE go_projesi"

4. Proje bağımlılıklarını yükleyin:

go mod tidy

5. Projeyi çalıştırın:

go run main.go

API şimdi http://localhost:8080 adresinde çalışmaya başlamalıdır.

Kullanım

API'yi test etmek için Postman veya cURL gibi bir araç kullanarak istekler yapabilirsiniz.

- Kullanıcı eklemek için:
  - Method: POST
  - Endpoint: http://localhost:8080/kullanici
  - Body: JSON formatında kullanıcı verileri

- Kullanıcı detaylarını getirmek için:
  - Method: GET
  - Endpoint: http://localhost:8080/kullanici/{id} (ID'yi belirtin)



Lisans

Bu proje MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakın.
