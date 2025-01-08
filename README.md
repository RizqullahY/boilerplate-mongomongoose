# MongoDB and Mongoose Challenges

This is the boilerplate for the MongoDB and Mongoose lessons. Instructions for completing these lessons start at https://www.freecodecamp.org/learn/apis-and-microservices/mongodb-and-mongoose/



Ganti Format URL
Ubah URL koneksi dari:

perl
Salin kode
mongodb://raflymongodb:raflymongodb@raflyasligalek-cluster-shard-00-00.jcsnu.mongodb.net:27017,...
Menjadi:

ruby
Salin kode
mongodb+srv://raflymongodb:raflymongodb@raflyasligalek-cluster.jcsnu.mongodb.net/?retryWrites=true&w=majority
Format mongodb+srv:// menggunakan DNS Seed List yang lebih sederhana dan otomatis menangani koneksi ke replika set.


update mongodb

mongoose.connect(process.env.MONGO_URI, { useNewUrlParser: true, useUnifiedTopology: true })
hapus { useNewUrlParser: true, useUnifiedTopology: true } karna nggka perlu??