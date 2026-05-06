<!-- ===================== index.html (Landing Page) ===================== -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Landing Page</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">Weblitooyy</a>
    <div>
      <a href="index.html" class="btn btn-outline-light btn-sm">Home</a>
      <a href="profile.html" class="btn btn-outline-light btn-sm">Profile</a>
      <a href="contact.html" class="btn btn-outline-light btn-sm">Contact</a>
    </div>
  </div>
</nav>

<div class="container text-center mt-5">
  <h1>Welcome to My Website</h1>
  <p class="lead">apa yaa</p>
  <button class="btn btn-primary" onclick="showAlert()">Klik Aku</button>
</div>

<script>
function showAlert() {
  alert("Halo! Selamat datang 😎");
}
</script>

</body>
</html>


<!-- ===================== profile.html ===================== -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Profile</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-dark bg-dark">
  <div class="container">
    <a href="index.html" class="btn btn-light btn-sm">Back</a>
  </div>
</nav>

<div class="container mt-5 text-center">
  <h2>Profile Saya</h2>
  <p>Nama: Felicita Suwondo</p>
  <p>Kelas: XI-D</p>

  <button class="btn btn-success" onclick="playGame()">Main Game</button>

  <p id="gameResult" class="mt-3"></p>
</div>

<script>
function playGame() {
  let angka = Math.floor(Math.random() * 10);
  document.getElementById("gameResult").innerText = "Angka random: " + angka;
}
</script>

</body>
</html>


<!-- ===================== contact.html ===================== -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-dark bg-dark">
  <div class="container">
    <a href="index.html" class="btn btn-light btn-sm">Back</a>
  </div>
</nav>

<div class="container mt-5">
  <h2>Contact Me</h2>
  <form onsubmit="return submitForm()">
    <div class="mb-3">
      <label class="form-label">Nama</label>
      <input type="text" class="form-control" id="nama" required>
    </div>
    <div class="mb-3">
      <label class="form-label">Pesan</label>
      <textarea class="form-control" id="pesan" required></textarea>
    </div>
    <button type="submit" class="btn btn-primary">Kirim</button>
  </form>
</div>

<script>
function submitForm() {
  alert("Pesan berhasil dikirim!");
  return false;
}
</script>

</body>
</html>
