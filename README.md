# Icons-APP
Animated application icons 
<!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8">

  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Social Icons Hover Effect</title>

  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

  <link rel="stylesheet" href="styles.css"> <!-- استبدل هذا المسار بملف CSS الخاص بك -->

</head>

<body>

  <div class="wrapper">

    <a href="#" class="icon" style="--color: #E4405F;"><i class="fab fa-instagram"></i></a>

    <a href="#" class="icon" style="--color: #0A66C2;"><i class="fab fa-linkedin-in"></i></a>

    <a href="#" class="icon" style="--color: #FF0000;"><i class="fab fa-youtube"></i></a>

    <a href="#" class="icon" style="--color: #1DA1F2;"><i class="fab fa-twitter"></i></a>

    <a href="#" class="icon" style="--color: #25D366;"><i class="fab fa-whatsapp"></i></a>

  </div>
<style>
.wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2rem;
}

.icon {
  width: 5.625rem; /* تأكيد العرض */
  height: 5.625rem; /* تأكيد الارتفاع ليكون نفس العرض */
  background-color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  position: relative;
  text-decoration: none; /* إزالة الخط تحت الأيقونات */
  border-radius: 10px; /* إضافة حواف مستديرة للمربع */
  transition: box-shadow 0.3s ease, transform 0.3s ease; /* إضافة تأثيرات الانتقال */
}

.icon > i {
  font-size: 2rem; /* حجم الأيقونة */
  color: var(--color);
}

.icon:hover > i {
  scale: 1.2;
  color: #f1f1f1;
}

.icon:hover {
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); /* إضافة تأثير التوهج */
  transform: translateY(-5px); /* رفع المربع قليلاً عند التمرير */
}

.icon:before {
  background: var(--color);
  content: "";
  position: absolute;
  width: 130%;
  height: 130%;
  left: -110%;
  top: 80%;
  transform: rotate(45deg);
}

.icon:hover:before {
  animation: slide 0.7s forwards;
}

@keyframes slide {
  50% {
    left: -15%;
    top: 40%;
  }
  100% {
    left: -15%;
    top: -15%;
  }
}

</style>
</body>

</html>
