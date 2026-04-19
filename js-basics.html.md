<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JS基础知识练习作业</title>
</head>
<body>
    <h1>JS基础知识练习作业</h1>
    <p>请按F12打开浏览器控制台，查看运行结果</p >

    <script>
        var username = "你的名字";
        console.log("var 变量：", username);

        let age = 20;
        console.log("let 变量（初始值）：", age);
        age = 21;
        console.log("let 变量（修改后）：", age);

        const PI = 3.14159;
        console.log("const 常量：", PI);

        let str = "Hello, JavaScript!";
        let num = 100;
        let isStudent = true;
        let hobbies = ["看书", "画画", "敲代码"];
        let student = { name: "你的名字", age: 20, grade: "大二" };
        let undef;
        let empty = null;

        console.log("字符串：", str, "| 类型：", typeof str);
        console.log("数字：", num, "| 类型：", typeof num);
        console.log("布尔值：", isStudent, "| 类型：", typeof isStudent);
        console.log("数组：", hobbies, "| 类型：", typeof hobbies);
        console.log("对象：", student, "| 类型：", typeof student);
        console.log("undefined：", undef, "| 类型：", typeof undef);
        console.log("null：", empty, "| 类型：", typeof empty);

        let a = 10;
        let b = 3;
        let add = a + b;
        let sub = a - b;
        let mul = a * b;
        let div = a / b;
        let mod = a % b;
        console.log("算术表达式结果：", add, sub, mul, div.toFixed(2), mod);

        let isEqual = a == b;
        let isBigger = a > b;
        console.log("比较表达式结果：", isEqual, isBigger);

        let andResult = (a > 5) && (b < 5);
        let orResult = (a > 15) || (b < 5);
        console.log("逻辑表达式结果：", andResult, orResult);

        let score = 85;
        if (score >= 90) {
            console.log("成绩等级：优秀");
        } else if (score >= 60) {
            console.log("成绩等级：及格");
        } else {
            console.log("成绩等级：不及格");
        }

        console.log("循环遍历数组：");
        for (let i = 0; i < hobbies.length; i++) {
            console.log("第" + (i+1) + "个爱好：" + hobbies[i]);
        }

        function greet(name) {
            return "你好，" + name + "！欢迎学习JavaScript~";
        }

        function calcAverage(score1, score2, score3) {
            let average = (score1 + score2 + score3) / 3;
            return average.toFixed(1);
        }

        let greetMsg = greet("你的名字");
        let avgScore = calcAverage(88, 92, 79);
        console.log("函数调用结果：", greetMsg);
        console.log("平均分：", avgScore);
    </script>
</body>
</html>
