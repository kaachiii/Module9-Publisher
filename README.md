# Tutorial Module 9
### Nama : Ischika Afrilla
### NPM : 2306227955

7a. How much data your publisher program will send to the message broker in one run? 

    Publisher akan mengirimkan 5 data ke message broker dalam satu kali run karena terdapat 5 data user_created pada main.

7b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

    URL "amqp://guest:guest@localhost:5672" yang sama dipakai di subscriber berarti publisher dan subscriber terhubung ke server RabbitMQ yang sama, yaitu: di komputer lokal (karena localhost), menggunakan username = 'guest' dan password = 'guest', melalui port 5672 (port standar amqp). Artinya, publisher (pengirim pesan) dan subscriber (penerima pesan) berkomunikasi melalui broker yang sama.

[Running RabbitMQ as message broker.](images/Screenshot%202025-05-06%20015107.png)