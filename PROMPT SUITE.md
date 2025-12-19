//Form Permohonan//

Ekstrak Informasi dari dalam dokumen berupa

1. Data Principal (Nama dan Alamat)
2. Data Obligee (Nama, alamat, dan sumber anggaran)
3. Detail Kafalah (produk, jenis, nilai potensi, dan nilai plafon/Plafond Guarantee)
4. Informasi Kontrak (jangka waktu dan periode kontrak)
5. Manajemen (nama dan jabatan penanggung jawab dari jajaran direksi)
   dengan format JSON seperti berikut:

{
"name_principal": str
"address_principal": str
"name_obligee": str
"address_obligee": str
"budget_obligee": str
"name_product": str
"type_product": str
"pvalue_product": str
"pguarantee_product": str
"length_contract": str
"period_contract": str
"stakeholder_name": str
"stakeholder_position": str
}

//

//LAPKEU PRINCIPAL//
Ekstrak Informasi dari dalam dokumen berupa:

1. Assets, yang terdiri atas Aset Lancar, Aset Tetap, dan Jumlah Aset
2. Performance yang terdiri atas Pendapatan dan Laba
3. Liabilities/Equity, yang terdiri atas Kewajiban Lancar, Tidak Lancar, Jumlah Kewajiban, Ekuitas, Total Kewajiban dan Ekuitas
4. Ownership, yang terdiri atas Nama pemegang saham, jumlah lembar saham, dan jumlah modal saham

dengan format dalam bentuk JSON seperti berikut:

{
"asset_aslancar": str
"asset_astetap": str
"asset_asjumlah": str
"perform_pendapatan": str
"perform_laba": str
"eq_kwlancar": str
"eq_tdklancar": str
"eq_jmlkw": str
"eq_ekuitas": str
"eq_total": str
"own_nama": str
"own_lbrsaham": str
"own_jmsaham": str

}
//////

//LAPKEU OBLIGEE//
Ekstrak informasi dari dalam dokumen berupa:

1. Laba Tahun berjalan yang dapat diatribusikan
2. Total Penghasilan komprehensif tahun berjalan yang dapat diatribusikan
3. Laba Tahun berjalan per saham yang dapat diatribusikan kepada pemilik entitas induk

dengan format dalam bentuk JSON seperti berikut:

{
"lbtahun_atribusi":str
"totalhasil_atribusi":str
"lbtahun_saham":str
}
//

//NIB//
Ekstrak informasi dari dalam dokumen berupa:

1. Bidang Usaha
2. Nomor Induk Berusaha
3. Kedudukan atas alamat kantor

dengan format dalam bentuk JSON seperti berikut:

{
"bidang_usaha": [
"nama_bidang_usaha":str
],
"nomor_induk":str
"kdd_aalamat":str
}
////////////

//Akta Pendirian//
Ekstrak informasi dari dalam dokumen berupa:

1. Nomor Akta Pendirian
2. Susunan Pengurus dan Pemegang Saham
3. Jumlah lembar saham
4. Lama Operasional Usaha
   Output hasil dalam format JSON sebagai berikut:
   {
   "nomor_akta_pendirian": "string",
   "susunan_pengurus_dan_pemegang_saham": [
   {
   "nama": "string",
   "jabatan": "string",
   }
   ],
   "jumlah_lembar_saham": "string",
   "lama_operasional_usaha": "string"
   }
   //////////////////////

//AKTA Perubahan/
Ekstrak informasi dari dalam dokumen berupa:

1. Nomor Akta Perubahan
2. Nama Notaris
3. Tanggal Akta Perubahan
4. Lokasi

dengan format dalam bentuk JSON seperti berikut:

{
"nomor_akta_perubahan":str
"name_notaris":str
"tgl_akta":str
"lokasi":str
}
//

//NPWP//
Ekstrak informasi dari dalam dokumen berupa:

1. Nomor NPWP

dengan format dalam bentuk JSON seperti berikut:

{
"npwp":str
}
//

//PEFINDO//
Ekstrak informasi dari dalam dokumen berupa:

1. Pefindo Kredit masing-masing pengurus dan pemegang saham
2. baki kredit

dengan format dalam bentuk JSON seperti berikut:

{
"pefindo_credit":str
"baki_credit":str
}

//

//List Tenaga Ahli//
Ekstrak informasi dari dalam dokumen berupa Semua Nama Tenaga Ahli yang tertera dalam Dokumen
Output hasil dalam format JSON seperti berikut:
{
"tenaga_ahli": [
"nama": str
],
}

```json
{
  "name_principal": "PT PROVICES INDONESIA",
  "address_principal": "Gedung Bakrie Tower Lantai 80, Kawasan Rasuna Epicentrum, Desa/Kelurahan Karet Kuningan, Kec. Setiabudi, Kota Adm. Jakarta Selatan, Provinsi DKI Jakarta",
  "name_obligee": "Bank Indonesia",
  "address_obligee": "Jl. M.H. Thamrin No.2 Jakarta 10350",
  "budget_obligee": "Rp 26.596.218.724,42",
  "name_product": "(V) JAMINAN PENAWARAN/BID BOND",
  "type_product": "PERFORMANCE BOND",
  "pvalue_product": "Rp. 400.000.000 dan Persentase 1,99%",
  "pguarantee_product": "120 (seratus dua puluh) hari",
  "length_contract": "120 (seratus dua puluh) hari",
  "period_contract": "Dari/From: Tanggal 13 November 2025 Sampai/To: 12 Maret 2026",
  "stakeholder_name": "MELKY ALIANDRI, ST/DIREKTUR",
  "stakeholder_position": "DIREKTUR"
}
```
