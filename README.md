# Bwebprogramiranje
-----------------------------------------------B01--CSS
body {
  background-color: rgb(180, 217, 235);
  font-family: Calibri;
}

* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

header {
  width: 100%;
  height: 60px;
}

h1 {
  color: rgb(43, 84, 128);
  margin-left: 40px;
}

nav {
  background-color: rgb(43, 84, 128);
  height: 41px;
  color: white;
}

.neaktivno {
  background-color: rgb(43, 84, 128);
  color: white;
  float: left;
  display: block;
  height: 40px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid white;
  border-right: 1px solid white;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.aktivno {
  background-color: rgb(130, 183, 208);
  color: white;
  float: left;
  display: block;
  height: 40px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #753a03;
  border-right: 1px solid #753a03;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

#desno {
  text-align: right;
  padding-right: 20px;
}

#kontejner {
  margin-top: 50px;
  width: 100%;
  display: flex;
  justify-content: center;
}

.galerija-content {
  margin-top: 20px;
  width: 640px;
  height: 640px;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

#opis {
  background-color: rgb(43, 84, 128);
  color: white;
  width: 640px;
  height: 104px;
  overflow: auto;
  padding: 4px;
  border: 3px solid white;
}


#glavna {
  width: 640px;
  height: 480px;
  border-top: 1px solid white;
  border-left: 2px solid white;
  border-right: 2px solid white;
  border-bottom: 4px solid white;
}

.mala {
  height: 40px;
  width: 64px;
  border: 2px solid white;
}

.male {
  display: flex;
  flex-direction: row;
  width: 640px;
  height: 40px;
  border: 1px solid white;
  margin-top: -6px;
}

#sadrzaj {
  clear:both;
  margin: auto;
  margin-top: 60px;
  background-color: rgb(43, 84, 128);
  color: white;
  width: 640px;
  height: 150px;
  border: 3px solid white;
}
----------------------------------------------pocetna
<body>

  <header>
    <h1>Фото галерија</h1>
    <nav>
      <a href="#" class="aktivno">Почетна</a>
      <a href="autor.html" class="neaktivno">О аутору</a>
      <a href="uputstvo.html" class="neaktivno">Упутство</a>
      <p id="desno">Завршни испит</p>
    </nav>
  </header>

  <form id="form1" runat="server">
    <div id="kontejner">
      <div class="galerija-content">
        <div id="opis">
          <asp:Label ID="Label1" Text="Седам чуда античког света је списак веома важних грађевина које је велики грчки историчар Херодот написао пре више од две хиљаде година. Има их седам јер је писао само о највећим структурама које је познавао. Није знао много о Азији и Америци. О овим древним чудима писали су и остали различити аутори у својим песмама и водичима. Седам чуда освојило је похвале због својих значајних карактеристика, у распону од врхунских највиших или највећих њихових типова, до уметности са којом су изведена. Њихове архитектонске и уметничке карактеристике опонашале су се широм хеленистичког света и шире. Значајан број авантуриста отпутовао је на стварна места да лично сведоче о чудима. Кружиле су легенде како би додатно употпуниле суперлативе чуда. Навођење седам најчудеснијих архитектонских и уметничких људских достигнућа наставило се и после старогрчких времена до Римског царства. Средњи век, ренесанса и у модерно доба. Међутим, од ових седам чуда још само комплекс великих пирамида у Гизи и дан данас постоји." runat="server"></asp:Label>
        </div>
        <div class="glavna">
          <asp:Image ID="glavna" runat="server" class="velika" ImageUrl="~/slike/slika1.jpg" />
        </div>
        <div class="male">
          <asp:ImageButton ID="ImageButton1" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika1.jpg" ToolTip="0" />
          <asp:ImageButton ID="ImageButton2" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika2.jpg" ToolTip="1" />
          <asp:ImageButton ID="ImageButton3" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika3.jpg" ToolTip="2" />
          <asp:ImageButton ID="ImageButton4" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika4.jpg" ToolTip="3" />
          <asp:ImageButton ID="ImageButton5" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika5.jpg" ToolTip="4" />
          <asp:ImageButton ID="ImageButton6" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika6.jpg" ToolTip="5" />
          <asp:ImageButton ID="ImageButton7" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika7.jpg" ToolTip="6" />
          <asp:ImageButton ID="ImageButton8" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika8.jpg" ToolTip="7" />
          <asp:ImageButton ID="ImageButton9" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika9.jpg" ToolTip="8" />
          <asp:ImageButton ID="ImageButton10" runat="server" OnClick="ImageButton_Click" CssClass="mala" ImageUrl="~/slike/slika10.jpg" ToolTip="9" />
        </div>
      </div>
    </div>
  </form>

</body>
-----------------------------------------------B02--CSS
body {
    background-image: url('../slike/pozadina.jpg');
    background-attachment: fixed;
    background-size: cover;
}

header {
  width: 100%;
  height: 60px;
}

h1,h2,p {
  color: #fefa99;
  font-family: Arial;
  text-shadow: 2px 2px 3px gray;
  text-align: center;
}

nav {
  height: 350px;
  width: 100%;
}

#centriraj {
  margin: auto;
  width: 460px;
}

