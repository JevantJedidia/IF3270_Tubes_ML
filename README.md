# IF3270_Tubes_ML

### Program
Pada program model FFNN blok 1, terdapat fungsi-fungsi aktivasi yang diperlukan yaitu linear, reLU, sigmoid, dan softmax. Setiap fungsi aktivasi ini akan menerima parameter berupa nilai net dan mengembalikan output yang dihitung berdasarkan fungsi aktivasi tersebut. Pada blok ini juga didefinisikan fungsi CountSSE untuk menghitung error dari ekspektasi output.

Pada program model FFNN blok 2, dilakukan pembacaan file model FFNN dalam format .json yang akan dibangun. Kemudian, model tersebut akan dituangkan ke dalam variabel-variabel yang diperlukan untuk melakukan Forward Propagation. Variabel-variabel ini berupa inp, activation, neuron, weight, eoutput, dan sse. Setelah itu, pengguna akan memasukkan input berupa jumlah instance dan nilai dari setiap instance tersebut, kemudian dimasukkan pada variabel inp bertipe array 2D untuk diproses selanjutnya.

Pada program model FFNN blok 3, dilakukan Forward Propagation pada input instance yang telah dilakukan. Untuk setiap layer, akan dihitung nilai net pada setiap neuron dari layer tersebut. Nilai net ini dihitung berdasarkan fungsi aktivasi yang dimasukkan pada layer tersebut. Proses ini dilakukan hingga didapatkan output untuk model FFNN yang telah diinput. Di akhir, dilakukan klasifikasi untuk menentukan kelas dari output tersebut.

Pada program model FFNN blok 4, dilakukan penggambaran model FFNN yang telah diinput. Yang ditampilkan adalah ANN dalam bentuk compact, bobot dari sebuah neuron ke neuron lainnya, serta fungsi aktivasi dari sebuah neuron ke neuron lainnya. Fungsi aktivasi dari sebuah neuron ke neuron lainnya ditulis dalam format layerX -> layerY = fungsiAktivasi sedangkan bobot dituliskan dalam format neuronX -> neuronY = bobot. Sebuah neuron dituliskan dalam format layer(neuron) sehingga untuk neuron pertama dari hidden layer pertama, formatnya adalah h1(1).

Pada program model FFNN blok 5, dibuat sebuah visualisasi model FFNN berbentuk graph apabila model yang dibuat pada blok 5 kurang jelas. Arah dari graph adalah dari atas ke bawah.
