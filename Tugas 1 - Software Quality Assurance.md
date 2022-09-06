Chapter 1

# The software quality challenge

# Tantangan Mutu Perangkat Lunak

    Chapter outline

    1.1  The uniqueness of software quality assurance

    1.2 The environments for which SQA methods are developed

    Summary

    Review questions

    Topics for discussion

<div style="text-align: justify">Two basic questions should be raised before we proceed to list the variety of
subjects and details of the book:

Dua pertanyaan dasar yang diajukan sebelum kita melakukan pendaftaran jenis 
dari subjek dan rincian dari buku :


1.  Is it justified to devote a special book to software quality assurance (SQA)
or, in other words, can we not use the general quality assurance textbooks
available that are applicable to numerous areas and industries?

1) *Apakah membuat buku yang di khususkan untuk penjaminan perangkat 
lunak dapat dibenarkan atau, dengan kata lain, kenapa tidak menggunakan 
buku tentang penjaminan mutu pada umum nya yang tersedia dan dapat 
diterapkan di berbagai macam industri ?*

2.   Having decided to develop specialized books for software quality assurance, at which of the various environments of software development, from
amateurs’ hobby to professionals’ work, should we aim our main efforts?
Put simply, what are the unique characteristics of the SQA environment?

2) *Jika telah memutuskan untuk mengembangkan buku yang dikhusukan 
untuk penjaminan mutu perangkat lunak, dari bagian mana kah dari 
penjaminan perangkat lunak, apakah mulai dari hobi amatir sampai 
professional ?*


The objective of this chapter is to answer these questions by exploring the
related issues.

*Tujuan dari bab ini ialah untuk menjawab pertanyaan diatas dengan cara 
menelusuri berbagai masalah terkait.*


After completing this chapter, you will be able to:

*Setelah menyelesaikan bab ini , anda akan mampu :*

<ul>
■ Identify the unique characteristics of software as a product and as production process that justify separate treatment of its quality issues.

■ Recognize the characteristics of the environment where professional software development and maintenance take place.

■ Explain the main environmental difficulties faced by software development and maintenance teams as a result of the environment in which 
they operate.

■ *Mengidentifikasi keunikan karakteristik dari perangkat lunak sebagai 
produk dan sebagai proses produksi dengan penanganan masalah mutu 
yang berbeda pada umum nya.*

■ *Mengenali karakteristik dari lingkungan pengembangan software 
professional dan perawatan software.*

■ *Menjelaskan masalah utama yang dihadapi pada pengembangan perangkat 
lunak dan tim perawatan.*</ul>

### 1.1 The uniqueness of software quality assurance

### 1.1 Keunikan dari Penjaminan Mutu Perangkat Lunak

“Look at this,” shouted my friend while handing me **Dagal Features’s**
Limited Warranty leaflet. “Even **Dagal Features** can’t cope with software
bugs.” He pointed to a short paragraph on page 3 of the leaflet that states
the conditions of the warranty for **AMGAL**, a leading Software Master product
sold all over the world. The leaflet states the following:

*“Lihat ini,” seru teman saya sembari memberikan ku selebaran garansi terbatas
Dagal Feature. “ Bahkan Dagal Feature tidak bisa mengatasi bugs pada software.”
Dia menunjukkan paragraf pendek di halaman 3 pada selebaran yang menyatakan 
kondisi garansi dari AMGAL, leading software master product yang terjual di 
seluruh dunia. Seleberan tersebut menyatakan :*

<ul>
LIMITED WARRANTY

*GARANSI TERBATAS*

**Dagal Features** provides no warranty, either expressed or implied, with
respect to **AMGAL’s** performance, reliability or fitness for any specified
purpose. **Dagal Features** does not warrant that the software or its documentation will fulfil your requirements. although **Dagal Features** has
performed thorough tests of the software and reviewed the documentation, **Dagal Features** does not provide any warranty that the software and
its documentation are free of errors. **Dagal Features** will in no case be
liable for any damages, incidental, direct, indirect or consequential,
incurred as a result of impaired data, recovery costs, profit loss and third
party claims. the software is licensed “as is”. the purchaser assumes the
complete risk stemming from application of the **AMGAL** program, its
quality and performance.