.aktivno {
  background-color: #753a03;
  color: #fefa99;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #753a03;
  border-right: 1px solid #753a03;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.neaktivno {
  background-color: #fefa99;
  color: #753a03;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #753a03;
  border-right: 1px solid #753a03;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

footer {
  background: #753a03;
  color: #fefa99;
  text-align: center;
  height: 40px;
  padding-top: 12px;
}

img {
    width: 250px;
    height: 250px;
    border-radius: 50%;
    border: 3px solid rgb(243, 243, 157);
    float:left;
}

#slike {
  clear: left;
  padding-top: 30px;
  width: 1300px;
  min-width: 1255px;
  margin: auto;
  text-align:center;
}

#sadrzaj {
  clear: left;
  padding-top: 30px;
  width: 1300px;
  min-width: 1255px;
  margin: auto;
  text-align: center;
  background-color: #753a03;
}

footer {
  background-color: rgb(60, 24, 38);
  color: rgb(243, 243, 157);
  padding-top: 20px;
  padding-bottom: 20px;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
}
----------------------------------------------pocetna
<body>

  <header>
    <h1>ДОМАЋЕ ЖИВОТИЊЕ</h1>
    <nav>
      <div id="centriraj">
        <a id="tlink" href="index.html" class="aktivno">Почетна</a>
        <a href="autor.html" class="neaktivno">О аутору</a>
        <a href="uputstvo.html" class="neaktivno">Упутство</a>
      </div>
    </nav>
  </header>

  <div id="slike">
    <div id="konj">
      <img alt="Konj" src="slike/konj.jpg" onmouseover="Pusti('zkonj')" onmouseout="Zaustavi('zkonj')" onclick="Podaci('Konj')" />
    </div>
    <div id="koza">
      <img alt="Koza" src="slike/koza.jpg" onmouseover="Pusti('zkoza')" onmouseout="Zaustavi('zkoza')" onclick="Podaci('Koza')" />
    </div>
    <div id="krava">
      <img alt="Krava" src="slike/krava.jpg" onmouseover="Pusti('zkrava')" onmouseout="Zaustavi('zkrava')" onclick="Podaci('Krava')" />
    </div>
    <div id="ovca">
      <img alt="Ovca" src="slike/ovca.jpg" onmouseover="Pusti('zovca')" onmouseout="Zaustavi('zovca')" onclick="Podaci('Ovca')" />
    </div>
    <div id="petao">
      <img alt="Petao" src="slike/petao.jpg" onmouseover="Pusti('zpetao')" onmouseout="Zaustavi('zpetao')" onclick="Podaci('Petao')" />
    </div>
  </div>

  <footer>
    Copyright &copy; Предшколска Установа "Срећно дете"
  </footer>

  <audio id="zkonj">
    <source src="zvuk/konj.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zkoza">
    <source src="zvuk/koza.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zkrava">
    <source src="zvuk/krava.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zovca">
    <source src="zvuk/ovca.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zpetao">
    <source src="zvuk/petao.mp3" type="audio/mpeg" />
  </audio>

</body>
----------------------------------------------javascript
function Podaci(zivotinja) {
  var p = window.open('', '', 'width = 300,height = 200');
  if (zivotinja == 'Konj')
    p.document.write("<html><head><title>Домаће животиње</title></head><body><center><h1><b>ПАС<b></h1></center><p>Пас је најстарија домаћа животиња. Одaнa је човеку. Има добро развијено памћење и чуло мириса. Оглашава се лајањем.</p><body/></html>")
  else if (zivotinja == 'Koza')
    p.document.write("<html><head><title>Домаће животиње</title></head><body><center><h1><b>ПАС<b></h1></center><p>Пас је најстарија домаћа животиња. Одaнa је човеку. Има добро развијено памћење и чуло мириса. Оглашава се лајањем.</p><body/></html>")
  else if (zivotinja == 'Krava')
    p.document.write("<html><head><title>Домаће животиње</title></head><body><center><h1><b>ПАС<b></h1></center><p>Пас је најстарија домаћа животиња. Одaнa је човеку. Има добро развијено памћење и чуло мириса. Оглашава се лајањем.</p><body/></html>")
  else if (zivotinja == 'Ovca')
    p.document.write("<html><head><title>Домаће животиње</title></head><body><center><h1><b>ПАС<b></h1></center><p>Пас је најстарија домаћа животиња. Одaнa је човеку. Има добро развијено памћење и чуло мириса. Оглашава се лајањем.</p><body/></html>")
  else if (zivotinja == 'Petao')
    p.document.write("<html><head><title>Домаће животиње</title></head><body><center><h1><b>ПАС<b></h1></center><p>Пас је најстарија домаћа животиња. Одaнa је човеку. Има добро развијено памћење и чуло мириса. Оглашава се лајањем.</p><body/></html>")
}

function Pusti(zvuk) {
  var z = document.getElementById(zvuk);
  z.play();
}

function Zaustavi(zvuk) {
  var z = document.getElementById(zvuk);
  z.pause();
  z.currentTime = 0;
}
-----------------------------------------------B03--CSS
body {
  background-color: rgb(254 250 153);
  font-family: Calibri;
}

header {
  width: 100%;
  height: 70px;
}

h1 {
  color: #487f2e;
  text-align: center;
}

h2 {
  color: #487f2e;
}

p {
  color: #487f2e;
}

nav {
  height: 35px;
  width: 100%;
  background-color: #c4fea9;
}

#centriraj {
  margin: auto;
  width: 460px;
}

.aktivno {
  background: #487f2e;
  color: white;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #487f2e;
  border-right: 1px solid #487f2e;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.neaktivno {
  background: #c4fea9;
  color: #487f2e;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #487f2e;
  border-right: 1px solid #487f2e;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.zemlja {
  color: rgb(72, 127, 46);
  font-family: Arial;
}

