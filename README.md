<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Change Text Cycle</title>
</head>
<body>

<h1 id="text">Hello World</h1>
<button id="btn">Change Contents</button>

<script>
    // ข้อความที่ต้องการให้แสดงวนไป
    const messages = [
        "Hello World",
        "Welcome",
        "This is JavaScript",
        "Learning is fun",
        "Back to start!"
    ];

    let index = 0; // เริ่มจากข้อความแรก

    document.getElementById("btn").addEventListener("click", function() {
        // เลื่อนไปข้อความถัดไป
        index++;

        // ถ้าถึงท้ายสุด ให้วนกลับไปเริ่มใหม่
        if (index >= messages.length) {
            index = 0;
        }

        // เปลี่ยนข้อความ
        document.getElementById("text").innerHTML = messages[index];

        // เปลี่ยนปุ่มตามสถานะ
        if (index === 0) {
            this.innerHTML = "Change Contents";
        } else if (index === messages.length - 1) {
            this.innerHTML = "Default Text";
        } else {
            this.innerHTML = "Next Text";
        }
    });
</script>

</body>
</html>
