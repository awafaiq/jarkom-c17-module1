| Name | NRP | Class |
| ---- | --- | ----- |
| Danish Faiq Ibad Yuadi | 5025241038 | C |

## Task 1

- Flag

<img width="1355" height="39" alt="image" src="https://github.com/user-attachments/assets/4ae377bc-539b-42b1-9f57-5730d3b3683f" />


> a. Berapa banyak packet yang terekam pada file pcapng?

> _a. How many packets are recorded in the pcapng file?_

**Answer:**
<img width="526" height="36" alt="image" src="https://github.com/user-attachments/assets/7aa59251-aa25-4aa7-9662-b394f0fcf607" />

- Filter expression

None

- Explanation

On the Wireshark Application after you open the pcapng file for soal1234 at the right-bottom side of the application.

- Output result

<img width="1537" height="992" alt="image" src="https://github.com/user-attachments/assets/74c6c5e0-4b37-4867-a797-ac71627cc7fa" />

<br>
<br>

> b. Ada berapa jenis protocol (total) yang terekam pada traffic?

> _b. How many types of protocol (totals) are recorded in the traffic?_

**Answer:** 
<img width="613" height="37" alt="image" src="https://github.com/user-attachments/assets/0a695848-965a-4a9b-b7d5-ce12db6f2135" />

- Filter expression

None

- Explanation

Go to the Statistic option at the top of the application and choose Protocol Hierarchy to check how much protocol is displayed on the pcapng file for soal1234.

- Output result

<img width="1371" height="353" alt="image" src="https://github.com/user-attachments/assets/a45f5086-14f8-4af7-a7cc-fa449a633d7d" />

<br>
<br>

> c. Ada berapa jenis protocol berbasis TCP yang terekam pada traffic?

> _c. How many types of TCP-based applications protocol are recorded in the traffic?_

**Answer:**
<img width="690" height="42" alt="image" src="https://github.com/user-attachments/assets/6958a65f-512d-4b64-9982-811ff9cf1205" />

- Filter expression

None

- Explanation

Go to the Statistic option at the top of the application and choose Protocol Hierarchy to check how much protocol below TCP is displayed on the pcapng file for soal1234.

- Output result

<img width="1367" height="202" alt="image" src="https://github.com/user-attachments/assets/2919ecc2-6890-4752-9c43-4079f9dc6114" />

  <br>
  <br>

> d. Ada berapa banyak packet dengan protokol TCP murni yang terekam pada traffic (tanpa data)?

> _d. How many packets with pure TCP protocol are recorded in the traffic (without data)?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

## Task 2

- Flag

  `put your flag here`

> a. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag [ACK]?