#podnaslov1 {
  clear: both;
  text-align: center;
}

.container {
  display: flex;
  align-items: center;
  justify-content: center;
}


.uspravan {
  writing-mode: vertical-lr;
  text-orientation: upright;
  position: absolute;
  top: 250px;
  left: 250px;
  font-size: 40px;
  font-family: Arial;
  color: rgb(72, 127, 46);
  text-shadow: 2px 2px 10px rgb(72, 127, 46);
  letter-spacing: 10px;
}

.image {
  position: relative;
  max-width: 50%;
  margin: auto;
  margin-left: 460px;
}

.zastava {
  position: absolute;
  width: 40px;
  height: 20px;
}

#srb {
  position: absolute;
  left: 35%;
  top: 50%;
}

#rum {
  position: absolute;
  left: 70%;
  top: 10%;
}

#madj {
  position: absolute;
  top: 1%;
}

#hrv {
  position: absolute;
  left: -4%;
  top: 22%;
}

#mak {
  position: absolute;
  left: 55%;
  top: 90%;
}

#cg {
  position: absolute;
  left: 5%;
  top: 70%;
}

#bug {
  position: absolute;
  left: 85%;
  top: 80%;
}

#bih {
  position: absolute;
  left: -11%;
  top: 45%;
}

#alb {
  position: absolute;
  left: 20%;
  top: 90%;
}

footer {
  background-color: rgb(72, 127, 46);
  color: rgb(254, 250, 153);
  padding-top: 15px;
  padding-bottom: 15px;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
}

#f {
  width: 100%;
  height: 40px;
  position: absolute;
  top: 870px;
}
----------------------------------------------pocetna
<body>

  <header>
    <h1>ОСНОВНА ШКОЛА "СОЊА МАРИНКОВИЋ"</h1>
    <nav>
      <div id="centriraj">
        <a href="Pocetna.html" class="aktivno">Почетна</a>
        <a href="Autor.html" class="neaktivno">О аутору</a>
        <a href="Uputstvo.html" class="neaktivno">Упутство</a>
      </div>
    </nav>
</header>

  <center>
    <h2 id="podnaslov1">
      Србија и њени суседи
    </h2>
    <div class="container">
      <p class="uspravan">
        Географија
      </p>
      <div class="image">
        <div id="srb">
          <img class="zastava" alt="Srbija" src="slike/srpskaZastava.jpg" onmouseover="Pusti('hsrb')" onmouseout="Zaustavi('hsrb')" onclick="Podaci('Srbija')" /><br>
          <div class="zemlja">Србија</div>
        </div>
        <div id="rum">
          <img class="zastava" src="slike/rumunskaZastava.jpg" onmouseover="Pusti('hrum')" onmouseout="Zaustavi('hrum')" onclick="Podaci('Rumunija')" /><br>
          <div class="zemlja">Румунија</div>
        </div>
        <div id="madj">
          <img class="zastava" src="slike/madjarskaZastava.jpg" onmouseover="Pusti('hmadj')" onmouseout="Zaustavi('hmadj')" onclick="Podaci('Madjarska')" /><br>
          <div class="zemlja">Мађарска</div>
        </div>
        <div id="hrv">
          <img class="zastava" src="slike/hrvatskaZastava.jpg" onmouseover="Pusti('Hrvatska')" onmouseout="Zaustavi('Hrvatska')" onclick="Podaci('Hrvatska')" /><br>
          <div class="zemlja">Хрватска</div>
        </div>
        <div id="mak">
          <img class="zastava" src="slike/makedonskaZastava.jpg" onmouseover="Pusti('hmak')" onmouseout="Zaustavi('hmak')" onclick="Podaci('Makedonija')" /><br>
          <div class="zemlja">Македонија</div>
        </div>
        <div id="cg">
          <img class="zastava" src="slike/crnogorskaZastava.jpg" onmouseover="Pusti('hcg')" onmouseout="Zaustavi('hcg')" onclick="Podaci('Crna Gora')" /><br>
          <div class="zemlja">Црна Гора</div>
        </div>
        <div id="bug">
          <img class="zastava" src="slike/bugarskaZastava.jpg" onmouseover="Pusti('hbug')" onmouseout="Zaustavi('hbug')" onclick="Podaci('Bugarska')" /><br>
          <div class="zemlja">Бугарска</div>
        </div>
        <div id="bih">
          <img class="zastava" src="slike/bosanskaZastava.jpg" onmouseover="Pusti('hbih')" onmouseout="Zaustavi('hbih')" onclick="Podaci('Bosna i Hercegovina')" /><br>
          <div class="zemlja">Босна и Херцеговина</div>
        </div>
        <div id="alb">
          <img class="zastava" src="slike/albanskaZastava.jpg" onmouseover="Pusti('halb')" onmouseout="Zaustavi('halb')" onclick="Podaci('Albanija')" /><br>
          <div class="zemlja">Албанија</div>
        </div>
        <img id="karta" src="slike/karta.jpg" width="570px" height="662px" />
      </div>
    </div>
    <footer>
      Copyright &copy; Основна школа "Соња Маринковић"
    </footer>

    <div id="f">
    </div>

    <audio id="hsrb">
      <source src="zvuk/Serbia.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hrum">
      <source src="zvuk/Romania.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hbih">
      <source src="zvuk/BosniaHerzegovina.mp3" type="audio/mpeg" />
    </audio>
    <audio id="Hrvatska">
      <source src="zvuk/Croatia.mp3" type="audio/mpeg" />
    </audio>
    <audio id="halb">
      <source src="zvuk/Albania.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hbug">
      <source src="zvuk/Bulgaria.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hmadj">
      <source src="zvuk/Hungary.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hmak">
      <source src="zvuk/Macedonia.mp3" type="audio/mpeg" />
    </audio>
    <audio id="hcg">
      <source src="zvuk/Montenegro.mp3" type="audio/mpeg" />
    </audio>

  </center>
