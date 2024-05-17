<script>
  function getParam(get){
    var url_string = window.location.href.replace('#/', '');
    var url = new URL(url_string);
    var c = url.searchParams.get(get);
    console.log(c);
    return c;
  }
</script>

<div class="Item">
  {#if getParam('id') == 'nothingear'}
    <h2>สิ่งของ : Nothing Ear</h2>
      <img src="https://inwfile.com/s-cb/n1gnk1.jpg" alt="">
      <!-- owner,addtime,last see,last gps -->
      <p>
        เจ้าของ : นายพงศกร วิเศษธร
      </p>
      <p>
        วันที่เพิ่ม : <time datetime="2024-05-17">2024-05-17</time>
      </p>
      <p>
        วันที่อัพเดทล่าสุด : <time datetime="2024-05-17">2024-05-17</time>
      </p>
      <!-- button แจ้งหาย,อัปเดตที่อยู่ล่าสุด -->
      <p>
        <a href="https://www.facebook.com/profile.php?id=100009180981801">
          <button>แจ้งหาย</button>
        </a>
        <!-- <a href="https://www.facebook.com/profile.php?id=100009180981801">
          <button>อัปเดตที่อยู่ล่าสุด</button>
        </a> -->
      </p>
  {:else}
    <h2>{getParam('id')} ไอเทม : Fino</h2>
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
        <!-- <a href="https://www.facebook.com/profile.php?id=100009180981801">
          <button>อัปเดตที่อยู่ล่าสุด</button>
        </a> -->
    </p>
  {/if}
</div>
  