> _a. How many packets succeed that are pure TCP based and have [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> b. Berapa banyak packet berhasil yang berbasis murni TCP yang hanya memiliki flag [ACK]?

> _b. How many packets succeed that are pure TCP based and have only [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag selain hanya [ACK]?

> _c. How many packets succeed that are pure TCP based and contain flags other than just [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 3

- Flag

<img width="1360" height="43" alt="image" src="https://github.com/user-attachments/assets/4098f929-6c23-4dfd-a0fe-a2de3f493a6b" />

> a. Pada port berapa client telnet terbuka?

> _a. In what port is the telnet client open?_

**Answer:**
<img width="417" height="45" alt="image" src="https://github.com/user-attachments/assets/97fbcbac-5f14-43ff-8b45-c59a153da9cd" />

- Filter expression

telnet

- Explanation

search any telnet package and check the packet details. We will see its source port is 54184.

- Output result

<img width="901" height="318" alt="image" src="https://github.com/user-attachments/assets/b17b2ff0-1446-447b-ac07-1b791ac78514" />

  <br>
  <br>

> b. Berapa byte file response yang dikirim dari server?

> _b. How many bytes of the response files are sent from the server?_

**Answer:**
<img width="525" height="45" alt="image" src="https://github.com/user-attachments/assets/30d5cea0-9fbf-439d-ab72-14f16d9177bf" />

- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. The total size of byte file that is from the server (172.16.16.102) to destination is (1449 bytes).

- Output result

<img width="1176" height="992" alt="image" src="https://github.com/user-attachments/assets/62456b9b-663a-41fb-b9ab-e7db8e490516" />

  <br>
  <br>

> c. Apa username yang digunakan client telnet untuk berhubungan dengan server?

> _c. What telnet client's username is used to connect with the server?_

**Answer:**
<img width="758" height="45" alt="image" src="https://github.com/user-attachments/assets/7763dff0-e104-42dc-a263-86eaaef3233f" />

- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. From there, you will see from server perspective (172.16.16.102), the client name is jovyan.

- Output result

<img width="698" height="158" alt="image" src="https://github.com/user-attachments/assets/42e22305-a1b3-41cd-a293-0f137f18efb7" />

  <br>
  <br>

> d. Apa password client telnet?

> _d. What is the telnet client's password?_

**Answer:**
<img width="293" height="41" alt="image" src="https://github.com/user-attachments/assets/c947d8e2-c68b-40df-a75d-ed4d68447edc" />

- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. Checking from the entire conversation, you will see password 123.

- Output result

<img width="1176" height="985" alt="image" src="https://github.com/user-attachments/assets/ccad013c-a4e8-49a6-bb3a-c260ad4ec81b" />

  <br>
  <br>

## Task 4

- Flag

<img width="1369" height="48" alt="image" src="https://github.com/user-attachments/assets/d8f17d3b-4b9f-4cc6-923f-dcc954fdec8f" />

> a. Apa perintah pertama yang ditulis client pada koneksi telnet?

> _a. What is the first command that client wrote on telnet connection?_

**Answer:**
<img width="646" height="42" alt="image" src="https://github.com/user-attachments/assets/2d5a29e9-e4bd-42fc-8eb1-38f43abc399c" />

- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. From there, you will see from server perspective (172.16.16.102), and we will see the client type 'echo' as the first command.

- Output result

<img width="1096" height="39" alt="image" src="https://github.com/user-attachments/assets/43a77ef4-6a89-4fb4-a28f-cfdd5bbff887" />

  <br>
  <br>

> b. Apa nama file .txt di server (ditulis bersama ekstensinya)?

> _b. What is the name of .txt file on the server (write with the extension)?_

**Answer:**
<img width="628" height="51" alt="image" src="https://github.com/user-attachments/assets/3c77d2e9-b774-48fc-89ea-518700aa0972" />

- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. From there, you will see from server perspective (172.16.16.102), and we will see the client type test as the name of the txt file they made.

- Output result

<img width="885" height="32" alt="image" src="https://github.com/user-attachments/assets/90bb49a2-a4a9-4020-a96e-f12637ffa6ce" />

  <br>
  <br>

> c. Apa kata pertama dari frasa yang dimasukkan client ke dalam file sebelumnya?

> _c. What is the first word that the client inserted into the previous file?_

**Answer:**
<img width="788" height="53" alt="image" src="https://github.com/user-attachments/assets/8132908d-1e9a-4fdb-8829-98ec0b98b4a2" />


- Filter expression

1. telnet
2. tcp.stream eq 7 (automatically converted to this filter once you follow its TCP stream)

- Explanation

search any telnet package and pick one of those packages to follow its TCP Stream. From there, you will see from server perspective (172.16.16.102), and we will see the client type Jarkom as the first word on the test.txt

- Output result

<img width="1144" height="56" alt="image" src="https://github.com/user-attachments/assets/099fcb87-97ee-4fba-8744-e12ac6ce205f" />

  <br>
  <br>

## Task 5

- Flag

<img width="1219" height="44" alt="image" src="https://github.com/user-attachments/assets/508b0350-2efc-4d0b-8df7-61c505c32304" />

> a. Berapa banyak packet berbasis HTTP yang terekam pada file pcapng?

> _a. How many HTTP packets are recorded in the pcapng file?_

**Answer:** 
<img width="680" height="36" alt="image" src="https://github.com/user-attachments/assets/cedf14dc-05e1-4a79-9086-939878c553d0" />

- Filter expression

http

- Explanation

Check displayed packets after typing the filter to see how much packets it is.

- Output result

<img width="1733" height="896" alt="image" src="https://github.com/user-attachments/assets/1aaaeb5e-79b1-4c1f-bf4f-81a92d1613ca" />

  <br>
  <br>

> b. Ada berapa HTTP packet yang berupa response?

> _b. How many response HTTP packets are recorded in the traffic?_

**Answer:**
<img width="467" height="38" alt="image" src="https://github.com/user-attachments/assets/6c74d036-c811-40d6-8cde-8c3a96f2a60c" />

- Filter expression

http.response

- Explanation

Check displayed packets after typing the filter to see how much packets it is.

- Output result

<img width="1747" height="892" alt="image" src="https://github.com/user-attachments/assets/cc16aa52-9d27-4951-b8e8-56460e97842a" />

  <br>
  <br>

> c. Ada berapa paket berbasis HTTP yang berhasil?

> _c. How many HTTP packets that succeed?_

**Answer:**
<img width="465" height="35" alt="image" src="https://github.com/user-attachments/assets/4b909834-0e8a-4891-aa5a-c49875bac5a6" />

- Filter expression

http

- Explanation

Check displayed packets after typing the filter to see how much packets it is. But exclude the black package one because it is not captured (resulting for not succeed). The total packages after excluding are 298 - 2 = 296.

- Output result

<img width="1751" height="862" alt="image" src="https://github.com/user-attachments/assets/a91d9692-05f7-4018-b2ae-962a92cc0c81" />

  <br>
  <br>

> d. Apa alamat IP dari client HTTP yang tersambung lokal dengan mesin lain?

> _d. What is the client HTTP IP Address in connection with other local machine?_

**Answer:**
<img width="760" height="43" alt="image" src="https://github.com/user-attachments/assets/1874b7ea-a985-4d28-9c84-74520e648af7" />

- Filter expression

1. http
2. tcp.stream eq 73 (automatically converted to this filter once you follow its HTTP stream)

- Explanation

search any http package and pick one of those packages to follow its TCP Stream. From there, you will see from server perspective (172.16.16.101) and client (172.16.16.101) IP are the same

- Output result

<img width="425" height="145" alt="image" src="https://github.com/user-attachments/assets/888d7ea1-f801-4b1e-9096-71e222a175bf" />


  <br>
  <br>

## Task 6

- Flag

<img width="1369" height="42" alt="image" src="https://github.com/user-attachments/assets/53cd1ae7-f097-4fe3-8c7b-aa9f1092cbc2" />

> a. Apakah kamu menemukan fake flag? Tuliskan seluruhnya!

> _a. Did you find the fake flag? Write it whole!_

**Answer:**
<img width="597" height="40" alt="image" src="https://github.com/user-attachments/assets/9479bb3c-6309-47e8-a503-bb86f2ac8db7" />

- Filter expression

1. http
2. Packet List : String : Flag (to get packet that has flag on its info)
3. tcp.stream eq 31 (automatically converted to this filter once you follow its HTTP stream)

- Explanation

After you get a packet that has flag.txt on its info, follow its HTTP stream, and you will see FakeFlag{JarkomGampang} on the txt file

- Output result

<img width="1919" height="1003" alt="image" src="https://github.com/user-attachments/assets/5bd89975-dd63-40be-8dec-b2a0c0e578e7" />

  <br>
  <br>

> b. Tuliskan username dan password yang tertulis! (format username:password)

> _b. Write the written username and password! (format username:password)_

**Answer:**
<img width="754" height="50" alt="image" src="https://github.com/user-attachments/assets/ebc92f01-cce1-4870-9dfd-a2f6531028e5" />

- Filter expression

1. http
2. Packet List : String : txt (to get packet that has txt on its info)
3. tcp.stream eq 32 (automatically converted to this filter once you follow its HTTP stream)

- Explanation

Similar to previous sub-task, after you get a packet that has password on its info (in this case, the name is passwd.txt), follow its HTTP stream, and you will see Rey:123 on the txt file

- Output result

<img width="1919" height="1030" alt="image" src="https://github.com/user-attachments/assets/7d96f7d5-3844-4ea9-b146-18cc814fb897" />

  <br>
  <br>

## Task 7

- Flag

  `put your flag here`

> Apa nama gambar yang direquest oleh client? (tulis dengan ekstensinya)

> _What is the image that is being requested by the client? (write with its extension)_

**Answer:**
<img width="701" height="42" alt="image" src="https://github.com/user-attachments/assets/339d5131-d8cd-483a-a057-ae5210e9a290" />


- Filter expression

1. http
2. Packet List : String : jpg (to get packet that has jpg on its info)

- Explanation

Because the question said 'image', the only possible extension that comes to mind is either jpg/jpeg/png for the most used extension nowadays. But for this case after the filter is used, jpg is used and the file name is donalbebek.

- Output result

<img width="1919" height="911" alt="image" src="https://github.com/user-attachments/assets/47f04053-9b37-4de4-a687-a3cd10e2e76e" />


  <br>
  <br>

## Task 8

- Flag

<img width="1354" height="47" alt="image" src="https://github.com/user-attachments/assets/5ce07222-fb85-4822-820e-8a6c937b3e78" />

> a. Berapa banyak packet berbasis FTP yang terekam pada file pcapng? (with the data)

> _a. How many FTP packets are recorded in the pcapng file? (with the data)_

**Answer:**
<img width="873" height="46" alt="image" src="https://github.com/user-attachments/assets/16dc1f45-488e-43b9-aae3-830a8e77f278" />

- Filter expression

ftp or ftp-data

- Explanation

Check displayed packets after typing the filter to see how much packets it is.

- Output result

<img width="1208" height="900" alt="image" src="https://github.com/user-attachments/assets/ad0fe9c0-3044-4b1d-b0bc-4a37677cd078" />


  <br>
  <br>

> b. Apa username dan password client di koneksi FTP? (tulis dalam format username:password)

> _b. What is the client's username and password in FTP connection? (write in following format username:password)_

**Answer:**
<img width="890" height="43" alt="image" src="https://github.com/user-attachments/assets/18999ca9-a661-4bf6-96e3-54ea4e4f8d1d" />

- Filter expression

1. ftp
2. tcp.stream eq 8 (automatically converted to this filter once you follow its tcp stream)

- Explanation

search any FTP package and pick one of those packages to follow its TCP Stream. Check the entire conversation, you will see the user password after the server asked for it. 

- Output result

<img width="1591" height="1025" alt="image" src="https://github.com/user-attachments/assets/19c47a40-8afb-4492-b6da-8cabf9f57776" />

  <br>
  <br>

> c. What is the client's command for showing server directory that was sent on request packet?

> _c. Apa command client untuk melihat direktori server yang dikirimkan dalam request packet?_

**Answer:**
<img width="882" height="42" alt="image" src="https://github.com/user-attachments/assets/55765c4c-7ba4-48c5-9914-13ce6bc1e495" />

- Filter expression

1. ftp
2. tcp.stream eq 8 (automatically converted to this filter once you follow its tcp stream)

- Explanation

search any FTP package and pick one of those packages to follow its TCP Stream. Check the entire conversation, you will see the user type LIST to check if there's anything inside of a folder in ftp directory server

- Output result

<img width="1590" height="1019" alt="image" src="https://github.com/user-attachments/assets/5e1e16d6-9f41-4428-a022-8ca7c5838244" />

  <br>
  <br>

## Task 9

- Flag

<img width="1397" height="47" alt="image" src="https://github.com/user-attachments/assets/0cd24d03-8b8f-4c4a-8a92-adce0b60079c" />

> a. Apa alamat IP dari FTP server?

> _a. What is the FTP server IP Address?_

**Answer:**
<img width="321" height="45" alt="image" src="https://github.com/user-attachments/assets/8b324ca7-b7ba-4209-8f9a-42da20539145" />

- Filter expression

ftp

- Explanation

based from the conversation of 2 ftp packages, the conversation that is showed in Info, FTP server IP is 172.16.16.101

- Output result

<img width="1919" height="104" alt="image" src="https://github.com/user-attachments/assets/92dc4914-2d9e-45f8-a33e-a0a1e1d7bb93" />


  <br>
  <br>

> b. Berapa banyak file yang ada dalam direktori FTP server?

> _b. How many files are there inside the FTP server directory?_

**Answer:**
<img width="558" height="39" alt="image" src="https://github.com/user-attachments/assets/a9e8307d-0e0d-4c4d-99c8-232e8a24adea" />

- Filter expression

1. Packet List : String : LIST (to get packet that has LIST on its info)

- Explanation

To check how much files, we will go to package that has LIST response (meaning that LIST showing result how much file in the FTP server directory)

- Output result

<img width="1767" height="1012" alt="image" src="https://github.com/user-attachments/assets/99911e38-a489-4f55-8edc-e8abac4bedd6" />

  <br>
  <br>

> c. Apa nama dari file yang digunakan dalam page.html? (tulis lengkap namanya beserta ekstensinya dan dipisahkan dengan koma ',')

> _c. What are the filenames used in the page.html? (write the filebames with their extensions and separate them with comma ',')_

**Answer:**
<img width="1283" height="40" alt="image" src="https://github.com/user-attachments/assets/2670cb2e-49df-43ed-a750-ba286898a5e8" />

- Filter expression

1. Packet List : String : html (to get packet that has html on its info)

- Explanation

To check what is the name of the file on html file, we will go to package that has html response (meaning that html showing result what file inside of html)

- Output result

<img width="1858" height="1027" alt="image" src="https://github.com/user-attachments/assets/48eb5604-1d22-493e-b5ac-70a74019f1dd" />

  <br>
  <br>

## Task 10

- Flag

<img width="1372" height="53" alt="image" src="https://github.com/user-attachments/assets/2ba67347-94d0-4749-a7dd-89cd0f4c3a4a" />

> a. Apa nama file yang mengandung string terencode?

> _a. What is the filename that contains encoded string?_

**Answer:**
<img width="491" height="49" alt="image" src="https://github.com/user-attachments/assets/2d738c51-b24c-450f-9d45-bb94274ae44c" />

- Filter expression

1. Packet List : String : secret (to get packet that has secret on its info)

- Explanation

After listening the conversation based from the previous question, a package that named secret should have encoded string.

- Output result

<img width="1918" height="1032" alt="image" src="https://github.com/user-attachments/assets/9a7cf9d3-e08e-49aa-9683-0a48e2288930" />

  <br>
  <br>

> b. Apa nama file hasil copy file sebelumnya?

> _b. What is the filename of the previous file copy?_

**Answer:**
<img width="447" height="54" alt="image" src="https://github.com/user-attachments/assets/174b248a-62df-46b8-865a-0b8b8c248146" />

- Filter expression

1. ftp
2. tcp.stream eq 8 (automatically converted to this filter once you follow its tcp stream)

- Explanation

search any FTP package and pick one of those packages to follow its TCP Stream. Check the entire conversation, you will see the user copying using STOR command and its copy file named secret1.txt

- Output result

<img width="499" height="103" alt="image" src="https://github.com/user-attachments/assets/4f873c23-5f9d-48ef-ad4a-e15c89ba6ed0" />


  <br>
  <br>

> c. What is the decoded string from the previous file?

> _c. Apa decoded string dari file tersebut?_

**Answer:**
<img width="1374" height="59" alt="image" src="https://github.com/user-attachments/assets/7db6d09d-ed41-4426-858d-212c78252df9" />

- Filter expression

1. Packet List : String : secret (to get packet that has secret on its info)

- Explanation

went back to 10.a and copy the string to a decoder website so we can get the decoded version of the encoded string

- Output result

<img width="1914" height="874" alt="image" src="https://github.com/user-attachments/assets/bb58050e-de0f-44af-8c0d-d2a158b0951d" />

  <br>
  <br>

## Summary
This practicum is indeed very insightful for me. We are using Wireshark to sniff out informations that we could get from the pcapng file by utilizing the tools Wireshark provided such as filter and following a protocol stream to answer the question on CTF-based practicum. As time passed, I've realized that finding information isn't easy as it looks, as we need to know exactly the details of the information before by using correct tools to sniff out of it.


## Problems
The most frustrating question for me is number 2 where I cannot found any logical filter to get the exact number of the answer even after getting a hint until the practicum ends. I was so disappointed on myself, that I should just have use a good filter + a manual search to get the answer. Picture below is a representative of my emotion.

<img width="431" height="240" alt="image" src="https://github.com/user-attachments/assets/098faeb0-a5b1-4ed7-82b8-331a0d87a904" />
