<template>
  <div class="CompHome">
    <header>
      <div class="thongBao">
        <p>{{mgs}}</p>
      </div>
      <div class="iconHeader">
        <i class="fa-solid fa-bell"></i>
        <i class="fa-solid fa-gear"></i>
      </div>
    </header>

    <main>
      <div class="infoAndMenu">
        <div class="infoUser">
          <div class="avatar">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/9/99/Sample_User_Icon.png"
              alt=""
            />
          </div>
          <div class="userName">
            <h3>{{ userName }}</h3>
          </div>
        </div>
        <div class="menu">
          <div class="point">
            <i class="fa-regular fa-gem"></i> <span>{{point}}</span>
          </div>
          <div class="menuItem">
            <ul>
                <li>
                    <i class="fa-solid fa-wallet"></i>
                    <p>Tài sản</p>
                </li>
                <li>
                    <i class="fa-solid fa-user-shield"></i>
                    <p>Đội ngũ</p>
                </li>
                <li>
                    <i class="fa-solid fa-building-columns"></i>
                    <p>Ngân hàng</p>
                </li>
                <li>
                    <i class="fa-solid fa-clipboard"></i>
                    <p>Lịch sử</p>
                </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="soDuUSDT mainItem">
        <h4>Số dư USDT:</h4>
        <br />
        <p>USDT</p>
        <p>******</p>
      </div>
      <div class="soDuVND mainItem">
        <h4>Số dư VND:</h4>
        <br />
        <p>VND</p>
        <p>******</p>
      </div>
      <div class="giaoDich mainItem">
        <h4>Giao dịch gần nhất:</h4>
        <br />
        <h5>Ngày xx giờ xx ></h5>
        <p>Số lượng giao dịch:</p>
        <p>xxUSDT Hoàn Thành</p>
      </div>
    </main>

    <footer>
      <i class="fa-solid fa-house"></i>
      <i class="fa-solid fa-credit-card"></i>
      <i class="fa-solid fa-shield-halved"></i>
      <i class="fa-solid fa-user"></i>
    </footer>
  </div>
</template>

<script>
import "../static/fontawesome-free-6.4.0-web/css/all.min.css";

export default {
  name: "CompHome",
  data() {
    return {
        userName: 'Nguyễn Văn A',
        mgs:"Thông báo trạng thái",
        point: 125
    };
  },
};
</script>

<style>
.CompHome {
  margin: 30px 30px;
  width: 300px;
  height: 580px;
  background-color: #f2f8f4;
  border-radius: 8px;
  position: relative;
}
header {
  height: 50px;
  width: 100%;
  background-color: #6fdfb1;
}

.thongBao {
  width: 75%;
  display: inline-block;
}

.thongBao p {
  height: 26px;
  line-height: 26px;
  padding-left: 4px;
  margin-top: 10px;
  margin-left: 10px;
  background-color: #f2f8f4;
  border-radius: 14px;
  color: gray;
  font-size: 10px;
}

.iconHeader {
  width: 25%;
  display: inline-block;
}

.iconHeader i {
  margin: 0 8px;
}

.infoAndMenu {
  padding-bottom: 4px;
  margin-bottom: 10px;
  background-color: #6fdfb1;
}

.mainItem {
  background-color: #c4e4d6;
  border-radius: 6px;
  margin: 0 12px 10px 12px;
  padding: 8px;
}

.infoUser {
  display: flex;
  height: 60px;
  margin: 0 12px 10px 12px;
}

.avatar {
  width: 25%;
  height: 100%;
  display: inline-block;
  background-color: #f2f8f4;
  border-radius: 50%;
}

.avatar img {
  width: 100%;
  height: 100%;
}

.userName {
  line-height: 60px;
  padding-left: 12px;
  width: 75%;
  height: 100%;
  display: inline-block;
}
.menu {
  margin: 0 12px 10px 12px;
  background-color: white;
  padding: 8px;
  border-radius: 8px;
}
.menuItem ul {
    padding-top: 16px;
    list-style: none;
}
.menuItem ul li {
    text-align: center;
    width: 25%;
    display: inline-block;
}

.menuItem ul p {
    padding-top: 8px;
    font-size: 11px;
}

.giaoDich p {
  color: gray;
  font-size: 12px;
}

footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 40px;
  background-color: #e8edea;
}
footer i {
  display: inline-block;
  width: 25%;
  height: 40px;
  text-align: center;
  padding-top: 10px;
}
footer i:hover {
  cursor: pointer;
  background-color: #6fdfb1;
}
</style>
