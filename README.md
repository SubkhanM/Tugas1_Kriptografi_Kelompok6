# Tugas1_Kriptografi_Kelompok6
Anggota :
| Nama      | NRP        |
|-----------|-----------|
| Subkhan Masudi  | 5027221044 |

## 1. Kriptanalisis Cipher Abjad-Tunggal
Di laboratorium KCKS, Cyber Fox yang penasaran, sedang menyelidiki sebuah anomali dalam sistem jaringan DTI. Saat menelusuri log, Cipher menemukan sebuah dokumen terenkripsi yang mencurigakan. Namun, ada satu masalah: teks dalam dokumen tersebut telah dikodekan menggunakan cipher substitusi abjad-tunggal (monoalphabetic cipher), dan kunci enkripsinya tidak diketahui. Untungnya, Cipher adalah ahli dalam kriptanalisis dan tahu bahwa metode ini bisa dipecahkan menggunakan analisis frekuensi dan terkaan kata. Jika diketahui bahwa bahasa yang digunakan dalam teks adalah bahasa inggris, bantulah Cyber Fox membuat tabel substitusi huruf dan mendekripsi teks sebelum waktunya habis! 

```
LAHYCXPAJYQHRBJWRWMRBYNWBJKUNCXXUOXAYAXCNLCRWPRWOXAVJCRXWRWLXV
YDCRWPBHBCNVBRCRBDBNMNENAHFQNANKHKRUURXWBXOYNXYUNFXAUMFRMNXWJM
JRUHKJBRBBNLDARWPKXCQMJCJJCANBCJWMMJCJRWVXCRXWLAHYCXPAJYQRLBHB
CNVBJANODWMJVNWCJUCXBCJWMJAMYAXCXLXUBVXBCWXCJKUHCQNCAJWBYXACUJ
HNABNLDARCHCUBYAXCXLXUFQRLQNWJKUNBBCAXWPNWLAHYCRXWJLAXBBJFRMNA
JWPNXOJYYURLJCRXWBMNBYRCNRCBRVYXACJWLNLAHYCXPAJYQHRBRWQNANWCUH
OAJPRUNNENWCQNVXBCBNLDANLAHYCXPAJYQRLBHBCNVLJWKNANWMNANMLXVYUN
CNUHRWBNLDANKHJBRWPUNBYNLRORLJCRXWOUJFXAYAXPAJVVRWPNAAXACAJMRC
RXWJUBXOCFJANCNBCRWPVNCQXMBBDLQJBDWRCCNBCRWPJANRWBDOORLRNWCCXD
WLXENABNLDARCHEDUWNAJKRURCRNBRWLAHYCXBHBCNVBRWBCNJMLAHYCXPAJYQ
RLBNLDARCHRBNBCJKURBQNMCQAXDPQVJCQNVJCRLJUVXMNURWPJWMARPXAXDBY
AXXOBMNVXWBCAJCRWPCQJCJBHBCNVVNNCBCQNWNLNBBJAHBNLDARCHYAXYNACR
NBCQNBNJAPDVNWCBXOCNWANUHXWYUJDBRKUNJBBDVYCRXWBCXEJURMJCNCQNRA
LUJRVBXWNXOCQNNJAURNBCJWMBRVYUNBCLAHYCXPAJYQRLCNLQWRZDNBRBCQNL
JNBJALRYQNAFQRLQMJCNBKJLTCXJAXDWMKLCQRBVNCQXMNWLXMNBYUJRWCNGCK
HBQROCRWPNJLQUNCCNAXOCQNJUYQJKNCKHJORGNMWDVKNAXOYXBRCRXWBFQRUN
CQRBJYYAXJLQFJBNOONLCRENJCCQNCRVNMDNCXCQNXKBLDARCHXOCQNVNCQXMR
CYAXERMNBWXANJUBNLDARCHCXMJHBRWLNCQNANJANXWUHYXBBRKUNBQROCBCQN
LRYQNALJWKNNJBRUHKAXTNWCQAXDPQKADCNOXALNMNBYRCNRCBBRVYURLRCHCQ
NLJNBJALRYQNAANVJRWBXWNXOCQNVXBCFRMNUHANLXPWRINMNWLAHYCRXWCNLQ
WRZDNBQXFNENARCXOONABWXANJUYAXCNLCRXWJBRCLJWKNZDRLTUHMNLRYQNAN
MKHQJWMJMMRCRXWJUUHRCBLRYQNACNGCRBNJBRUHRMNWCRORJKUNKNLJDBNCQN
OANZDNWLHMRBCARKDCRXWXOUNCCNABVRAAXABCQJCXOCQNNWPURBQUJWPDJPNC
QRBQRPQURPQCBJTNHYARWLRYUNRWVXMNAWLAHYCXPAJYQHCADNBNLDARCHANUR
NBWXCXWUHXWBNLANLHKDCJUBXXWBCAXWPVJCQNVJCRLJUOXDWMJCRXWBJWMLXV
YDCJCRXWJURWONJBRKRURCH
```