</body>
----------------------------------------------javascript
function Podaci(drzava) {
  var p = window.open('', '', 'width = 500,height = 300');
  if (drzava == 'Srbija')
    p.document.write("<html><head></head><body><h2>Србија<h2/><p>Главни град: Београд</p><p>Површина: 88.499 km²</p><p>Број становника: 6,834 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Rumunija')
    p.document.write("<html><head></head><body><h2>Румунија<h2/><p>Главни град: Букурешт</p><p>Површина: 238.397 km²</p><p>Број становника: 19,12 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Bugarska')
    p.document.write("<html><head></head><body><h2>Бугарска<h2/><p>Главни град: Софија</p><p>Површина: 110.994 km²</p><p>Број становника: 6,878 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Makedonija')
    p.document.write("<html><head></head><body><h2>Македонија<h2/><p>Главни град: Скопље</p><p>Површина:  25.713  km²</p><p>Број становника: 2,065 милиона (2021.))</p><body/></html>")
  else if (drzava == 'Madjarska')
    p.document.write("<html><head></head><body><h2>Мађарска<h2/><p>Главни град: Будимпешта</p><p>Површина: 93.025 km²</p><p>Број становника: 9,71 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Hrvatska')
    p.document.write("<html><head></head><body><h2Хрватска><h2/><p>Главни град: Загреб</p><p>Површина: 56.594 km²</p><p>Број становника: 3,899 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Albanija')
    p.document.write("<html><head></head><body><h2>Албанија<h2/><p>Главни град: Тирана</p><p>Површина: 28.748 km²</p><p>Број становника: 2,812 милиона (2021.)</p><body/></html>")
  else if (drzava == 'Bosna i Hercegovina')
    p.document.write("<html><head></head><body><h2>Босна и Херцеговина<h2/><p>Главни град: Сарајево</p><p>Површина: 51.209 km²</p><p>Број становника: 3,271  милиона (2021.)</p><body/></html>")
  else if (drzava == 'Crna Gora')
    p.document.write("<html><head></head><body><h2>Црна Гора<h2/><p>Главни град: Подгорица</p><p>Површина: 13.812 km²</p><p>Број становника: 619.211 (2021.)</p><body/></html>")
}

function Pusti(drzava) {
  var himna = document.getElementById(drzava);
  himna.play();
}

function Zaustavi(drzava) {
  var himna = document.getElementById(drzava);
  himna.pause();
  himna.currentTime = 0;
}
-----------------------------------------------B05--CSS
body {
  background-color: rgb(254 250 153);
  font-family: Calibri;
}

header {
  width: 100%;
  height: 70px;
}

h1 {
  color: #487f2e;
  text-align: center;
}

h2 {
  color: #487f2e;
}

p {
  color: #487f2e;
}

nav {
  height: 35px;
  width: 100%;
  background-color: #c4fea9;
}

#centriraj {
  margin: auto;
  width: 460px;
}

.aktivno {
  background: #487f2e;
  color: white;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #487f2e;
  border-right: 1px solid #487f2e;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.neaktivno {
  background: #c4fea9;
  color: #487f2e;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid #487f2e;
  border-right: 1px solid #487f2e;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.zemlja {
  color: rgb(72, 127, 46);
  font-family: Arial;
}

#podnaslov1 {
  clear: both;
  text-align: center;
}

#tabela {
  border: 1px solid;
  text-align: center;
  background-color: rgb(196, 254, 169);
}

.okvir {
  border: 1px solid;
  border-bottom: 1px inset rgb(199, 189, 189);
  border-right: 1px inset rgb(199, 189, 189);
}

td {
  font-size: 20px;
  text-align: center;
}

th {
  background-color: rgb(72, 127, 46);
  border: 1px solid;
  font-size: 14px;
  color: rgb(254, 250, 153);
  height: 40px;
  font-weight: 100;
  padding-left: 13px;
  padding-right: 13px;
}

img {
  width: 50px;
  height: 50px;
}

.slova {
  font-size: 12px;
  text-decoration: underline;
  display: block;
}

#podnaslov1 {
    text-align: center;
}

#podnaslov2 {
    text-align: center;
    top: 20%;
}

footer {
    background-color: rgb(72, 127, 46);
    color: rgb(254, 250, 153);
    padding-top: 15px;
    padding-bottom: 15px;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
}

#uspravan1 {
    writing-mode: vertical-lr;
    text-orientation: upright;
    position: absolute;
    top: 200px;
    left: 250px;
    font-size: 60px;
    font-family: Arial;
    color: rgb(72, 127, 46);
    text-shadow: 2px 2px 10px rgb(72, 127, 46);
    letter-spacing: 10px;
}
#uspravan2 {
    writing-mode: vertical-lr;
    text-orientation: upright;
    position: absolute;
    top: 200px;
    left: 320px;
    font-size: 60px;
    font-family: Arial;
    color: rgb(72, 127, 46);
    text-shadow: 2px 2px 10px rgb(72, 127, 46);
    letter-spacing: 10px;
}

    #f {
    width: 100%;
    height: 40px;
    position: absolute;
    top: 850px;
}

