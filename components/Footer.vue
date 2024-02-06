<template>
  <div class="footer">
  <ul>
  <li><Icon style="font-size:5rem" name="material-symbols:calendar-month" color="white" /><span>予約</span>
  </li>
  <li><Icon style="font-size:5rem"  name="material-symbols:list-rounded" color="white" /><span>予定管理</span>
  </li>
  <li><Icon style="font-size:5rem"  name="material-symbols:person-rounded" color="white" /><span>マイページ</span>
  </li>
  <li><Icon style="font-size:5rem"  name="mdi:qrcode" color="white" /><span>会員証</span>
  </li>
  </ul>
</div>
</template>

<style>
.footer{
  background-color:#333;
  width:100%;
  height:auto;

}
.footer ul{
    display:flex;
  justify-content:space-around;
}
.footer ul li{
      display:flex;
    flex-direction:column;
    align-items:center;
}
</style>

<script>
export default defineAppConfig({
  nuxtIcon: {
    size: '24px',
  }
})
</script>