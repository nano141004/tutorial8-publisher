- How many data your publisher program will send to the message broker in one run? 
Publisher akan mengirimkan 5 pesan kepada broker. Terjadi 5 kali pemanggilan method publish_event, masing - masing mengirim instance UserCreatedEventMessage.
- The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
Berarti mereka menggunakan broker AMPQ yang sama untuk melakukan komunikasi.

![ss1](images/ss1.png)

![ss2](images/ss2.png)
![ss3](images/ss3.png)
Ketika dijalankan cargo run pada publisher, akan dikirimkan 5 event ke message broker, lalu diterima dan diproses oleh subscriber.

![ss4](images/ss4.png)
Dapat dilihat pada RabbitMQ saat dijalankan cargo run dua kali pada publisher maka terjadi pula dua spike. Spike yang terjadi menunjukkan tiap kali publisher dijalankan.