#sadrzaj {
  clear: both;
  margin: auto;
  margin-top: 60px;
  color: white;
  width: 640px;
  height: 150px;
}
----------------------------------------------pocetna
<body>
  <header>
    <h1>ОСНОВНА ШКОЛА "СОЊА МАРИНКОВИЋ"</h1>
    <nav>
      <div id="centriraj">
        <a href="index.html" class="aktivno">Почетна</a>
        <a href="Autor.html" class="neaktivno">О аутору</a>
        <a href="Uputstvo.html" class="neaktivno">Упутство</a>
      </div>
    </nav>
  </header>

  <center>
    <h2 id="podnaslov1">
      Звуци инструмената
    </h2>
    <p id="uspravan1">
      Музичка
    </p><br>
    <p id="uspravan2">
      култура
    </p>

    <div>
      <table id="tabela">
        <tr>
          <th>Назив инструмента</th>
          <th>Слика инструмента</th>
          <th>Звук инструмента</th>
        </tr>
        <tr>
          <td class="okvir">Гитара</td>
          <td class="okvir">
            <a href="https://sr.wikipedia.org/wiki/%D0%93%D0%B8%D1%82%D0%B0%D1%80%D0%B0/">
              <img alt="gitara" src="slike/Gitara.jpg" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukgitare')" onmouseout="Zaustavi('zvukgitare')" />
            <a class="slova" href="#" onclick="Podaci('Gitara')">Сазнај више</a>
          </td>
        </tr>
        <tr>
          <td class="okvir">Виолина</td>
          <td class="okvir">
            <a href="https://sr.m.wikipedia.org/sr-ec/%D0%92%D0%B8%D0%BE%D0%BB%D0%B8%D0%BD%D0%B0">
              <img alt="violina" src="slike/Violina.jpg" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukvioline')" onmouseout="Zaustavi('zvukvioline')" />
            <a class="slova" href="#" onclick="Podaci('Violina')">Сазнај више</a>
          </td>
        </tr>

        <tr>
          <td class="okvir">Клавир</td>
          <td class="okvir">
            <a href="https://sr.m.wikipedia.org/sr-ec/%D0%9A%D0%BB%D0%B0%D0%B2%D0%B8%D1%80">
              <img src="slike/Piano.jpg" alt="klavir" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukklavira')" onmouseout="Zaustavi('zvukklavira')" />
            <a class="slova" href="#" onclick="Podaci('Klavir')">Сазнај више</a>
          </td>
        </tr>

        <tr>
          <td class="okvir">Бубњеви</td>
          <td class="okvir">
            <a href="https://sr.wikipedia.org/sr-ec/%D0%91%D1%83%D0%B1%D1%9A%D0%B5%D0%B2%D0%B8">
              <img alt="bubnjevi" src="slike/Bubnjevi.jpg" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukbubnja')" onmouseout="Zaustavi('zvukbubnja')" />
            <a class="slova" href="#" onclick="Podaci('Bubnjevi')">Сазнај више</a>
          </td>
        </tr>

        <tr>
          <td class="okvir">Хармоника</td>
          <td class="okvir">
            <a href="https://sr.m.wikipedia.org/sr-ec/%D0%A5%D0%B0%D1%80%D0%BC%D0%BE%D0%BD%D0%B8%D0%BA%D0%B0">
              <img alt="harmonika" src="slike/Harmonika.jpg" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukharmonike')" onmouseout="Zaustavi('zvukharmonike')" />
            <a class="slova" href="#" onclick="Podaci('Harmonika')">Сазнај више</a>
          </td>
        </tr>

        <tr>
          <td class="okvir">Контрафагот</td>
          <td class="okvir">
            <a href="https://sr.m.wikipedia.org/sr-ec/%D0%9A%D0%BE%D0%BD%D1%82%D1%80%D0%B0%D1%84%D0%B0%D0%B3%D0%BE%D1%82">
              <img alt="kontrafagot" src="slike/Kontrafagot.jpg" />
            </a>
          </td>
          <td class="okvir">
            <img src="slike/zvucnik.jpg" onmouseover="Pusti('zvukkontrafagot')" onmouseout="Zaustavi('zvukkontrafagot')" />
            <a class="slova" href="#" onclick="Podaci('Kontrafagot')">Сазнај више</a>
          </td>
        </tr>
      </table>
    </div>
    <footer>
      Copyright &copy; Основна школа "Соња Маринковић"
    </footer>
  </center>

  <div id="f">
  </div>

  <audio id="zvukgitare">
    <source src="zvuk/gitara.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zvukvioline">
    <source src="zvuk/violina.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zvukbubnja">
    <source src="zvuk/bubnjevi.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zvukflaute">
    <source src="zvuk/flauta.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zvukklavira">
    <source src="zvuk/piano.mp3" type="audio/mpeg" />
  </audio>
  <audio id="zvukkontrafagot">
    <source src="zvuk/kontrafagot.wav" />
  </audio>
  <audio id="zvukharmonike">
    <source src="zvuk/harmonika.wav" />
  </audio>
</body>
----------------------------------------------javascript
function Pusti(zvuk) {
  document.getElementById(zvuk).play();
}
function Zaustavi(zvuk) {
  document.getElementById(zvuk).currentTime = 0;
}

