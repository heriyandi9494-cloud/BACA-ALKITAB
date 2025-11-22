<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Komitmen membaca alkitab</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body { background-image:url('https://i.postimg.cc/sXcWH6ZP/eaaa57f44a6f5a960fa19b2f23d256f8.jpg'); }
    .card { border-radius: 12px; }
    .item-nama { cursor: pointer; color: #0d6efd; font-weight: 600; }
    .btn-group-toggle .btn { min-width: 100px; }
  </style>
</head>
<body>
<div class="container py-4">
  <h3 class="text-center mb-4">𝐊𝐌𝐀𝟑𝟏𝟐𝐇𝐀𝐑𝐈</h3>

  <div class="card p-3 shadow-sm mb-4">
    <div class="mb-2">
      <label class="form-label">𝐍𝐨</label>
      <input type="number" id="no" class="form-control" />
    </div>

    <div class="mb-2">
      <label class="form-label">𝐍𝐚𝐦𝐚 𝐏𝐞𝐬𝐞𝐫𝐭𝐚</label>
      <input type="text" id="nama" class="form-control" />
    </div>

    <div class="row">
      <div class="col-md-6 mb-2">
        <label class="form-label">𝐇𝐚𝐫𝐢</label>
        <input type="text" id="hari" class="form-control" placeholder="contoh: Senin" />
      </div>
      <div class="col-md-6 mb-2">
        <label class="form-label">𝐓𝐚𝐧𝐠𝐠𝐚𝐥</label>
        <input type="date" id="tanggal" class="form-control" />
      </div>
    </div>

    <div class="mb-2">
      <label class="form-label">𝐒𝐭𝐚𝐭𝐮𝐬 𝐌𝐞𝐦𝐛𝐚𝐜𝐚</label>
      <div class="btn-group btn-group-toggle d-flex mb-2" data-bs-toggle="buttons">
        <button type="button" class="btn btn-outline-success" id="btnMembaca" onclick="setStatus(true)">𝐌𝐞𝐦𝐛𝐚𝐜𝐚</button>
        <button type="button" class="btn btn-outline-danger" id="btnTidakMembaca" onclick="setStatus(false)">𝐓𝐢𝐝𝐚𝐤 𝐌𝐞𝐦𝐛𝐚𝐜𝐚</button>
      </div>
    </div>

    <div class="mb-2">
      <label class="form-label">𝐉𝐮𝐦𝐥𝐚𝐡 (𝐏𝐞𝐫𝐢𝐤𝐨𝐩)</label>
      <input type="number" id="jumlah" class="form-control" onchange="hitungPersen()" />
    </div>

    <div class="mb-2">
      <label class="form-label">𝐏𝐞𝐫𝐬𝐞𝐧𝐭𝐚𝐬𝐞 𝐌𝐞𝐦𝐛𝐚𝐜𝐚 (%)</label>
      <input type="number" id="persen" class="form-control" readonly style="background:#e7c8c8" />
    </div>

    <div class="mb-2">
      <label class="form-label">𝐁𝐚𝐜𝐚𝐚𝐧 𝐈𝐧𝐣𝐢𝐥</label>
      <input type="text" id="bacaan" class="form-control" />
    </div>

    <div class="mb-2">
      <label class="form-label">𝐀𝐲𝐚𝐭 𝐄𝐦𝐚𝐬</label>
      <input type="text" id="ayat" class="form-control" />
    </div>

    <div class="d-grid gap-2">
      <button id="btnSimpan" class="btn btn-primary" onclick="simpan()">𝐒𝐢𝐦𝐩𝐚𝐧</button>
      <button id="btnBatal" class="btn btn-secondary d-none" onclick="batalEdit()">𝐁𝐚𝐭𝐚𝐥 𝐄𝐝𝐢𝐭</button>
    </div>
  </div>

  <h4 class="mb-3">𝐃𝐚𝐭𝐚 𝐏𝐞𝐬𝐞𝐫𝐭𝐚</h4>
  <div id="list" class="mb-4"></div>

  <hr>
  <h4 class="mb-2">𝐃𝐞𝐭𝐚𝐢𝐥 𝐏𝐞𝐬𝐞𝐫𝐭𝐚</h4>
  <div id="detail" class="card p-3 shadow-sm min-vh-25"></div>
</div>

<script>
let data = JSON.parse(localStorage.getItem('dataPeserta') || '[]');
let editIndex = -1;
const TOTAL_BACAAN = 365;
let statusMembaca = true; // default membaca

function setStatus(flag){
  statusMembaca = flag;
  document.getElementById('btnMembaca').classList.toggle('active', flag);
  document.getElementById('btnTidakMembaca').classList.toggle('active', !flag);
  hitungPersen();
}

function hitungPersen(){
  const jumlahInput = Number(document.getElementById('jumlah').value) || 0;
  const nama = document.getElementById('nama').value.trim();
  let sebelumnya = data.filter(d => d.nama === nama).reduce((acc, cur) => acc + cur.jumlah, 0);
  let total = statusMembaca ? sebelumnya + jumlahInput : Math.max(0, sebelumnya - jumlahInput);
  const persen = total > 0 ? (total / TOTAL_BACAAN * 100).toFixed(1) : 0;
  document.getElementById('persen').value = persen;
}

function validasiInput(item){
  if(!item.no) { alert('Masukkan No'); return false; }
  if(!item.nama) { alert('Masukkan Nama Peserta'); return false; }
  if(!item.tanggal) { alert('Pilih Tanggal'); return false; }
  if(!item.jumlah && item.jumlah !== 0) { alert('Masukkan Jumlah Bacaan'); return false; }
  return true;
}

function simpan(){
  const item = {
    no: document.getElementById('no').value.trim(),
    nama: document.getElementById('nama').value.trim(),
    hari: document.getElementById('hari').value.trim(),
    tanggal: document.getElementById('tanggal').value,
    jumlah: statusMembaca ? Number(document.getElementById('jumlah').value) || 0 : -(Number(document.getElementById('jumlah').value) || 0),
    persen: Number(document.getElementById('persen').value) || 0,
    bacaan: document.getElementById('bacaan').value.trim(),
    ayat: document.getElementById('ayat').value.trim()
  };

  if(!validasiInput(item)) return;

  if(editIndex >= 0){
    data[editIndex] = item;
    editIndex = -1;
    document.getElementById('btnBatal').classList.add('d-none');
    document.getElementById('btnSimpan').textContent = 'Simpan';
    clearForm();
    simpanLocalStorage();
    tampilkan();
    return;
  }

  data.push(item);
  clearForm();
  simpanLocalStorage();
  tampilkan();
}

function simpanLocalStorage(){
  localStorage.setItem('dataPeserta', JSON.stringify(data));
}

function clearForm(){
  document.getElementById('no').value = '';
  document.getElementById('nama').value = '';
  document.getElementById('hari').value = '';
  document.getElementById('tanggal').value = '';
  document.getElementById('jumlah').value = '';
  document.getElementById('persen').value = '';
  document.getElementById('bacaan').value = '';
  document.getElementById('ayat').value = '';
  statusMembaca = true;
  setStatus(true);
}

function tampilkan(){
  const container = document.getElementById('list');
  container.innerHTML = '';
  const namaUnik = [...new Set(data.map(d => d.nama))];

  if(namaUnik.length === 0){ container.innerHTML = '<div class="text-muted">𝓑𝓮𝓵𝓾𝓶 𝓪𝓭𝓪 𝓭𝓪𝓽𝓪.</div>'; document.getElementById('detail').innerHTML=''; return; }

  namaUnik.forEach(nm =>{
    const card = document.createElement('div');
    card.className = 'card p-3 shadow-sm mb-2';
    const safeName = nm.replace(/'/g, "\\'").replace(/"/g, '\\"');
    card.innerHTML = `<div class='item-nama' onclick="bukaDetail('${safeName}')">${nm}</div>`;
    container.appendChild(card);
  });
}

function bukaDetail(nama){
  const detail = document.getElementById('detail');
  detail.innerHTML = '';
  const items = data.map(d => ({...d})).filter(d => d.nama === nama);
  if(items.length === 0){ detail.innerHTML = '<div class="text-muted">Tidak ada data.</div>'; return; }

  let html = `<h5>${nama}</h5>`;
  items.forEach(it =>{
    html += `<div class='mt-2 p-2 border rounded'>
      <strong>No:</strong> ${it.no}<br>
      <strong>Hari:</strong> ${it.hari}<br>
      <strong>Tanggal:</strong> ${it.tanggal}<br>
      <strong>Persentase:</strong> ${it.persen}%<br>
      <strong>Bacaan Injil:</strong> ${it.bacaan}<br>
      <strong>Ayat Emas:</strong> ${it.ayat}<br>
      <div class='mt-2'>
        <button class='btn btn-warning btn-sm' onclick="mulaiEdit('${it.no}','${it.tanggal}','${it.bacaan.replace(/'/g,"\\'")}')">Edit</button>
        <button class='btn btn-danger btn-sm ms-2' onclick="hapusItem('${it.no}','${it.tanggal}','${it.bacaan.replace(/'/g,"\\'")}')">Hapus</button>
      </div>
    </div>`;
  });
  detail.innerHTML = html;
}

function mulaiEdit(no, tanggal, bacaan){
  const index = data.findIndex(d => d.no === no && d.tanggal === tanggal && d.bacaan === bacaan);
  if(index === -1) return;
  editIndex = index;
  const item = data[index];
  document.getElementById('no').value = item.no;
  document.getElementById('nama').value = item.nama;
  document.getElementById('hari').value = item.hari;
  document.getElementById('tanggal').value = item.tanggal;
  document.getElementById('jumlah').value = Math.abs(item.jumlah);
  statusMembaca = item.jumlah >= 0;
  setStatus(statusMembaca);
  hitungPersen();
  document.getElementById('bacaan').value = item.bacaan;
  document.getElementById('ayat').value = item.ayat;
  document.getElementById('btnBatal').classList.remove('d-none');
  document.getElementById('btnSimpan').textContent = 'Perbarui';
  window.scrollTo({top:0,behavior:'smooth'});
}

function batalEdit(){
  editIndex = -1;
  clearForm();
  document.getElementById('btnBatal').classList.add('d-none');
  document.getElementById('btnSimpan').textContent = 'Simpan';
}

function hapusItem(no, tanggal, bacaan){
  if(!confirm('Hapus data ini?')) return;
  data = data.filter(d => !(d.no === no && d.tanggal === tanggal && d.bacaan === bacaan));
  simpanLocalStorage();
  tampilkan();
  document.getElementById('detail').innerHTML = '';
}

tampilkan();
</script>
</body>
</html>
