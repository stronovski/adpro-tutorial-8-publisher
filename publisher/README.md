## Reflection for Publisher

### How many data your publisher program will send to the message broker in one run?
Karena p.publish_event dipanggil sebanyak 5 kali, maka terdapat 5 data yang dikirimkan dalam satu waktu

### The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
Kedua URL tersebut digunakan untuk mengkoneksikan ke broker AMQP dengan menggunakan kredensial dan detail connection yang sama. Dengan hal tersebut, message yang dipublish oleh publisher dapat digunakan oleh subscriber dengan menggunakan broker instance yang sama