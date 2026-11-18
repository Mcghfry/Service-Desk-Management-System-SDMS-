const guidance = {
  network: {
    title: 'Koneksi jaringan / Wi-Fi',
    steps: ['Pastikan Wi-Fi perangkat menyala dan mode pesawat tidak aktif.', 'Putuskan koneksi lalu sambungkan kembali ke jaringan yang benar.', 'Coba buka layanan dari perangkat lain untuk mengecek apakah gangguan terjadi pada jaringan atau perangkat.'],
    followup: 'Apakah perangkat lain juga mengalami gangguan yang sama?'
  },
  device: {
    title: 'Laptop atau komputer lambat',
    steps: ['Simpan pekerjaan yang sedang terbuka.', 'Tutup aplikasi yang tidak digunakan, lalu periksa apakah ruang penyimpanan hampir penuh.', 'Mulai ulang perangkat jika kondisinya aman dan tidak ada proses penting yang berjalan.'],
    followup: 'Apakah perangkat terasa lambat sejak dinyalakan atau setelah membuka aplikasi tertentu?'
  },
  account: {
    title: 'Masalah akun dan akses',
    steps: ['Pastikan nama pengguna dan alamat layanan sudah benar.', 'Periksa apakah Caps Lock aktif dan koneksi internet tersedia.', 'Gunakan proses reset kata sandi resmi jika tersedia. Jangan kirim kata sandi atau kode OTP kepada siapa pun.'],
    followup: 'Apakah muncul pesan kesalahan tertentu saat kamu mencoba masuk?'
  },
  software: {
    title: 'Aplikasi atau software',
    steps: ['Catat nama aplikasi dan pesan kesalahan yang tampil.', 'Tutup lalu buka kembali aplikasi, kemudian coba ulangi langkah yang memunculkan masalah.', 'Periksa apakah aplikasi lain juga terdampak sebelum melanjutkan troubleshooting.'],
    followup: 'Kapan masalah mulai terjadi dan apakah ada pesan kesalahan?'
  }
};

const form = document.getElementById('ticketForm');
const category = document.getElementById('issueCategory');
const detail = document.getElementById('issueDetail');
const assistantContent = document.getElementById('assistantContent');
const ticketDemo = document.getElementById('ticketDemo');
const ticketTitle = document.getElementById('ticketTitle');

function showGuidance(key, description) {
  const item = guidance[key];
  if (!item) return;
  assistantContent.replaceChildren();
  const response = document.createElement('div');
  response.className = 'assistant-response';
  const question = document.createElement('span');
  question.className = 'response-question';
  question.textContent = description || item.title;
  const answer = document.createElement('div');
  answer.className = 'response-answer';
  const avatar = document.createElement('span');
  avatar.className = 'assistant-avatar';
  avatar.textContent = '✳';
  const bubble = document.createElement('div');
  bubble.className = 'response-bubble';
  const heading = document.createElement('strong');
  heading.textContent = `Langkah awal · ${item.title}`;
  const list = document.createElement('ol');
  item.steps.forEach(step => {
    const li = document.createElement('li');
    li.textContent = step;
    list.append(li);
  });
  const followup = document.createElement('p');
  followup.className = 'response-followup';
  followup.textContent = item.followup;
  bubble.append(heading, list, followup);
  answer.append(avatar, bubble);
  const actions = document.createElement('div');
  actions.className = 'response-actions';
  const resolved = document.createElement('button');
  resolved.type = 'button';
  resolved.textContent = 'Sudah teratasi';
  resolved.addEventListener('click', () => {
    actions.replaceChildren();
    const note = document.createElement('span');
    note.className = 'form-hint';
    note.textContent = 'Bagus! Pada sistem lengkap, solusi ini akan dicatat sebagai bantuan mandiri.';
    actions.append(note);
  });
  const createTicket = document.createElement('button');
  createTicket.type = 'button';
  createTicket.textContent = 'Buat tiket teknisi';
  createTicket.addEventListener('click', createDemoTicket);
  actions.append(resolved, createTicket);
  response.append(question, answer, actions);
  assistantContent.append(response);
}

function createDemoTicket() {
  const item = guidance[category.value] || guidance.network;
  ticketTitle.textContent = item.title;
  ticketDemo.hidden = false;
  ticketDemo.scrollIntoView({ behavior: 'smooth', block: 'center' });
}

form.addEventListener('submit', event => {
  event.preventDefault();
  const key = category.value;
  if (!key) return;
  showGuidance(key, detail.value.trim() || guidance[key].title);
});

document.querySelectorAll('.suggestion-chips button').forEach(button => {
  button.addEventListener('click', () => {
    const key = button.dataset.category;
    category.value = key;
    detail.value = button.textContent;
    showGuidance(key, button.textContent);
  });
});

document.getElementById('reopenTicket').addEventListener('click', event => {
  const button = event.currentTarget;
  button.textContent = button.textContent === 'Buka ulang tiket' ? 'Tiket dibuka ulang' : 'Buka ulang tiket';
  button.classList.toggle('reopened');
});

const menuToggle = document.getElementById('menuToggle');
const mainNav = document.getElementById('mainNav');
menuToggle.addEventListener('click', () => {
  const expanded = menuToggle.getAttribute('aria-expanded') === 'true';
  menuToggle.setAttribute('aria-expanded', String(!expanded));
  mainNav.classList.toggle('open', !expanded);
});
mainNav.querySelectorAll('a').forEach(link => link.addEventListener('click', () => {
  mainNav.classList.remove('open');
  menuToggle.setAttribute('aria-expanded', 'false');
}));
