# ViT_Vision-Transformer-and-EANet_External-Attention-Transformer

<p align="center">
 <img src="https://github.com/sultanbst123/ViT_Vision-Transformer-and-EANet_External-Attention-Transformer/blob/main/source.gif"><i></i>
</p>

## Vision Transformer(ViT)

<p align="center">
 <img src="https://github.com/sultanbst123/ViT_Vision-Transformer-and-EANet_External-Attention-Transformer/blob/main/images.png"><i>Vision Transformer Architecture</i>
</p>

Vision Transformer(ViT) adalah model untuk klasifikasi citra(image classification) yang mempekerjakan Transformer arsitektur. Gambar dipecah menjadi tambalan berukuran tetap, masing-masing kemudian disematkan secara linier, penyematan posisi ditambahkan, dan urutan vektor yang dihasilkan diumpankan ke enkoder Transformer standar, Untuk melakukan klasifikasi.

untuk lebih lanjut silahkan liat paper. 

Paper: <p><a href="https://arxiv.org/pdf/2010.11929"> An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale</a> [Dosovitskiy et al.]</p>


## External Attention Transformer(EANet) 

Model EANet hanya mengganti Self-Attention, perbedaan antara [0]Self-Attention dan [1]External-Attention adalah  [1]Perhatian eksternal(External Attention) memiliki kompleksitas linier dan secara implisit mempertimbangkan korelasi antara semua sampel data sementara  
[0]Self-Attention memiliki kompleksitas kuadrat dan mengabaikan potensi korelasi antara sampel yang berbeda.

untuk lebih lanjut silahkan liat paper. 

Paper: <p><a href="https://arxiv.org/pdf/2105.02358"> Beyond Self-attention: External Attention using Two Linear Layers for Visual Tasks</a></p>

## Laporan
Setelah berlatih dengan 10 epoch dan adabelief optimizer dengan Triangular2CyclicalLearningRate

validation_accuracy = 76%
validation_top5_accuracy = 98%
test_accuracy = 70%

### Note
kalian bisa ber-eksperimen sendiri seperti: 

- menambahkan epoch lebih banyak
- menambahkan layers transformers
- mengubah ukuran gambar(224 recommend)
- mengubah ukuran tambalan(patches)
- mengunakan CutMix & MixUp Augmentation 

## Referensi 

- <p><a href="https://ai.googleblog.com/2020/12/transformers-for-image-recognition-at.html?m=1">Transformers for Image Recognition at Scale</a></p>
- Google 

