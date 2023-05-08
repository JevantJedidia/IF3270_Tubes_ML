# IF3270_Tubes_ML

### Program
Pada program model Mini-batch Gradient Descent blok 1, dilakukan import library yang dibutuhkan. Selain itu, dilakukan juga pengambilan dataset iris yang kemudian dipisah menjadi data dan target.

Pada program model Mini-batch Gradient Descent blok 2, terdapat fungsi-fungsi aktivasi yang diperlukan yaitu linear, reLU, sigmoid, dan softmax yang diperlukan untuk melakukan FFNN terhadap input. Setiap fungsi aktivasi ini akan menerima parameter berupa nilai net dan mengembalikan output yang dihitung berdasarkan fungsi aktivasi tersebut. Pada blok ini juga didefinisikan fungsi derive dan deriveSoftmax untuk memberikan hasil turunan berdasarkan jenis aktivasi yang diterima. Selain itu, diberikan fungsi loss untuk menghitung error dari model FFNN.

Pada program model Mini-batch Gradient Descent blok 3, disediakan kelas ANN dengan berbagai method sebagai berikut.

<table>
    <tr>
        <th>
            Method
        </th>
        <th>
            Fungsi
        </th>
    </tr>
    <tr>
        <td>
            readInput(self, activation, layer, neuron_each_layer, inp, weight, target, learning_rate, batch_size, max_iter, error_threshold)
        </td>
        <td>
            Membaca seluruh atribut yang diperlukan dari input pengguna
        </td>
    </tr>
    <tr>
        <td>
            readFile(self, file)
        </td>
        <td>
            Membaca seluruh atribut yang diperlukan dari sebuah file
        </td>
    </tr>
    <tr>
        <td>
            generateWeight(self)
        </td>
        <td>
            Inisialisasi bobot awal secara random
        </td>
    </tr>
    <tr>
        <td>
            forwardProp(self, inp)
        </td>
        <td>
            Melakukan FFNN terhadap input berdasarkan batch size yang diberikan
        </td>
    </tr>
    <tr>
        <td>
            gradient(self, index, level, j, k, is_leaf)
        </td>
        <td>
            Menghitung nilai gradien dari bobot yang diberikan
        </td>
    </tr>
    <tr>
        <td>
            backwardProp(self, start, end, count)
        </td>
        <td>
            Melakukan Backward Propagation terhadap input berdasarkan batch size dan learning rate yang diberikan
        </td>
    </tr>
    <tr>
        <td>
            mini_batch(self)
        </td>
        <td>
            Melakukan Mini Batch Gradient Descent terhadap seluruh input berdasarkan batch size, max iteration, dan error threshold yang diberikan
        </td>
    </tr>
    <tr>
        <td>
            saveModel(self, file_name)
        </td>
        <td>
            Melakukan save terhadap model yang sudah dibangun
        </td>
    </tr>
</table>

Program model Mini-batch Gradient Descent blok 4 merupakan blok yang berisi program pertama untuk melakukan Mini-batch Gradient Descent. Pada blok ini, diberikan variabel file yang berisi nama file model yang akan dibaca. Program kemudian melakukan Mini-batch Gradient Descent terhadap file tersebut dan menyimpan modelnya dalam sebuah folder output.

Pada program model Mini-batch Gradient Descent blok 5, dilakukan pembangunan model Mini-batch Gradient Descent dari dataset iris yang telah dipisah. Kemudian, model ini disimpan dalam sebuah file untuk dilakukan uji coba dengan model FFNN.

Pada program model Mini-batch Gradient Descent blok 6, dilakukan pengujian hasil model Mini-batch Gradient Descent dari dataset iris dengan menggunakan file model yang sudah disimpan. Pengujian ini dilakukan dengan menggunakan fungsi model FFNN yang sudah diimplementasikan pada bagian sebelumnya.

Pada program model Mini-batch Gradient Descent blok 7, dilakukan visualisasi terhadap model dataset iris yang telah dibuat.