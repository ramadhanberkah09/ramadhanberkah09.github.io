---
layout: post
title:  "Web Storage"
date:   2016-21-06
excerpt: "Minimal, one column Jekyll theme for your blog."
project: true
tag:
- webstorage 
- localstorage
- sessionstorage
comments: false
---

<script type="text/javascript" >
// fungsi simpan(), ketika tombol diklik maka string 
// di dalam input akan tersimpan ke dalam storage browser
function simpan() {		
	var storage = document.getElementById('nama').value;
	localStorage.setItem('Text',storage);
} 
// tampil() akan menampilkan string yang tersimpan
// ke tag div yang ditentukan "hasil"
function tampil() {
	var tampilNama = localStorage.getItem('Text');
	if (tampilNama) {
	x = document.getElementById('tampil');
	x.innerHTML=tampilNama;
	}
}
// fungsi untuk menghapus localstorage browser
function hapus() {
	localStorage.removeItem('Text');
}
</script>

		<input type="text" id="nama" />
		<input type="button" value="Simpan" onclick="simpan()" />
		<input type="button" value="Tampil" onclick="tampil()" />
		<input type="button" value="Hapus" onclick="hapus()" />
		<div id="tampil"></div>
