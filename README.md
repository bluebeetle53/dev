<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
    <style>
      .card {
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    background-color: #f9f9f9;
    text-align: center;
    width: 300px;
    margin: 50px auto;
}


#rcorners9 {
  border-radius: 15px 50px 30px;
  background: #40E0D0;
  font-size: 20px;
  text-align: left;
  color: white;
  padding: 20px; 
  width: 200px;
  height: 8px; 
}


   .withdraw-button {
        display: inline-block;
        padding: 10px 20px;
        background-color: #007bff;
        color: #fff;
        float: right;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
        position: relative;
    }

    .withdraw-button i {
        margin-right: 10px;
    }

    .toast {
        display: none;
        position: fixed;
        bottom: 20px;
        left: 50%;
        transform: translateX(-50%);
        padding: 10px 20px;
        background-color: #333;
        color: #fff;
        border-radius: 5px;
        z-index: 9999;
    }






  .container5 {
        max-width: 800px;
        margin: 50px auto;
        padding: 20px;
        background-color: #fff;
        border-radius: 5px;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }
    h3 {
        color: #333;
    }
    p3 {
        color: #666;
        line-height: 1.6;
    }
    
    
    
    .fab {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: green;
  color: white;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  text-align: center;
  line-height: 50px;
  cursor: pointer;
}
    
    

    </style>
  
    
</head>
<body>
    <div class="container">
        <h1>Welcome to Digital Finance</h1>
    </div>
    
    <div class="rcorners9">
   <strong>    <p id="rcorners9"> Your Balance : ₦55,000</p> </strong>
    </div>
    
    <div class="card">
        <strong>New Generated account number</strong>
        <p> Bank : Stering Bank </p>
        <p> Account number : 8973582490 </p>
    </div>
    
    
    
    <script>
      // JavaScript to change card color every 2 seconds
const colors = ["blue", "red", "white"];
let index = 0;

function changeColor() {
    document.querySelector(".card").style.backgroundColor = colors[index];
    index = (index + 1) % colors.length;
}

setInterval(changeColor, 2000); // Change color every 2 seconds
    </script>
    
    
    
    
    
    <p>This website is the property of the Central Bank of Nigeria (CBN) to help citizens of Nigeria manage their finances, access important financial information, and stay informed about the latest economic developments in the country.</p>
    <p>Our mission is to promote a sound financial system in Nigeria that supports economic growth and development, ensures price stability, and fosters a stable and efficient financial sector.</p>
    
    
    <div class="fab" onclick="redirectToWhatsapp()">
      
  <i class="fa fa-share"></i>
</div>

<script>
function redirectToWhatsapp() {
  window.location.href = "https://api.whatsapp.com";
}
</script>
    
    
    
    
    
   <button class="withdraw-button" onclick="showToast()">
    <i class="fas fa-coins"></i> Withdraw
</button>

<div class="toast" id="toast">Minimum withdraw balance is ₦60,000. Kindly fund your account to withdraw.</div>

<script>
function showToast() {
    var toast = document.getElementById('toast');
    toast.style.display = 'block';
    setTimeout(function() {
        toast.style.display = 'none';
    }, 5000); // 5000 milliseconds = 5 seconds
}
</script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/js/all.min.js"></script>
    
    
</body>
</html>
