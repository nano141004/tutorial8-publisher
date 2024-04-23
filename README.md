- How many data your publlsher program will send to the message broker in one run? 
    Publisher akan mengirimkan 5 pesan kepada broker. Terjadi 5 kali pemanggilan method publish_event, masing - masing mengirim instance UserCreatedEventMessage.
- The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
    Berarti mereka menggunakan broker AMPQ yang sama untuk melakukan komunikasi.