function Podaci(instrument) {
  var p = window.open('', '', 'width = 300,height = 200');
  if (instrument == 'Gitara')
    p.document.write("<p>Инструменти код којих се звук производи треперењем његових жица.</p></center><body/></html>")
  else if (instrument == 'Violina')
    p.document.write("<html><head><title>Инструменти</title></head><body><center><h4><b>ГУДАЧКИ ИНСТРУМЕНТИ<b></h4><p>Добили су име због начина добијања тона: превлачење гудала преко жице изазива треперење жице и ствара тон. Гудачки инструменти имају четири жица различите дебљине.</p></center><body/></html>")
  else if (instrument == 'Klavir')
    p.document.write("<html><head><title>Инструменти</title></head><body><center><h4><b>ЖИЧАНИ ИНСТРУМЕНТИ СА ДИРКАМА<b></h4><p>Инструменти код којих се тон производи ударом филцем прекривеним чекићем о металну жицу.</p></center><body/></html>")
  else if (instrument == 'Bubnjevi')
    p.document.write("<html><head><title>Инструменти</title></head><body><center><h4><b>УДАРАЉКЕ<b></h4><p>Удараљке су по грађи најпримитивнији род музичких инструмената. Од прадавних времена па до данас оне су се јављале у различитим облицима и врстама у народној и уметничкој музици. Звук се добија ударом по звучном извору. Удара се руком (тамбурин), разним врстама палица (тимпани, гонг, звона, ксилофон и други), металном шипком (тријангл) или једном површином о другу (чинели, кастањете), ређе помоћу механизма (челеста).</p></center><body/></html>")
  else if (instrument == 'Harmonika')
    p.document.write("<html><head><title>Инструменти</title></head><body><center><h4><b>ЖИЧАНИ ИНСТРУМЕНТИ<b></h4><p>Инструменти код којих се звук производи треперењем његових жица.</p></center><body/></html>")
  else if (instrument == 'Kontrafagot')
    p.document.write("<html><head><title>Инструменти</title></head><body><center><h4><b>ДРВЕНИ ДУВАЧКИ ИНСТРУМЕНТИ<b></h4><p>Група музичких инструмената (познати и као аерофони инструменти од грч. αερο ваздух и φονος звук) код којих се звук производи дувањем, у већини случајева из уста и плућа свирача. Струјање ваздуха покреће на треперење језичке направљене од трске.</p></center><body/></html>")

  p.document.body.style.backgroundColor = "rgb(254 250 153)";
  p.document.body.style.color = "rgb(72, 127, 46)";
}
-----------------------------------------------B06--CSS
body {
  font-family: Calibri;
}

header {
  width: 100%;
  height: 70px;
  background-color: rgb(75, 108, 158);
}

h1 {
  color: rgb(233, 244, 242);
  margin-left:25px;
}

h2 {
  color: rgb(233, 244, 242);
}

p {
  color: rgb(233, 244, 242);
}

nav {
  height: 40px;
  width: 100%;
  background-color: rgb(58,79,99);
}

#centriraj {
  margin: auto;
  width: 460px;
}

.aktivno {
  background: rgb(70, 92, 113);
  color: rgb(233, 244, 242);
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid rgb(70, 92, 113);
  border-right: 1px solid rgb(70, 92, 113);
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

#GridView1, #Chart1 {
  background-color: white;
  width: 40%;
  margin-left: 20px;
  margin-top: 100px;
}

footer {
    background-color: rgb(177, 184, 183);
    color: dimgray;
    bottom: 0;
    position: fixed;
    left: 0;
    padding-top: 10px;
    width: 100%;
    text-align: center;
    font-size: 15px;
    border-top: 2px solid gray;
}
----------------------------------------------pocetna
<body>
  <header>
    <h1>Uspeh učenika</h1>
    <nav>
      <a href="Pocetna.aspx" class="aktivno">Početna</a>
      <a href="Grafika.aspx" class="aktivno">Grafika</a>
      <a href="Autor.html" class="aktivno">O autoru</a>
    </nav>
  </header>
    <form id="form1" runat="server">
        <div>
            <div>
                <asp:GridView ID="GridView1" runat="server" AutoGenerateColumns="False" DataSourceID="SqlDataSource1">
                    <Columns>
                        <asp:BoundField DataField="Razred" HeaderText="Razred" SortExpression="Razred" />
                        <asp:BoundField DataField="Odlican" HeaderText="Odlican" SortExpression="Odlican" />
                        <asp:BoundField DataField="Vrlodobar" HeaderText="Vrlodobar" SortExpression="Vrlodobar" />
                        <asp:BoundField DataField="Dobar" HeaderText="Dobar" SortExpression="Dobar" />
                        <asp:BoundField DataField="Dovoljan" HeaderText="Dovoljan" SortExpression="Dovoljan" />
                        <asp:BoundField DataField="Nedovoljan" HeaderText="Nedovoljan" SortExpression="Nedovoljan" />
                        <asp:BoundField DataField="ProsOcena" HeaderText="ProsOcena" SortExpression="ProsOcena" />
                    </Columns>
                </asp:GridView>

                <asp:SqlDataSource ID="SqlDataSource1" runat="server" ConnectionString="<%$ ConnectionStrings:SkolaConnectionString %>" ProviderName="<%$ ConnectionStrings:SkolaConnectionString.ProviderName %>" SelectCommand="SELECT * FROM [Uspeh] ORDER BY [ProsOcena]"></asp:SqlDataSource>
                 
            </div>
            <footer>
                &copy; Osnovna škola "Sonja Marinković"
            </footer>
        </div>
    </form>