*Dagal Features tidak menyediakan jaminan, baik secara tersurat maupun tersirat, 
sehubungan dengan kinerja, keandalan, atau kesesuaian AMGAL untuk tujuan 
tertentu apa pun. Dagal Features tidak menjamin bahwasanya software atau 
dokumentasi yang ada akan memenuhi keperluan anda. Meskipun Dagal Features 
telah melakukan berbagai macam test terhadap software dan telah mengkaji 
dokumentasi nya, Dagal Features tidak menjamin software dan dokumentasi 
terbebas dari kecacatan. Dagal Features tidak akan menjadi bertanggung jawab
atas segala kerusakan, insidental, langsung, tidak langsung atau konsekuensial,
timbul sebagai akibat dari data yang rusak, biaya pemulihan, kerugian laba, dan
ketiga klaim pihak. perangkat lunak dilisensikan "sebagaimana adanya". Pembeli
mengasumsikan risiko lengkap yang berasal dari penerapan program 
AMGAL,kualitas dan kinerja.*

If physical defects are discovered in the documentation or the CD on
which **AMGAL** is distributed, **Dagal Features** will replace, at no charge,
the documentation or the CD within 180 days of purchase, provided
proof of purchase is presented.

*Jika kerusakan fisik ditemukan pada dokumentasi atau CD yang di distribusikan 
oleh AMGAl, maka Dagal Features akan menggantinya, tanpa biaya, selama 180 
hari masa pembelian dengan bukti pembelian terlampir.*</ul>

“Is the AMGAL software really so special that its developers are incapable
of meeting the challenge of assuring a bug-free product?” continued my
friend. “Do other software packages limit their warranties in the same way?”

*“Apakah software buatan AMGAL sangat spesial sampai sampai para developer 
tidak mampu menjamin produk mereka bebas dari bug ? “ lanjut teman saya.
“Apakah software yang lain juga membatasi garansi sebagaimana yang dilakukan 
AMGAL ?.”*

Though **Dagal Features** and AMGAL are fictitious, an examination of
the warranties offered by other software developers reveals a similar pattern.
No developer will declare that its software is free of defects, as major manufacturers of computer hardware are wont to do. This refusal actually
reflects the essential elemental differences between software and other industrial
products, such as automobiles, washing machines or radios. These differences can be categorized as follows:

*Meskipun Dagal Features dan AMGAL adalah fiktif, pemeriksaan terhadap
jaminan yang ditawarkan oleh pengembang perangkat lunak lain memiliki pola 
yang sama. Tidak ada developer perangkat lunak yang menyatakan produk 
mereka terbebas dari kecacatan atau bug. Pernyataan ini sebenarnya menunjukkan 
perbedaan unsur penting antara perangkat lunak dengan industri lainnya seperti 
mobil, mesin cuci atau radio. Perbedaan nya dapat di kategorikan sebagai berikut :
*

1.  **Product complexity.** Product complexity can be measured by the number of operational modes the product permits. An industrial product,
even an advanced machine, does not allow for more than a few thousand modes of operation, created by the combinations of its different
machine settings. Looking at a typical software package one can find
millions of software operation possibilities. Assuring that the multitude
of operational possibilities is correctly defined and developed is a major
challenge to the software industry.

1) *Kompleksitas Produk. Kompleksitas produk dapat diukur menggunakan 
angka dari mode operasional yang diizinkan produk. Produk industri, 
bahkan mesin sekalipun tidak mengizinkan lebih dari beberapa ribu mode 
operasional, yang dibuat dari berbagai macam pengaturan mesin. 
Dilihat dari software package pada umum nya,kita bisa melihat jutaan 
lebih kemungkinan operasi software yang dapat dilakukan. Memastikan 
bahwa orang banyak kemungkinan operasional didefinisikan dengan benar 
dan dikembangkan adalah tantangan bagi industri perangkat lunak.*

2.  **Product visibility.** Whereas the industrial products are visible, software
products are invisible. Most of the defects in an industrial product can be
detected during the manufacturing process. Moreover the absence of a
part in an industrial product is, as a rule, highly visible (imagine a door
missing from your new car). However, defects in software products
(whether stored on diskettes or CDs) are invisible, as is the fact that parts
of a software package may be absent from the beginning.

