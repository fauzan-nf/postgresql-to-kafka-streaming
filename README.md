# PostgreSQL to Kafka Streaming Pipeline

Tugas praktik Data Engineering: membaca data dari PostgreSQL dan mengirimkannya ke Apache Kafka menggunakan Python.

## Teknologi
- Python 3.11
- PostgreSQL 13
- Apache Kafka 7.5.0 (Confluent)
- psycopg2, kafka-python

## Cara Menjalankan
1. `docker compose up -d postgres zookeeper kafka jupyter`
2. Buat tabel `crypto_price` di database `streaming_db`.
3. Buka `Nurfaudzan_PostgreSQL_to_Kafka.ipynb`, jalankan cell 1–5.

## Struktur
- Cell 1: instalasi `kafka-python`
- Cell 2: import library
- Cell 3: koneksi PostgreSQL
- Cell 4: kirim pesan uji ke Kafka
- Cell 5: streaming loop (`while True`, polling tiap 3 detik)
- Cell 6: kosong (sesuai referensi)