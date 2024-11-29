MUCA : Merupakan Group chat yang memungkin client/user untuk berdiskusi dalam satu server dengan bantuain chatbot ai.

Arsitektur : Event-Driven
Model komunikasi : Publish-Subscribe
Chatgroup yang terdiri atas: server, client, chatbot ai

Memungkinkan skenario seperti berikut berjalan:

PC A yang menjalankan server
PC B yang menjalankan client 1
PC C yang menjalankan client 2

1. Ketika client 1 di PC B memulai diskusi dengan bot AI dengan mengirimkan perintah /start_discussion, server akan memproses perintah tersebut dan memulai sesi diskusi baru. Server akan menyiarkan respons bot ke semua client yang terhubung, termasuk client 2 di PC C.
2. Dengan demikian, client 2 di PC C juga akan menerima respons bot terkait diskusi yang dimulai oleh client 1. Selanjutnya, client 2 dapat mengirimkan pesan ke bot AI menggunakan perintah /respond [message], dan server akan meneruskan pesan tersebut ke bot AI.
3. Bot AI akan memproses pesan dari client 2 dan mengirimkan respons kembali ke server. Server kemudian akan menyiarkan respons bot tersebut ke semua client yang terhubung, termasuk client 1 dan client 2.
4. Jadi, client 2 yang berada di PC C dapat bergabung dan berpartisipasi dalam diskusi yang dimulai oleh client 1 di PC B, dengan mengirimkan pesan-pesan ke bot AI melalui server.
Inti dari kemampuan ini adalah arsitektur server-client yang memungkinkan server untuk menyiarkan pesan-pesan dari bot AI ke semua client yang terhubung, sehingga mereka dapat saling berinteraksi meskipun berada di PC yang berbeda.
