<style>
    body {
        font-family: Arial;
    }
    /* Style the tab */
    
    .tab {
        overflow: hidden;
        border: 1px solid #ccc;
        background-color: #f1f1f1;
    }
    /* Style the buttons inside the tab */
    
    .tab button {
        background-color: inherit;
        float: left;
        border: none;
        outline: none;
        cursor: pointer;
        padding: 14px 16px;
        transition: 0.3s;
        font-size: 17px;
    }
    /* Change background color of buttons on hover */
    
    .tab button:hover {
        background-color: #ddd;
    }
    /* Create an active/current tablink class */
    
    .tab button.active {
        background-color: #ccc;
    }
    /* Style the tab content */
    
    .tabcontent {
        display: none;
        padding: 6px 12px;
        border: 1px solid #ccc;
        border-top: none;
        font-size: 18px;
    }
    
    html {
        height: 100%;
    }
    
    body {
        background-image: url("http://web2.ctsh.hcc.edu.tw/stu101/s10111236/public_html/images/%E9%B5%9D%E9%91%BE%E9%BC%BB.jpg");
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-position: center;
        background-size: cover;
    }
    
    .smaller-image {
        width: 300px;
    }
    
    .bigger-image {
        width: 400px;
    }
    
    .smallest-image {
        width: 50px;
    }
    
    .image-position {
        width: 10px:
    }
    
    body {
        background-color: #CCFF99;
    }
    
    td {
        font-family: "微軟正黑體";
        font-size: 18px;
    }
    
    th {
        font-family: "微軟正黑體";
        font-size: 18px;
        font-weight: 900;
    }
    
    .button {
        background-color: #a0fdff;
        border: 2px solid black;
        color: #0645ad;
        padding: 8px 24px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        display: block;
    }
    
    .button:hover {
        background-color: #A1D0FF;
    }
    
    #flip {
        background-color: #a0fdff;
        border: 2px solid black;
        color: black;
        padding: 8px 42px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        display: block;
    }
    
    .button-bar {
        position: fixed;
        top: 5%;
        right: 5%;
    }
    
    * {
        box-sizing: border-box
    }
    
    body {
        font-family: Verdana, sans-serif;
        margin: 0
    }
    
    .mySlides {
        display: none
    }
    
    img {
        vertical-align: middle;
    }
    /* Slideshow container */
    
    .slideshow-container {
        max-width: 1000px;
        position: relative;
        margin: auto;
    }
    /* Next & previous buttons */
    
    .prev,
    .next {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: auto;
        padding: 16px;
        margin-top: -22px;
        color: white;
        font-weight: bold;
        font-size: 18px;
        transition: 0.6s ease;
        border-radius: 0 3px 3px 0;
        user-select: none;
    }
    /* Position the "next button" to the right */
    
    .next {
        right: 0;
        border-radius: 3px 0 0 3px;
    }
    /* On hover, add a black background color with a little bit see-through */
    
    .prev:hover,
    .next:hover {
        background-color: rgba(0, 0, 0, 0.8);
    }
    /* Caption text */
    
    .text {
        color: #f2f2f2;
        font-size: 15px;
        padding: 8px 12px;
        position: absolute;
        bottom: 8px;
        width: 100%;
        text-align: center;
    }
    /* Number text (1/3 etc) */
    
    .numbertext {
        color: #f2f2f2;
        font-size: 12px;
        padding: 8px 12px;
        position: absolute;
        top: 0;
    }
    /* The dots/bullets/indicators */
    
    .dot {
        cursor: pointer;
        height: 15px;
        width: 15px;
        margin: 0 2px;
        background-color: #bbb;
        border-radius: 50%;
        display: inline-block;
        transition: background-color 0.6s ease;
    }
    
    .active,
    .dot:hover {
        background-color: #717171;
    }
    /* Fading animation */
    
    .fade {
        -webkit-animation-name: fade;
        -webkit-animation-duration: 1.5s;
        animation-name: fade;
        animation-duration: 1.5s;
    }
    
    @-webkit-keyframes fade {
        from {
            opacity: .4
        }
        to {
            opacity: 1
        }
    }
    
    @keyframes fade {
        from {
            opacity: .4
        }
        to {
            opacity: 1
        }
    }
    /* On smaller screens, decrease text size */
    
    @media only screen and (max-width: 300px) {
        .prev,
        .next,
        .text {
            font-size: 11px
        }
    }
