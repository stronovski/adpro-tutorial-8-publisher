## Reflection for Publisher

### 1. How many data your publisher program will send to the message broker in one run?
Karena p.publish_event dipanggil sebanyak 5 kali, maka terdapat 5 data yang dikirimkan dalam satu waktu

### 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
Kedua URL tersebut digunakan untuk mengkoneksikan ke broker AMQP dengan menggunakan kredensial dan detail connection yang sama. Dengan hal tersebut, message yang dipublish oleh publisher dapat digunakan oleh subscriber dengan menggunakan broker instance yang sama

### 3. Put the screen of your running RabbitMQ here
![alt text](image.png)

### 4. Try to capture your screen showing these console and put some sentences describing what was happening
![alt text](image-2.png)
Ketika 'cargo run' dijalankan di publisher, publisher akan mengirimkan data-data ke dalam message queue. Setelah itu, event akan diproses di dalam subscriber sehingga akan menampilkan pesan berikut di dalam console subscriber:
![alt text](image-1.png)

### 5. Capture your browser, and explain how the spike got to do with running the publisher.
![alt text](image-3.png)
Jika terjadi peningkatan message dalam suatu interval waktu, maka peningkatan tersebut akan terlihat di dalam grafik kedua seperti gambar di atas.  Setiap kali publisher dijalankan dengan menggunakan cargo run, maka message rate dalam RabbitMQ akan terlihat meningkat yang mana menunjukkan message queue dari program tersebut. 