2) *Visibilitas Produk. Dimana pada umum nya produk industri terlihat, akan 
tetapi produk software tidak terlihat. Kebanyakan kecacatan pada produk 
industri dapat terdeteksi pada saat proses manufaktur. Lebih-lebih lagi jika 
suatu bagian hilang pada produk industry makan akan sangat terlihat 
(bayangkan mobil baru tanpa pintu). Akan tetapi, kecacatan pada produk 
software sangat susah terlihat, bahkan mungkin saja ada beberapa bagian 
software yang tidak ada.*

3.  **Product development and production process**. Let us now review the
phases at which the possibility of detecting defects in an industrial product may arise:

3) *Pengembangan Produk dan Proses Produksi. Mari kita ulas fase-fase 
dimana kemungkinan kecacatan produk dapat dideteksi:*
<ul>

(a) **Product development.** In this phase the designers and quality assurance (QA) staff check and test the product prototype, in order to
detect its defects.

*Pengembangan Produk. Pada fase ini, desainer dan staff 
penjamin mutu memeriksa dan mencoba prototype produk, dengan 
tujuan untuk mengetahui dimana letak kecacatan nya.*

(b) **Product production planning.** During this phase the production
process and tools are designed and prepared. In some products there
is a need for a special production line to be designed and built. This
phase thus provides additional opportunities to inspect the product,
which may reveal defects that “escaped” the reviews and tests conducted during the development phase.

*Perencanaan Produksi Produk. Pada fase ini, proses produksi 
dan alat telah dirancang dan disediakan. Sebagian produk 
memerlukan rancangan produksi khusus. Pada fase ini dilakukan 
peninjauan Kembali dengan tujuan untuk mendeteksi kecacatan 
yang “lolos” pada fase sebelum nya.
*

(c) **Manufacturing.** At this phase QA procedures are applied to detect
failures of products themselves. Defects in the product detected in the
first period of manufacturing can usually be corrected by a change in
the product’s design or materials or in the production tools, in a way
that eliminates such defects in products manufactured in the future. 

*Manufaktur. Pada fase ini, prosedur QA dilakukan dengan tujuan 
mendeteksi kegagalan produk . Biasanya kecacatan yang dideteksi 
pada tahap awal manufaktur dapat di koreksi dengan cara 
mengganti desain atau material agar menghilangkan kecacatan 
kedepan nya.*</ul>

In comparison to industrial products, software products do not benefit
from the opportunities for detection of defects at all three phases of the
production process. The only phase when defects can be detected is the
development phase. Let us review what each phase contributes to the
detection of defects:

*Dibanding dengan produk industri, produk software tidak melakukannya pada tiga 
tahap produksi. Tahap ketika kecacatan produk dapat di deteksi adalah pada tahap 
development(pengembangan). Mari kita ulas fase atau tahap untuk mendeteksi 
kecacatan produk pada produksi software:*
<ul>

(a) **Product development.** During this phase, efforts of the development
teams and software quality assurance professionals are directed
toward detecting inherent product defects. At the end of this phase
an approved prototype, ready for reproduction, becomes available.

*Pengembangan Produk. Pada tahap ini, tim pengembang dan staff 
penjaminan mutu diarahkan untuk mendeteksi cacat bawaan produk. 
Setelah itu protoype yang telah di approve dan siap diproduksi telah 
tersedia.*

(b) **Product production planning.** This phase is not required for the software production process, as the manufacturing of software copies
and printing of software manuals are conducted automatically. This
applies to any software product, whether the number of copies is
small, as in custom-made software, or large, as in software packages
sold to the general public.

*Perencanaan Produksi Produk. Tahap ini tidak diperlukan untuk proses 
produksi perangkat lunak, karena pembuatan salinan perangkat lunak dan 
pencetakan manual perangkat lunak dilakukan secara otomatis. Ini berlaku 
untuk produk perangkat lunak apa pun, baik jumlah salinannya kecil, 
seperti dalam perangkat lunak yang dibuat khusus, atau besar, seperti 
dalam paket perangkat lunak yang akan dijual kepada masyarakat umum.*