</style>
<html>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.0/jquery.min.js">
    </script>
    <script>
        $(document).ready(function() {
            $('#top').click(function() {
                $('html, body').animate({
                    scrollTop: 0
                }, 1000);
            });
            $('#bottom').click(function() {
                $('html, body').animate({
                    scrollTop: $(document).height() - $(window).height()
                }, 1000);
            });
            $('#a').click(function() {
                $('html, body').animate({
                    scrollTop: $("#A").offset().top
                }, 1000);
            });
            $('#b').click(function() {
                $('html, body').animate({
                    scrollTop: $("#B").offset().top
                }, 1000);
            });
            $('#c').click(function() {
                $('html, body').animate({
                    scrollTop: $("#C").offset().top
                }, 1000);
            });
            $('#d').click(function() {
                $('html, body').animate({
                    scrollTop: $("#D").offset().top
                }, 1000);
            });
            $('#e').click(function() {
                $('html, body').animate({
                    scrollTop: $("#E").offset().top
                }, 1000);
            });
            $('#f').click(function() {
                $('html, body').animate({
                    scrollTop: $("#F").offset().top
                }, 1000);
            });
            $("#flip").click(function() {
                $(".button").slideToggle("slow");
            });
        });
    </script>
</head>
<div id="google_translate_element"></div>

<script type="text/javascript">
    function googleTranslateElementInit() {
        new google.translate.TranslateElement({
            pageLanguage: 'zh-tw',
            layout: google.translate.TranslateElement.InlineLayout.SIMPLE
        }, 'google_translate_element');
    }
</script>

<script type="text/javascript" src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>

