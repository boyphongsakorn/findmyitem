<script>
  //get id from url params
  const id = new URLSearchParams(window.location.search).get("id");
</script>
  
  <div class="Item">
    <h2>{id} ไอเทม : Fino</h2>
    <img src="https://inwfile.com/s-cb/n1gnk1.jpg" alt="">
    <!-- owner,addtime,last see,last gps -->
    <p>
      ผู้ดูแล : <a href="https://www.facebook.com/profile.php?id=100009180981801">นายสมชาย สมบัติชัย</a>
    </p>
    <p>
      วันที่เพิ่ม : <time datetime="2019-01-01">2019-01-01</time>
    </p>
    <p>
      วันที่อัพเดทล่าสุด : <time datetime="2019-01-01">2019-01-01</time>
    </p>
    <!-- button แจ้งหาย,อัปเดตที่อยู่ล่าสุด -->
    <p>
      <a href="https://www.facebook.com/profile.php?id=100009180981801">
        <button>แจ้งหาย</button>
      </a>
      <a href="https://www.facebook.com/profile.php?id=100009180981801">
        <button>อัปเดตที่อยู่ล่าสุด</button>
      </a>
    </p>
  </div>  