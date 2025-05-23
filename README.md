# Tutorial Module 9
### Nama : Ischika Afrilla
### NPM : 2306227955

7a. How much data your publisher program will send to the message broker in one run? 

    Publisher akan mengirimkan 5 data ke message broker dalam satu kali run karena terdapat 5 data user_created pada main.

7b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

    URL "amqp://guest:guest@localhost:5672" yang sama dipakai di subscriber berarti publisher dan subscriber terhubung ke server RabbitMQ yang sama, yaitu: di komputer lokal (karena localhost), menggunakan username = 'guest' dan password = 'guest', melalui port 5672 (port standar amqp). Artinya, publisher (pengirim pesan) dan subscriber (penerima pesan) berkomunikasi melalui broker yang sama.

### Commit Running RabbitMQ as message broker.
![Running RabbitMQ as message broker.](images/Screenshot%202025-05-06%20015107.png)

### Commit Sending and processing event.
![Sending and processing event.](images/Screenshot%202025-05-06%20015639.png)

![Sending and processing event.](images/Screenshot%202025-05-06%20015730.png)

Pada kedua gambar di atas, publisher mengirimkan 5 event ke message broker. Event-event tersebut kemudian diproses oleh subscriber. Akibatnya, di RabbitMQ akan terlihat penambahan pada bagian connections, channels, queues, dan consumers, sesuai dengan aktivitas pengiriman dan penerimaan pesan.

### Commit Monitoring chart based on publisher.
![Monitoring chart based on publisher](images/Screenshot%202025-05-06%20020342.png)

Lonjakan message rates terjadi ketika publisher sering mengirim pesan ke message broker. Tingginya message rate menunjukkan bahwa broker menerima banyak pesan dalam waktu singkat. 