<html lang="th">
<head>
    <meta charset="utf-8">
    <title>รักเค้ามั้ย</title>
    <style type="text/css">
        #main {
            text-align: center;
            padding-top: 50px;
        }
        #reject {
            position: relative;
            left: 0;
            top: 0;
            transition: all .1s ease-in-out;
        }
    </style>
</head>
<body>
    <div id="main">
        <h1>รักเค้ามั้ย :D</h1>
        <button id="accept">รัก</button>
        <button id="reject">ไม่รัก</button>
    </div>

    <script type="text/javascript">
        // ปุ่ม "รัก"
        document.getElementById("accept").addEventListener("click", function(event) {
            alert('เย้เธอรักเค้าที่สุด :D');
        });

        // ปุ่ม "ไม่รัก"
        document.getElementById("reject").addEventListener("mouseover", function(event) {
            var random_x = randomNumber(0, 300);
            var random_y = randomNumber(0, 300);

            this.style.left = random_x + "px";
            this.style.top = random_y + "px";
        });

        // ฟังก์ชันสุ่มตัวเลข
        function randomNumber(min, max) {
            return Math.floor(Math.random() * (max - min + 1)) + min;
        }
    </script>
</body>
</html>
