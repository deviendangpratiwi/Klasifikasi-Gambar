# Proyek Klasifikasi Gambar - CNN

Proyek ini adalah tugas akhir untuk membuat model klasifikasi gambar menggunakan Convolutional Neural Network (CNN) di TensorFlow.

## Deskripsi Proyek
Model CNN dibuat untuk mengklasifikasikan gambar arah pandangan wajah ke dalam 4 kelas:
- close look
- forward look
- right look
- left look

Dataset yang digunakan terdiri dari lebih dari 10000 gambar, dan dibagi menjadi:
- training set
- validation set
- testing set

## Arsitektur Model
Model dibangun dengan:
- Sequential model dari Keras
- Beberapa Conv2D dan MaxPooling2D
- Flatten dan Dense layer
- Optimizer: Adam
- Loss: Categorical Crossentropy

## Hasil Training
- Akurasi training dan testing lebih dari 95%
- Tidak overfitting
- Plot akurasi dan loss tersedia di notebook

## Format Model
Model disimpan dalam 3 format:
- SavedModel (`cnn_saved_model/`)
- TF-Lite (`cnn_model_lite.tflite`)
- TFJS (`model_tfjs/`)

## Inference
Model diuji dengan gambar baru, dan berhasil melakukan prediksi. Hasil dan gambar prediksi ditampilkan di notebook.

## Catatan Tambahan
- Sudah menggunakan callback (EarlyStopping & ModelCheckpoint)
- Dataset sudah dibagi dengan baik (train, test, valid)