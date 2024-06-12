### Deskripsi HomeWork

Proyek ini bertujuan untuk mengimplementasikan Avro Producer dan Avro Consumer menggunakan dataset Bitcoin Price Training. Dalam proyek ini, kita akan menggunakan Apache Kafka sebagai middleware untuk mentransmisikan data antara Avro Producer dan Avro Consumer.

### Komponen Proyek

1. **Apache Kafka Services**
   - Zookeeper: Layanan manajemen koordinasi yang dibutuhkan oleh Kafka.
   - Broker: Layanan broker Kafka untuk menangani pengiriman pesan antara Avro Producer dan Avro Consumer.
   - Schema Registry: Layanan registri skema Avro untuk memastikan kompatibilitas skema antara Avro Producer dan Avro Consumer.
   - Control Center: Antarmuka pengguna grafis untuk memantau dan mengelola cluster Kafka.

2. **Avro Producer**
   - Avro Producer bertugas untuk membaca dataset Bitcoin Price Training, mengonversinya ke format Avro, dan mengirimkannya ke topik Kafka bernama "bitcoin".

3. **Avro Consumer**
   - Avro Consumer bertugas untuk mengonsumsi pesan dari topik Kafka "bitcoin", membacanya dalam format Avro, dan menampilkannya.

### Struktur Dataset

Dataset Bitcoin Price Training berisi data historis harga Bitcoin dengan kolom-kolom berikut:
- **Date**: Tanggal data
- **Open**: Harga pembukaan pada hari tersebut
- **High**: Harga tertinggi pada hari tersebut
- **Low**: Harga terendah pada hari tersebut
- **Close**: Harga penutupan pada hari tersebut
- **Volume**: Volume perdagangan pada hari tersebut
- **MarketCap**: Kapitalisasi pasar pada hari tersebut

### Implementasi Avro Producer dan Avro Consumer

Avro Producer dan Avro Consumer akan menggunakan skema Avro untuk memastikan kesesuaian struktur data. Skema Avro akan memastikan bahwa pesan yang dikirim oleh Avro Producer dapat dibaca dengan benar oleh Avro Consumer.

### Cara Menjalankan Proyek

1. Pastikan bahwa layanan Apache Kafka sudah berjalan.
2. Jalankan Avro Producer untuk membaca dataset Bitcoin Price Training, mengonversinya ke format Avro, dan mengirimkannya ke topik "bitcoin" pada cluster Kafka.
3. Jalankan Avro Consumer untuk mengonsumsi pesan dari topik "bitcoin" dalam format Avro dan menampilkannya.

### Referensi

- [Apache Kafka Documentation](https://kafka.apache.org/documentation/)
- [Confluent Avro Python Documentation](https://docs.confluent.io/5.0.0/clients/confluent-kafka-python/index.html#avro-producer)
