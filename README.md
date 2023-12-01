# Tugas Kuliah: Form Biodata dengan Java JFrame dan MySQL

Selamat datang di tugas kuliah ini! Tugas ini bertujuan untuk membuat formulir biodata menggunakan Java JFrame yang terhubung ke MySQL. Berikut adalah langkah-langkah implementasinya.

## Deskripsi Tugas

Tugas ini mengharuskan Anda membuat sebuah formulir biodata menggunakan Java JFrame. Formulir tersebut akan terhubung ke database MySQL, yang telah disediakan struktur dan contoh datanya.

## Struktur Database MySQL

Dalam tugas ini, kami telah menyiapkan struktur database MySQL sebagai berikut:

```sql
-- Struktur Database
CREATE DATABASE IF NOT EXISTS `biodata` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci */ /*!80016 DEFAULT ENCRYPTION='N' */;
USE `biodata`;

-- Struktur Tabel
CREATE TABLE IF NOT EXISTS `biodata` (
  `id` varchar(255) NOT NULL,
  `nama` varchar(255) NOT NULL,
  `no_telepon` varchar(255) NOT NULL,
  `jenis_kelamin` varchar(255) NOT NULL,
  `alamat` varchar(255) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

-- Contoh Data
REPLACE INTO `biodata` (`id`, `nama`, `no_telepon`, `jenis_kelamin`, `alamat`) VALUES
	('d410ea22-1ff2-4e90-b923-1b59693c73c0', 'asdasdas', 'asdasd', 'Laki-Laki', 'asdasda'),
	('ee26a079-e721-4c34-9861-020dc506febb', 'aasdasdas', 'dasdasd', 'Laki-Laki', 'sdaasdasd');

```

Implementasi Form Biodata
Berikut adalah contoh implementasi sederhana menggunakan Java JFrame:

```java

java
Copy code
import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.SQLException;

public class BiodataForm extends JFrame {
    // ... (Isi dengan komponen-komponen yang diperlukan)
}
