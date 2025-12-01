# Holiday-Tours-And-Travels

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HOLIDAY TOURS AND TRAVELS</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}
body{background:#f4f6f8;color:#222;}

/* HEADER */
header{
  height:90vh;
  background:url('https://images.unsplash.com/1600267185393-e6ec8b85adba') center/cover;
  position:relative;
  display:flex;
  justify-content:center;
  align-items:center;
}
header::after{
  content:"";
  position:absolute;
  inset:0;
  background:rgba(0,0,0,.65);
}
.hero{
  position:relative;
  color:#fff;
  text-align:center;
  max-width:650px;
}
.hero h1{font-size:3rem;}
.hero button{
  margin-top:20px;
  padding:12px 30px;
  background:#ff9800;
  border:none;
  color:white;
  font-weight:bold;
  cursor:pointer;
  border-radius:5px;
}

/* SECTIONS */
section{padding:70px 10%;}
.about,.packages,.contact{
  background:white;
  margin-top:25px;
  padding:40px;
  border-radius:8px;
}

/* PACKAGES */
.packages-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:20px;
}
.card{
  box-shadow:0 5px 15px rgba(0,0,0,.1);
  border-radius:8px;
  overflow:hidden;
}
.card img{width:100%;height:180px;object-fit:cover;}
.card div{padding:15px;}

/* FORM */
form{max-width:500px;margin:auto;display:grid;gap:15px;}
input,textarea{
  padding:10px;
  border:1px solid #ccc;
  border-radius:5px;
  width:100%;
}
button{
  padding:12px;
  background:#111;
  color:white;
  border:none;
  cursor:pointer;
}

/* FOOTER */
footer{
  background:#111;
  color:#aaa;
  text-align:center;
  padding:15px;
  margin-top:30px;
}
</style>
</head>

<body>

<header>
  <div class="hero">
    <h1>HOLIDAY TOURS AND TRAVELS</h1>
    <p>Your trusted travel partner worldwide</p>
    <button>Book Now</button>
  </div>
</header>

<section class="about">
<h2>About Us</h2>
<p>
HOLIDAY TOURS AND TRAVELS provides professional travel services including:
Hotels, Cab Booking, Group Tours, Honeymoon Packages, International Tours.
</p>
</s
