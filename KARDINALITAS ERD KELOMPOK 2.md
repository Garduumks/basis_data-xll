
### 1. **Relasi antara `siswa` dan `event sekolah` melalui relasi `mengikuti` (Many-to-Many)**
   - **Penjelasan:** 
     Relasi ini menunjukkan bahwa seorang siswa dapat mengikuti banyak event sekolah, dan satu event sekolah dapat diikuti oleh banyak siswa. Oleh karena itu, relasinya bersifat banyak ke banyak (N:N).
   - **Kardinalitas:** 
     - Satu siswa dapat mengikuti lebih dari satu event.
     - Satu event dapat memiliki banyak siswa yang mengikutinya.

### 2. **Relasi antara `guru` dan `event sekolah` melalui relasi `mengawasi` (One-to-Many)**
   - **Penjelasan:** 
     Relasi ini menunjukkan bahwa satu guru dapat mengawasi banyak event sekolah, tetapi satu event sekolah hanya diawasi oleh satu guru. Oleh karena itu, relasinya bersifat satu ke banyak (1:N).
   - **Kardinalitas:**
     - Satu guru dapat ditugaskan untuk mengawasi lebih dari satu event.
     - Satu event sekolah hanya diawasi oleh satu guru.

### 3. **Relasi antara `event sekolah` dan `pendaftaran` melalui relasi `minat` (One-to-Many)**
   - **Penjelasan:** 
     Relasi ini menunjukkan bahwa satu event sekolah dapat memiliki banyak pendaftaran, tetapi satu pendaftaran hanya terkait dengan satu event tertentu. Oleh karena itu, relasinya bersifat satu ke banyak (1:N).
   - **Kardinalitas:** 
     - Satu event sekolah dapat memiliki banyak pendaftar.
     - Satu pendaftaran hanya terkait dengan satu event sekolah.

### 4. **Entitas `pendaftaran` dan atribut terkaitnya**
   - **Penjelasan:** 
     Entitas ini memuat detail dari siswa yang mendaftar ke event tertentu. Atribut seperti `NIS`, `nama_lengkap`, `kelas`, dan `lomba` digunakan untuk menyimpan informasi spesifik terkait pendaftaran siswa.

---

#### **Alasan Kardinalitas:
- **1:1** digunakan jika hanya satu entitas dihubungkan dengan satu entitas lainnya tanpa pengulangan.
- **1:N** digunakan jika satu entitas dapat dihubungkan dengan banyak entitas lainnya (misalnya, satu guru mengawasi banyak event).
- **N:N** digunakan jika kedua entitas dapat berhubungan secara banyak ke banyak (misalnya, siswa mengikuti banyak event, dan event dapat diikuti banyak siswa).