</body>
-----------------------------------------------B08--CSS
body {
  font-family: Calibri;
}

header {
  width: 100%;
  height: 70px;
  background-color: rgb(75, 108, 158);
}

h1 {
  color: rgb(233, 244, 242);
  margin-left: 25px;
}

nav {
  height: 40px;
  width: 100%;
  background-color: rgb(58,79,99);
}

#sredina {
  clear:both;
  margin: 60px;
  width: 460px;
}

.aktivno {
  background: rgb(70, 92, 113);
  color: rgb(233, 244, 242);
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid rgb(70, 92, 113);
  border-right: 1px solid rgb(70, 92, 113);
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

#t2 {
    margin-left: 10px;
}

td {
    text-align: center;
}

footer {
    background-color: rgb(177, 184, 183);
    color: dimgray;
    bottom: 0;
    position: fixed;
    left: 0;
    padding-top: 10px;
    width: 100%;
    text-align: center;
    font-size: 15px;
    border-top: 2px solid gray;
}

#txtKomentar {
    width: 180px;
    height: 130px;
    margin-left: 20px;
}

#top {
    vertical-align: text-top;
}

#txtIme, #txtEmail {
    width: 150px;
}

#btnDodaj {
    text-align: center;
    width: 200px;
    margin-left: 35px;
}

.tekst {
    text-align: left;
    font-size: 20px;
    font-variant: small-caps;
}
----------------------------------------------pocetna
<body>
  <header>
    <h1>Uspeh učenika</h1>
    <nav>
      <a href="Pocetna.aspx" class="aktivno">Početna</a>
      <a href="Uputstvo.html" class="aktivno">uputstvo</a>
      <a href="Autor.html" class="aktivno">O autoru</a>
    </nav>
  </header>
    <form id="form1" runat="server">
        <div id="sredina">
            <table id="t2">
                <tr>
                    <td class="tekst">Ime:</td>
                    <td><asp:TextBox ID="txtIme" runat="server"></asp:TextBox></td>
                    <td></td>
                </tr>
                <tr>
                    <td class="tekst">Email:</td>
                    <td><asp:TextBox ID="txtEmail" runat="server"></asp:TextBox></td>
                    <td"></td>
                </tr>
                <tr>
                    <td class="tekst" id ="top">Komentar:</td>
                    <td><asp:TextBox ID="txtKomentar" runat="server" TextMode="MultiLine"></asp:TextBox></td>
                    <td></td>
                </tr>
                <tr>
                    <td>&nbsp;</td>
                    <td><asp:Button ID="btnDodaj" runat="server" Text="Dodaj komentar" OnClick="btnDodaj_Click" /></td>
                    <td>&nbsp;</td>
                </tr>
            </table>
            <p>
                <asp:Label ID="Label1" runat="server"></asp:Label>
            </p>

            <footer>
                &copy Muzej Srbije
            </footer>
        </div>
    </form>
</body>
-----------------------------------------------B012--CSS
body {
    background-image: url('../slike/pozadina.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

header {
  width: 100%;
  height: 70px;
}

h1 {
  color: orangered;
  font-family: Arial;
  text-shadow: 2px 2px 3px gray;
  font-size: 20px;
  text-align: center;
}

h2 {
  color: #487f2e;
}

p {
  color: #487f2e;
}

nav {
  height: 35px;
  width: 100%;
}

#centriraj {
  margin: auto;
  width: 460px;
}

.aktivno {
  background: orangered;
  color: white;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid orangered;
  border-right: 1px solid orangered;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

.neaktivno {
  background: white;
  color: blue;
  float: left;
  display: block;
  height: 30px;
  width: 150px;
  padding-top: 9px;
  border-left: 1px solid orangered;
  border-right: 1px solid orangered;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
}

#okvir {
  clear:both;
    padding-top: 10px;
    height: 600px;
    width: 550px;
    background-color: white;
    opacity: 0.8;
}

#mojIframe {
    border: 1px solid black;
}

footer {
    color: orangered;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
}
----------------------------------------------pocetna
<body>

  <header>
    <h1>Turistička agencija "Planinar"</h1>
    <nav>
      <div id="centriraj">
        <a href="Pocetna.html" class="aktivno">Početna</a>
        <a href="Autor.html" class="neaktivno">O autoru</a>
        <a href="Uputstvo.html" class="neaktivno">Uputstvo</a>
      </div>
    </nav>
  </header>

  <center>
    <div id="okvir">
      <p>
        Izaberite grad
        <select id="grad" onChange="prognoza()">
          <option value="1">Beograd</option>
          <option value="2">Nis</option>
          <option value="3">Jagodina</option>
          <option value="4">Zlatibor</option>
          <option value="5">Kosovska Mitrovica</option>
          <option value="6">Palic</option>
          <option value="7">Pirot</option>
          <option value="8">Ruma</option>
          <option value="9">Vrnjacka Banja</option>
          <option value="10">Subotica</option>
        </select>
      </p>
      <iframe id="mojIframe" src="https://naslovi.net/vremenska-prognoza" width="450" height="450"></iframe>
    </div>

    <footer>
      &copy; Turistička agencija "Planinar"
    </footer>
  </center>