(c) **Manufacturing.** As mentioned previously, the manufacturing of
software is limited to copying the product and printing copies of the
software manuals. Consequently, expectations for detecting defects
are quite limited during this phase.

*Manufaktur Seperti yang dikatakan sebelum nya, proses manufaktur 
software hanya sebatas meng-copy produk dan mencetak software manual. 
Akibatnya, sangat jarang kecacatan produk terdeteksi pada tahap ini.
*</Ul>

The differences affecting the detection of defects in software products versus
other industrial products are shown in Table 1.1 and Frame 1.1.


It should be noted that significant parts of advanced machinery as well
as of household machines and other products include embedded software
components (usually termed “firmware”) that are integrated into the product. These software components (the firmware) share the same
characteristics of the software products mentioned above. It follows that the
comparison shown above should actually be that of software products versus other industrial products and non-software components of industrial
products that include firmware. Hereinafter, when mentioning software, we
will mean software products as well as firmware.

*Perlu dicatat bahwa bagian penting dari mesin canggih juga
pada mesin rumah tangga dan produk lainnya termasuk perangkat lunak tertanam
komponen (biasanya disebut "firmware") yang terintegrasi ke dalam produk. Komponen perangkat lunak ini (firmware) berbagi hal yang sama
karakteristik produk perangkat lunak yang disebutkan di atas. Oleh karena itu,
perbandingan yang ditunjukkan di atas sebenarnya adalah produk perangkat lunak versus produk industri lainnya dan komponen non-perangkat lunak industri
produk yang menyertakan firmware. Selanjutnya, ketika menyebutkan perangkat lunak, kami
akan berarti produk perangkat lunak serta firmware.*


The fundamental differences between the development and production
processes related to software products and those of other industrial products
warrant the creation of a different SQA methodology for software. The need
for special tools and methods for the software industry is reflected in the professional publications as well in special standards devoted to SQA, such as
ISO 9000-3, “Guidelines for the application of ISO 9001 to the development, supply and maintenance of software”. This point is supported by the fact
that targeted guidelines have not been prepared by ISO for other industries, 

*Perbedaan mendasar antara pengembangan dan produksi
proses yang terkait dengan produk perangkat lunak dan produk industri lainnya
menjamin pembuatan metodologi SQA yang berbeda untuk perangkat lunak. Kebutuhan
untuk alat dan metode khusus untuk industri perangkat lunak tercermin dalam publikasi profesional serta dalam standar khusus yang ditujukan untuk SQA, seperti
ISO 9000-3, “Pedoman penerapan ISO 9001 untuk pengembangan, penyediaan dan pemeliharaan perangkat lunak”. Poin ini didukung oleh fakta
bahwa pedoman yang ditargetkan belum disiapkan oleh ISO untuk industri lain,*

| Characteristik | Software Product | Other Industrial products |
| ---------- | --------- | ----------- |
| Complexity | Usually, very complex product allowing for very large number of operational | Degre of complexity much lower, allowing at mos a few thousand operational options | 
| visibility of product | Invisible to detect defects or omissions by sight (e.g. of a diskette or CD storing the software) | Visible product, allowing effective detection of defect by sight |
| Nature of development and production procces | Oppurtunities to detect defects arise in only one phase, namely product development | Oppurtunities to detect defect arise in all phases of development and production : <li> product development<li> product production planning<li> manufacturing |

    Frame 1.1  **The uniqueness of the software development process**

    ■ High complexity, as compared to other industrial products

    ■ Invisibility of the product

    ■ Opportunities to detect defects (“bugs”) are limited to the product
    development phase


and the only other targeted guidelines have been prepared for services (ISO
9004-2, “Quality management and quality systems elements: Guidelines for
the services”).

*dan satu-satunya pedoman yang ditargetkan lainnya telah disiapkan untuk layanan (ISO
9004-2, “Manajemen mutu dan elemen sistem mutu: Pedoman untuk
pelayanan").*

The great complexity as well as invisibility of software, among other
product characteristics, make the development of SQA methodology and its
successful implementation a highly professional challenge.

*Kompleksitas besar serta ketidaktampakan perangkat lunak, antara lain
karakteristik produk, membuat pengembangan metodologi SQA dan
keberhasilan implementasi tantangan yang sangat profesional.*</div>