## 1.1 Tabel Frekuensi Kemunculan Huruf dalam Bahasa Inggris

| Huruf | Frekuensi (%) |
|-------|---------------|
| E     | 12.70         |
| T     | 9.06          |
| A     | 8.17          |
| O     | 7.51          |
| I     | 6.97          |
| N     | 6.75          |
| S     | 6.33          |
| H     | 6.09          |
| R     | 5.99          |
| D     | 4.25          |
| L     | 4.03          |
| C     | 2.78          |
| U     | 2.76          |
| M     | 2.41          |
| F     | 2.23          |
| Y     | 2.02          |
| P     | 1.93          |
| B     | 1.49          |
| V     | 0.98          |
| K     | 0.77          |
| X     | 0.15          |
| Q     | 0.10          |
| J     | 0.10          |
| Z     | 0.07          |

data tersebut didapatkan dari https://en.wikipedia.org/wiki/Letter_frequency

## 1.2 Tabel Frekuensi Kemunculan Huruf dalam Cipherteks
| Huruf | Frekuensi (%) |
|-------|---------------|
| N     | 11.38         |
| C     | 9.85          |
| R     | 8.84          |
| B     | 7.63          |
| X     | 7.06          |
| A     | 6.93          |
| J     | 6.87          |
| W     | 6.17          |
| L     | 4.64          |
| Q     | 4.20          |
| U     | 3.88          |
| Y     | 3.56          |
| H     | 3.24          |
| M     | 2.92          |
| D     | 2.48          |
| V     | 2.35          |
| P     | 2.03          |
| O     | 2.03          |
| K     | 1.91          |
| F     | 0.76          |
| E     | 0.51          |
| Z     | 0.25          |
| T     | 0.25          |
| G     | 0.19          |
| I     | 0.06          |