</body>
----------------------------------------------javascript
function prognoza() {
        var p = window.open("", "", "width=250, height=200, left = 980, top = 250");
        var izbor = document.getElementById("grad").value;
        var a = document.getElementById("mojIframe");

    switch (izbor) {
        case "1":
                a.src = "https://naslovi.net/vremenska-prognoza/beograd";
                p.document.write("<html><head><title>Planinar | Obilazak</title></head><body><center><h2><b>Beograd<b></h2><p>Ovo je Beograd, glavni i najveci grad Srbije.</p></center><body/></html>"); break;
        case "2":       
                a.src = "https://naslovi.net/vremenska-prognoza/nis"; 
                p.document.write("<html><head><title>Planinar | Obilazak</title></head><body><center><h2><b>Niš<b></h2><p>Ovo je Nis, najveći grad u jugoistočnoj Srbiji i sedište Nišavskog upravnog okruga.</p></center><body/></html>"); break
        case "3":
                a.src = "https://naslovi.net/vremenska-prognoza/jagodina";
                p.document.write("<p>Ovo je Jagodina, grad i administrativni centar Pomoravskog okruga u centralnoj Srbiji. Smešten je na obali reke Belice, u geografskom regionu Šumadije.</p>"); break;
        case "4":
                a.src = "https://naslovi.net/vremenska-prognoza/zlatibor";
                p.document.write("<p>Ovo je Zlatibor, planina i park prirode u Srbiji koja se prostire na površini od oko 1.000 km², dugačka je 55 km, a široka i do 20 km.</p>"); break
        case "5":
                a.src = "https://naslovi.net/vremenska-prognoza/kosovska-mitrovica";
                p.document.write("<p>Ovo je Kosovska Mitrovica, radsko naselje i sedište istoimene opštine u Srbiji, koje se nalazi u severnom delu autonomne pokrajine Srbije Kosova i Metohije</p>"); break
        case "6":
                a.src = "https://naslovi.net/vremenska-prognoza/palic";
                p.document.write("<p>Ovo je Palic, gradsko naselje u Srbiji u gradu Subotici u Severnobačkom okrugu, izletište i lečilište, sedam kilometara udaljeno od Subotice</p>"); break
        case "7":
                a.src = "https://naslovi.net/vremenska-prognoza/pirot";
                p.document.write("<p>Ovo je Pirot, grad u Pirotskom okrugu. Prema popisu iz 2011. bilo je 57.928 stanovnika na teritoriji grada sa okolnim naseljima, dok je u samom gradu bilo 38.785 stanovnika</p>"); break
        case "8":
                a.src = "https://naslovi.net/vremenska-prognoza/ruma";
                p.document.write("<p>Ovo je Ruma, gradsko naselje u opštini Ruma, u Sremskom okrugu, u Srbiji. </p>"); break
        case "9":
                a.src = "https://naslovi.net/vremenska-prognoza/vrnjacka-banja";
                p.document.write("<p>Ovo je Vrnjacka Banja, gradsko naselje u Srbiji u opštini Vrnjačka Banja u Raškom okrugu. Ona je i najveća banja u Srbiji.</p>"); break
        case "10":
                a.src = "https://naslovi.net/vremenska-prognoza/subotica";
                p.document.write("<p>Ovo je Subotica, najseverniji grad u Srbiji, drugi po broju stanovnika u Vojvodini. </p>"); break

    }
    p.document.body.style.backgroundColor = "orangered";
}
-----------------------------------------------B021--CSS
html,
body {
    font-family: Arial;
}

a {
    font-size: 16px;
    color: white;
    margin-left: 20px;
}

#Zaglavlje {
    background: #264c73;
    color: white;
    width: 100%;
    height: 80px;
}

#Z1 {
    float: left;
    border-right: 1px solid white;
    height: 80px;
    width: 90px;
    font-size: 16px;
    padding: 30px;
}

#Z2 {
    float: left;
    height: 80px;
    font-size: 16px;
    padding: 30px;
    overflow: hidden;
}

#Sredina {
    clear: none;
    padding: 0;
    border: 1px solid #264c73;
}

#forma {
    width: 90%;
    margin: 5%;
}

#Podnozje {
    background: #264c73;
    color: white;
    width: 100%;
    height: 80px;
}

#P1 {
    float: left;
    height: 80px;
    width: 300px;
    font-size: 16px;
    padding: 30px;
}

#P2 {
    float: right;
    height: 80px;
    font-size: 16px;
    padding: 30px;
    text-align: right;
}

h2 {
    text-align: center;
}

hr {
    width: 90%;
}

table,
th,
td {
    border: 1px solid black;
    border-collapse: collapse;
}

table {
    width: 25%;
    margin: auto;
}

th {
    color: blueviolet;
    background-color: #d0d0d0;
    text-decoration: underline;
    cursor: pointer;
}

p {
    margin-left: 10%;
    margin-right: 10%;
}

#povratak {
    color: blue;
}
----------------------------------------------javascript
let pravac = -1; // pravac sortiranja (-1 uzlazno, 1 silazno)
        function sortiraj(x) {
            let tabela = document.getElementById("mojaTabela"); // pronalazimo tabelu
            let redovi = Array.from(tabela.rows).slice(1); // pravimo niz od redova i izbacujemo prvi red (zaglavlje sa tagom th)
            if (pravac < 0) { // sortiramo uzlazno
                Array.from(redovi)
                    .sort((a, b) => a.cells[x].textContent.localeCompare(b.cells[x].textContent))
                    .forEach(tr => tabela.appendChild(tr));
                pravac = 1;
            }
            else // sortiramo silazno
            {
                Array.from(redovi)
                    .sort((a, b) => b.cells[x].textContent.localeCompare(a.cells[x].textContent))
                    .forEach(tr => tabela.appendChild(tr));
                pravac = -1;
            }
        }
