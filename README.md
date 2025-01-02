# Tubes-Big-Data
## Pendahuluan
Data dalam masa modern ini sangat melimpah, pengambilan keputusan berdasarkan data sudah menjadi kebutuhan penting. Tetapi data-data itu sering kali tidak terstruktur dan sulit untuk dipahami. Dalam proyek ini kami melakukan analisis pada dataset yang terhitung besar untuk memberikan hasil dari analisis kami.  
Rencana kami dalam mengatasi masalah ini :  
 1. **Dataset:** kami menggunakan dataset  yang berisi data tentang
 2. **Metode:**
    - **Eksplorasi Data**
    - **Pra-pemrosesan**
    - **Analisis Statistik dan Visualisasi**
    - **Model**
## Package yang diperlukan
Ini adalah list package yang di perlukan untuk menjalankan codenya :  
- pandas
- numpy
- seaborn
- plotly.express
- matplotlib.pyplot
![Screenshot 2025-01-02 113949](https://github.com/user-attachments/assets/f2d6a47d-6d3b-4131-8af8-ab535b458b6d)
## Data Preparation
Dataset yang digunakan dalam project ini kami ambil dari [Spotify Genre Data](https://www.dropbox.com/sh/qj0ueimxot3ltbf/AACzMOHv7sZCJsj3ErjtOG7ya?raw=1). Dataset ini memiliki  23 variabel dengan ribuan baris data yang mencakup track_id, track_name, track_artist, track_popularity, dan sebagainya  
## Pre-processing
1. Import data menggunakan pandas
   ```python
   df = pd.read_csv("spotify_songs.csv")
3. Mengatasi Missing Values
   - Cek nilai null
     ```python
     pd.DataFrame({'count': df.shape[0],
              'nulls': df.isnull().sum(),
              'nulls%': df.isnull().mean() * 100
             })
    - Hapus data yang memiliki nilai null
      ```python
      df = df.dropna()
5. Cek Data Duplikat
   ```python
   print(f"Terdapat {df.duplicated().sum()} duplikasi.")
## Eksplorasi dan Analisis Data
### Eksplorasi Data
1. Gambaran Umum Dataset
2. Visualisasi Data
3. Analisis Statistik Deskriptif
### Analisis Data
1. **Analisis Popularitas Genre dan Subgenre**
2. **Analisis Lagu-lagu Terpopuler Beradsarkan Artis**
3. **Analisis Subgenre Terpopuler berdasarkan Genre**
4. **Analisis Distribusi Lagu Terpopuler berdasarkan Tahun Rilis**
5. **Analisis Tren Popularitas Selama Bertahun-tahun**
## Rangkuman
