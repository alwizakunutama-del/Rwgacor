<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Alwizz Market</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #222;
    color: #fff;
    text-align: center;
    padding: 20px;
  }
  .logo {
    width: 150px;
    margin-bottom: 20px;
  }
  .button {
    padding: 15px 30px;
    font-size: 18px;
    margin: 10px;
    cursor: pointer;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 8px;
  }
  .button.off {
    background-color: #f44336;
  }
  .footer {
    margin-top: 30px;
  }
  .update-btn {
    padding: 10px 20px;
    background-color: #008CBA;
    color: white;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    margin-bottom: 10px;
  }
</style>
</head>
<body>

<!-- Logo yang Anda kirimkan -->
<img src="https://your-logo-url.com/logo.png" alt="Logo" class="logo" />

<!-- Permintaan izin VPN saat masuk -->
<h2>Mohon izin untuk mengaktifkan VPN</h2>
<button class="button" onclick="requestVPN()">Izinkan VPN</button>

<!-- Tombol RW MUSUH GAMPANG -->
<h3>RW MUSUH GAMPANG</h3>
<button id="vpnToggle" class="button off" onclick="toggleVPN()">Matikan</button>

<!-- Tombol update -->
<div class="footer">
  <button class="update-btn" onclick="window.location.href='https://wa.me/628229VbAsKVFF6sn6f2Fvu51'">Update</button>
  <p>by AlwizzTeamX</p>
</div>

<script>
  let vpnActive = false;

  function requestVPN() {
    alert("Izin VPN diberikan. Silakan tekan tombol VPN untuk mengaktifkan.");
  }

  function toggleVPN() {
    const btn = document.getElementById("vpnToggle");
    if (!vpnActive) {
      // Aktifkan VPN ke negara Kamboja
      // Di sini Anda harus mengintegrasikan API VPN Anda
      // Contoh: panggil API VPN untuk mengubah lokasi
      // fetch('API_VPN_URL', {...})
      alert("VPN Negara Kamboja diaktifkan");
      vpnActive = true;
      btn.textContent = "Hentikan";
      btn.classList.remove("off");
    } else {
      // Matikan VPN
      // fetch('API_VPN_URL', {...})
      alert("VPN dimatikan");
      vpnActive = false;
      btn.textContent = "Nyalakan";
      btn.classList.add("off");
    }
  }
</script>

</body>
</html>