![image](https://github.com/user-attachments/assets/9a3e4b50-4c67-417c-9b57-b13131bbbecc)

# lalu kita coba untuk substitusikan hasil dari frekuensi kemunculan huruf dalam bahasa inggris, dan juga frekuensi kemunculan huruf dalam chiperteks. kita bisa menggunakan kode python dibawah:
![image](https://github.com/user-attachments/assets/0598d47d-e195-4b4a-a228-65a3fb0769f8)



# hasil ditemukan pada pergeseran (shift) 9, menggunakan kode Python yang dapat digunakan untuk mendekripsi ciphertext dengan shift 9:
![A](https://github.com/user-attachments/assets/9277e5d7-eeaf-4534-b2fa-d2d90c787608)


# Penjelasan Kode
**Fungsi caesar_decrypt:**
- Fungsi ini menerima ciphertext dan shift sebagai parameter.
- Untuk setiap karakter dalam ciphertext, jika karakter tersebut adalah huruf, maka karakter tersebut akan digeser mundur sebanyak shift posisi.
- Jika karakter adalah huruf kecil, digunakan rumus chr((ord(char) - shift_amount - 97) % 26 + 97).
- Jika karakter adalah huruf besar, digunakan rumus chr((ord(char) - shift_amount - 65) % 26 + 65).
- Jika karakter bukan huruf, karakter tersebut ditambahkan ke hasil tanpa perubahan.

**Fungsi caesar_decrypt dipanggil dengan shift 9.**
- Hasil dekripsi dicetak.

**Jika Anda menjalankan kode di atas, hasil dekripsi akan menjadi:**
```
CRYPTOGRAPHY IS AN INDISPENSABLE TOOL FOR PROTECTING INFORMATION IN COMPUTING SYSTEMS IT IS USED EVERYWHERE BY BILLIONS OF PEOPLE WORLDWIDE ON A DAILY BASIS SECURING BOTH DATA AT REST AND DATA IN MOTION CRYPTOGRAPHIC SYSTEMS ARE FUNDAMENTAL TO STANDARD PROTOCOLS MOST NOTABLY THE TRANSPORT LAYER SECURITY TLS PROTOCOL WHICH ENABLES STRONG ENCRYPTION ACROSS A WIDER RANGE OF APPLICATIONS DESPITE ITS IMPORTANCE CRYPTOGRAPHY IS INHERENTLY FRAGILE EVEN THE MOST SECURE CRYPTOGRAPHIC SYSTEM CAN BE RENDERED COMPLETELY INSECURE BY A SINGLE SPECIFICATION FLAW OR PROGRAMMING ERROR TRADITIONAL SOFTWARE TESTING METHODS SUCH AS UNIT TESTING ARE INSUFFICIENT TO UNCOVER SECURITY VULNERABILITIES IN CRYPTO SYSTEMS INSTEAD CRYPTOGRAPHIC SECURITY IS ESTABLISHED THROUGH MATHEMATICAL MODELING AND RIGOROUS PROOFS DEMONSTRATING THAT A SYSTEM MEETS THE NECESSARY SECURITY PROPERTIES THESE ARGUMENTS OFTEN RELY ON PLAUSIBLE ASSUMPTIONS TO VALIDATE THEIR CLAIMS ONE OF THE EARLIEST AND SIMPLEST CRYPTOGRAPHIC TECHNIQUES IS THE CAESAR CIPHER WHICH DATES BACK TO AROUND BC THIS METHOD ENCODES PLAINTEXT BY SHIFTING EACH LETTER OF THE ALPHABET BY A FIXED NUMBER OF POSITIONS WHILE THIS APPROACH WAS EFFECTIVE AT THE TIME DUE TO THE OBSCURITY OF THE METHOD IT PROVIDES NO REAL SECURITY TODAY SINCE THERE ARE ONLY 25 POSSIBLE SHIFTS THE CIPHER CAN BE EASILY BROKEN THROUGH BRUTE FORCE DESPITE ITS SIMPLICITY THE CAESAR CIPHER REMAINS ONE OF THE MOST WIDELY RECOGNIZED ENCRYPTION TECHNIQUES HOWEVER IT OFFERS NO REAL PROTECTION AS IT CAN BE QUICKLY DECIPHERED BY HAND ADDITIONALLY ITS CIPHERTEXT IS EASILY IDENTIFIABLE BECAUSE THE FREQUENCY DISTRIBUTION OF LETTERS MIRRORS THAT OF THE ENGLISH LANGUAGE THIS HIGHLIGHTS A KEY PRINCIPLE IN MODERN CRYPTOGRAPHY TRUE SECURITY RELIES NOT ONLY ON SECRECY BUT ALSO ON STRONG MATHEMATICAL FOUNDATIONS AND COMPUTATIONAL INFEASIBILITY```
