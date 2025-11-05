# Warehouse Sales Forecast

Project ini bertujuan untuk memprediksi penjualan bulanan dari data warehouse dan retail.  
Model ini menggunakan pendekatan regresi sederhana seperti Lasso, Ridge, Random Forest, dan Gradient Boosting.

## Dataset
Data diambil dari file `Warehouse_and_Retail_Sales.csv` yang berisi informasi tahunan dan bulanan tentang:
- Retail Sales  
- Warehouse Sales  
- Retail Transfers  

Kolom tersebut digabungkan menjadi satu metrik total (`TOTAL_SALES`) untuk dilakukan analisis dan prediksi.

## Langkah Utama
1. Data preprocessing (penggabungan kolom & konversi tanggal)
2. Exploratory Data Analysis (EDA) untuk melihat tren
3. Pembuatan fitur lag dan rolling window
4. Training model regresi
5. Evaluasi hasil (MAE, RMSE, R²)
6. Visualisasi hasil prediksi vs data aktual

## Hasil
Model Lasso Regression memberikan performa terbaik dengan:
- MAE: ±12.411
- R²: 0.868

## Visualisasi
Contoh hasil prediksi:
![Forecast Result](images/forecast_plot.png)

## Cara Menjalankan
```bash
pip install -r requirements.txt
jupyter notebook notebooks/Fixed_Forecast.ipynb