<div style="font-family:微軟正黑體">
    <h1 style="color: black; font-weight: bold;font-size:40px"><center>墾丁國家公園</center></h1>

    <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="A">基本資訊</h1>
    <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;font-size:18px;">
        <img style="width:300px;height:300px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Nanwan_%28South_Bay%29.jpg/426px-Nanwan_%28South_Bay%29.jpg" align="right"> 墾丁國家公園位於恆春半島南部，同時涵蓋陸域與海域面積共32,570.14公頃，成立於1984年1月，是我國第一座國家公園。其位置三面臨海，東面太平洋，南瀕巴士海峽，西鄰臺灣海峽，北接恆春縱谷平原、三台山、滿州市街，港口溪、九棚溪等。南北長約24公里，東西寬約24公里。 墾丁國家公園最具特色的海岸線，一向是國人最愛的旅遊聖地，由於百萬年來地殼運動使陸地與海洋深入交融，造就本區奇特的地理景觀，海面下的世界更是絢麗繽紛，種類繁多的魚種、多采多姿的珊瑚更是代表特色。生態方面，熱帶氣候蘊育出富有生命力的熱帶、海濱植物，每年秋冬眾多的過境候鳥，也讓這裡成為著名賞鳥聖地。此外，此區發現多處史前遺跡與原住民文化遺址，更是本區無價的人文資產。
    </div>

    <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="B">國家公園標誌意涵</h1>
    <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;font-size:18px;font-family:微軟正黑體">

        <p><img style="width:100px;height:100px" src="http://np.cpami.gov.tw/filesys/image/01_chinese/04_news/1logo.jpg" align="left"> 墾丁國家公園管理處處徽是由鵝鑾鼻方向遠眺大尖山所見的景觀藍天、白雲象徵著四季如春、晴朗的良好氣候尖聳的大尖山、蔚藍的海洋，代表著這是一座涵蓋陸地與海洋的國家公園。
        </p>

    </div>

    <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="C">公園特色介紹</h1>
    <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;">
        <div class="tab">
            <button class="tablinks" onclick="openCity(event, '自然生態')" id="defaultOpen">自然生態</button>
            <button class="tablinks" onclick="openCity(event, '觀光景點')">觀光景點</button>
            <button class="tablinks" onclick="openCity(event, '活動')">活動</button>
        </div>
        <div id="自然生態" class="tabcontent">
            <p>
                <gg style="font-weight:900">墾丁位處於熱帶，區內動植物種類豐富。至2014年，根據統計動物達5,164種，植物也有1,921種</gg>
                <br>
                <br>
                <gg style="font-weight:900">特有植物 :</gg>恆春半島的特有植物十分繁複。包括：瓜葉馬兜鈴、臺灣紅豆樹、鵝鑾鼻大戟、恆春鐵莧、南仁五月茶、恆春金線蓮、恆春石斑木等等近110種。
                <br>
                <gg style="font-weight:900;">海中生態：</gg>在恆春半島曾見的鯨豚類有大翅鯨、抹香鯨、吉氏海豚及黑身瓶鼻海豚。每年12月至翌年3月，在恆春西海岸之海口附近可見鯨類，而冬季時恆春半島各處沿海均可看到成群海豚。
                <br>
                <gg style="font-weight:900;">候鳥：</gg>由於墾丁位於台灣本島最南端，過境此區的候鳥種類眾多，其中最著名的有秋冬之際南下避寒的伯勞與灰面鷲，灰面鷲到達墾丁的時間常於十月十日前後，故又稱「國慶鳥」。 此外，墾丁北區的龍鑾潭也是境內水鳥聚集的地點，包括雁鴨與鷸鴴科鳥類均可發現。國家公園在此處設立龍鑾潭自然中心，擁有賞鳥的專業設施。
                <br>
            </p>
        </div>
        <div id="觀光景點" class="tabcontent">
            <p>
                <gg style="font-weight:900;">鵝鑾鼻燈塔：</gg>鵝鑾鼻燈塔是臺灣最南端的燈塔。塔身全白，為圓柱形，為白鐵製，塔高24.1公尺，塔頂換裝新式大型四等旋轉透鏡電燈，經過大型旋轉透鏡後，光力為1,800,000支燭光，每十秒一閃，照射距離達二十七點二浬，是目前臺灣光力最強的燈塔，被稱為「東亞之光」。<br>
                <gg style="font-weight:900;">墾丁國家森林遊樂區：</gg>全區遍布隆起珊瑚礁岩；植物共有1,200多種，分為椰子、油脂、橡膠、藥用、熱帶果樹等區，共有17處遊覽據點，其中以銀葉板根、仙洞、觀海樓、垂榕谷等較為出名。在仙洞、銀龍洞等天然石灰岩洞內，有各種石鐘乳及石筍，都是地下水中所溶蝕的碳酸鈣成份凝聚形成，成長緩慢，十分珍貴。<br>
                <gg style="font-weight:900;">社頂自然公園：</gg>園內並有豐富的動植物、石灰岩洞、以及珊瑚礁岩裂縫造成的「一線天」景觀。植物有329種以上，原生馬兜鈴科、芸香科、蘿科等蝴蝶食草植物大量分布，公園內有近50種蝴蝶，是觀賞及研究蝴蝶的理想地區。<br>
                <gg style="font-weight:900;">南灣：</gg>南灣是墾丁最負盛名的海灘之一，舊稱大坂埒。因海水湛藍，又稱做藍灣。此地沙灘長約600公尺，弧線美，沙質潔靜，在沙灘上經常有許多人進行游泳、日光浴、戲水等活動。本區漁產量豐富，時可見漁民使用地曳網（俗稱牽罟）作業的情形，每年4-7月虱目魚苗季可見到使用手抄網、塑膠筏捕捉魚苗，蔚為奇觀。近因觀光人潮眾多，已不復見。<br>
                <gg style="font-weight:900;">關山：</gg>關山山頂上有一座依珊瑚礁建造的廟宇，為台灣其他地區所罕見，因為主神是福德正神，故稱福德宮。宮外有一巨石，民間相傳是五百年前天外飛來的，故稱「飛來石」，又因為型似烏龜，被稱為「靈龜石」。從其組成及四週地形可知為隆起珊瑚礁經差異侵蝕而遺留，常為遊客攝影的好題材。<br>
                <gg style="font-weight:900;">船帆石：</gg>又稱「帆船石」，由墾丁往鵝鑾鼻方向，沿途可看到有一狀似帆船的珊瑚礁岩矗立於海中，看起來像是即將啟航的帆船，因而被稱為船帆石。由於從某一角度觀看像美國前總統尼克森的頭像，該石亦俗稱尼克森頭。<br>
                <gg style="font-weight:900;">瓊麻展示館：</gg>位於龍鑾潭南岸，佔地18公頃，館內有日據時期"台灣纖維株式會社"所留下的宿舍、神社拱門等遺跡，並有瓊麻製造廠房、曬麻場與加工機器等。<br>
                <gg style="font-weight:900;">佳樂水：</gg>佳樂水位於墾丁東海岸，原稱「高落水」、「佳落水」，是指該處有一瀑布。<br>
                <gg style="font-weight:900;">後壁湖港：</gg>後壁湖港設於民國61年間；為恆春半島上最具規模的漁港；其後又在民國80年設立觀光碼頭，碼頭內有玻璃船、遊艇等等設施，吸引許多觀光客前來遊玩；在後壁湖港亦有船班開往蘭嶼。<br>
            </p>
        </div>

        <div id="活動" class="tabcontent">
            <p>
                <gg style="font-weight:900;">墾丁大街 :</gg>夜間有夜市，為世界罕見設於國家公園內的商圈與夜市，加上大街的飯店、旅館、街頭小食、沙灘旁的水上機車，以及核能發電廠，所造成的光害、污染、水溫上升，影響國家公園的生態維護。<br>
                <gg style="font-weight:900;">墾丁風鈴季 :</gg>因墾丁秋冬之際落山風強勁，為平衡旅遊淡旺季之人潮，屏東縣政府於冬季開辦本活動，懸掛各式風鈴於主要景點。2006年最後一屆風鈴季結束後，不再舉辦。總計自2004－2006共三屆。<br>
                <gg style="font-weight:900;">春天吶喊 :</gg>每年春假期間（4月5日前後）舉行，吸引了大量的人潮。原意是參考1970年代美國Woodstock演唱之精神，提供創作音樂團體或個人發揮的舞台並帶動年輕族群愛、和平、自由...等精神。<br>
                <gg style="font-weight:900;">墾丁音樂季-戶外音樂活動 :</gg>近年由於商業行為的介入，周圍許多電音派對也隨之興起，甚至標榜女士著比基尼泳裝者免費入場。<br>
            </p>
        </div>

        <script>
            function openCity(evt, cityName) {
                var i, tabcontent, tablinks;
                tabcontent = document.getElementsByClassName("tabcontent");
                for (i = 0; i < tabcontent.length; i++) {
                    tabcontent[i].style.display = "none";
                }
                tablinks = document.getElementsByClassName("tablinks");
                for (i = 0; i < tablinks.length; i++) {
                    tablinks[i].className = tablinks[i].className.replace(" active", "");
                }
                document.getElementById(cityName).style.display = "block";
                evt.currentTarget.className += " active";
            }

            // Get the element with id="defaultOpen" and click on it
            document.getElementById("defaultOpen").click();
        </script>

        <p></p>
        <div class="slideshow-container">

            <div class="mySlides fade">
                <div class="numbertext">1 / 5</div>
                <img style="width:100%;height:400px" src="https://cdn2.ettoday.net/images/528/d528790.jpg">
                <div class="text"> 春浪</div>
            </div>

            <div class="mySlides fade">
                <div class="numbertext">2 / 5</div>
                <img style="width:100%;height:400px" src="http://mypaperimg.pchome.com.tw/newroot/t/p/tp1034/content/20030121/21/2116720.jpg">
                <div class="text"> 風鈴季</div>
            </div>

            <div class="mySlides fade">
                <div class="numbertext">3 / 5</div>
                <img style="width:100%;height:400px" src="https://tnimage.taiwannews.com.tw/photos/shares/5c8cbe627a7a3.png">
                <div class="text"> 音樂祭</div>
            </div>

            <div class="mySlides fade">
                <div class="numbertext">4 / 5</div>
                <img style="width:100%;height:400px" src="http://www.vrwalker.net/public/sceneryfiles/1415/1415_17154_1316518478.jpg">
                <div class="text"> 墾丁大街</div>
            </div>

            <div class="mySlides fade">
                <div class="numbertext">5 / 5</div>
                <img style="width:100%;height:400px" src="https://media-cdn.tripadvisor.com/media/photo-s/02/51/7a/77/plan-a-beach-vacation.jpg">
                <div class="text"> 墾丁青年活動中心</div>
            </div>

            <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
            <a class="next" onclick="plusSlides(1)">&#10095;</a>

        </div>
        <br>

        <div style="text-align:center">
            <span class="dot" onclick="currentSlide(1)"></span>
            <span class="dot" onclick="currentSlide(2)"></span>
            <span class="dot" onclick="currentSlide(3)"></span>
            <span class="dot" onclick="currentSlide(4)"></span>
            <span class="dot" onclick="currentSlide(5)"></span>
        </div>

        <script>
            var slideIndex = 1;
            showSlides(slideIndex);

            function plusSlides(n) {
                showSlides(slideIndex += n);
            }

            function currentSlide(n) {
                showSlides(slideIndex = n);
            }

            function showSlides(n) {
                var i;
                var slides = document.getElementsByClassName("mySlides");
                var dots = document.getElementsByClassName("dot");
                if (n > slides.length) {
                    slideIndex = 1
                }
                if (n < 1) {
                    slideIndex = slides.length
                }
                for (i = 0; i < slides.length; i++) {
                    slides[i].style.display = "none";
                }
                for (i = 0; i < dots.length; i++) {
                    dots[i].className = dots[i].className.replace(" active", "");
                }
                slides[slideIndex - 1].style.display = "block";
                dots[slideIndex - 1].className += " active";
            }
        </script>
    </div>
    
        <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="D">交通資訊</h1>
        <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;">
            <h3>♦ 自行開車:</h3>

            <h3>&nbsp;&nbsp;1. 可以多利用南二高到南州交流道下，順著指標直走到墾丁(從南州到墾丁沿途都有指標)。</h3>
            <h3>&nbsp;&nbsp;2. 高雄市區可由88快速道接二高從南州下。</h3>
            <h3>&nbsp;&nbsp;3. 也可以從中山高走到底，接17號省道往墾丁，不過比較塞，時間也比較久。</h3>
            <h3>&nbsp;&nbsp;4. 詳細交通路線，可以看我們特別繪製，然後一直被轉載的 墾丁對外交通路線圖 。</h3>

            <h3>♦ 客運：可以搭統聯或其他客運到高雄車站，再到車站前轉客運到墾丁。</h3>
            <h3>♦ 火車：坐火車高雄站，再轉客運到墾丁。</h3>
        </div>

        <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="E">住宿資訊</h1>
        <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;">
            <p>
                <table border="1" cellpadding="5" cellspacing="0" width="90%">

                    <thead>
                        <tr>
                            <th width="31%">酒店/旅館 </th>
                            <th width="48%">地址</th>
                            <th width="18%">電話</th>
                        </tr>
                    </thead>

                    <tbody>

                        <tr>
                            <td>夏都沙灘酒店</td>
                            <td>台灣恆春鎮墾丁路451號</td>
                            <td>08-8862345</td>
                        </tr>

                        <tr>
                            <td>漫步酒莊</td>
                            <td>台灣恆春鎮墾丁路石牛巷1-5號</td>
                            <td>08-8856886</td>
                        </tr>

                        <tr>
                            <td>墾丁凱撒大飯店</td>
                            <td>台灣恆春鎮墾丁路6號</td>
                            <td>08-8861888</td>
                        </tr>

                        <tr>
                            <td>墾丁福華渡假飯店</td>
                            <td>台灣恆春鎮墾丁路2號</td>
                            <td>08-8862323</td>
                        </tr>

                        <tr>
                            <td>承億文旅
                                <br>墾丁雅客小半島(恆春)</td>
                            <td>台灣恆春鎮墾丁路237、239號</td>
                            <td> 08-8861272</td>
                        </tr>

                    </tbody>
                </table>
            </p>
        </div>

        <h1 style="color: black; font-weight: bold;font-size:0.8cm" id="F">美食資訊</h1>
        <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;">
            <p>
                <table border="1" cellpadding="5" cellspacing="0" width="90%">

                    <thead>
                        <tr>
                            <th width="31%">店名</th>
                            <th width="48%">地址</th>
                            <th width="18%">電話</th>
                        </tr>
                    </thead>

                    <tbody>

                        <tr>
                            <td>搖滾披薩</td>
                            <td>台灣南灣路100號</td>
                            <td>08-8881535</td>
                        </tr>

                        <tr>
                            <td>巴沙諾瓦餐廳</td>
                            <td>台灣南灣路220號</td>
                            <td>08-8897137</td>
                        </tr>

                        <tr>
                            <td>墾丁街70活海產</td>
                            <td>台灣恆春鎮墾丁路70號</td>
                            <td>08-8862862</td>
                        </tr>

                        <tr>
                            <td>海饌活海鮮</td>
                            <td>台灣恆春鎮墾丁路70號</td>
                            <td>08-8861612</td>
                        </tr>

                        <tr>
                            <td>迷路小章魚餐酒館</td>
                            <td>台灣恆春鎮南灣里南灣路68號</td>
                            <td>08-8882822</td>
                        </tr>

                    </tbody>
                </table>
            </p>
        </div>

        <h1 style="color: black; font-weight: bold;font-size:0.8cm">參考資料</h1>
        <div style="background-color:#EEFFBB;border:2px black solid;padding:10px;">
            <a href="https://www.tripadvisor.com.tw/RestaurantsNear-g13806620-d553564-Kenting_National_Park-Hengchun_Pingtung.html"><h3>貓途鷹(美食)</h3></a>
            <a href="https://www.tripadvisor.com.tw/HotelsNear-g13806620-d553564-Kenting_National_Park-Hengchun_Pingtung.html"><h3>貓途鷹(住宿)</h3></a>
            <a href="https://zh.wikipedia.org/wiki/%E5%A2%BE%E4%B8%81%E5%9C%8B%E5%AE%B6%E5%85%AC%E5%9C%92#%E8%87%AA%E7%84%B6%E7%94%9F%E6%85%8B"><h3>維基百科</h3></a>
            <a href="http://np.cpami.gov.tw/youth/index.php?option=com_content&view=article&id=31&Itemid=6"><h3>台灣國家公園(墾丁國家公園)</h3></a>
            <a href="https://www.tjnp.gov.tw//chtNature/Environment/ShiDiXueXiao2.htm"><h3>台江國家公園(台江濕地學校)</h3></a>
            <a href="http://uukt.com.tw/traffic/how-to-go-kenting"><h3>悠遊墾丁</h3></a>
        </div>
</div>
<div class="button-bar">
    <a id="flip">選單</a>
    <a class="button" id="a" href="#">基本資訊</a>
    <a class="button" id="b" href="#">標示意涵</a>
    <a class="button" id="c" href="#">特色介紹</a>
    <a class="button" id="d" href="#">交通資訊</a>
    <a class="button" id="e" href="#">住宿資訊</a>
    <a class="button" id="f" href="#">美食資訊</a>
    <a class="button" id="top" href="#">網頁頂端</a>
    <a class="button" id="bottom" href="#">網頁底部</a>
    <a class="button" id="home" href="https://jim99224.github.io/HomePage/">返回主頁</a>
</div>

</html>
