# zqw
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Js</title>
    <style>
        .div1{
            margin-left: 425px;
            margin-top: 200px;
            position: absolute;
        }
        .div2{
            display: none;
            margin-left: 890px;
            margin-top: 300px;
            width: 300px;
            height: 300px;
            border: groove;
            background-color: violet;
            position: fixed;
        }

    </style>
</head>
<body>
<div  class="div1">
<button id = "click" style="width: 200px;height: 40px;background-color: plum;font-style: inherit;margin-left: 150px;">点击这里修改div的格式！</button><br>
<br />
    <div id = "div" style="width: 350px;height: 350px;background-color: #67b168;margin-left: 70px" >
</div>
</div>

<div    id = "div2" class = "div2">
    <br>
    <strong   style="margin-left: 10px;color: black">请选择颜色：</strong><br >
    <button   id ="red"   style="width: 30px;height:30px;border:1px;background-color: red ;margin-left: 10px">红</button>
    <button id = "yellow"  style="width: 30px;height:30px;border:1px;background-color: yellow;margin-left: 28px;">黄</button>
    <button id = "blue"  style="width: 30px;height:30px;border:1px;background-color: blue;margin-left: 30px;">蓝</button>
    <br ><br >
    <strong   style="margin-left: 10px;color: black">请选择长度：</strong><br >
    <button   id ="200w"   style="width: 30px;height:30px;border:1px;background-color:deepskyblue;margin-left: 10px"  value="200px" >200</button>
    <button   id ="400w"   style="width: 30px;height:30px;border:1px;background-color: deepskyblue;margin-left: 10px"  value="400px" >400</button>
    <button   id ="600w"   style="width: 30px;height:30px;border:1px;background-color:deepskyblue;margin-left: 10px"  value="400px" >400</button>
    <br ><br>
    <strong   style="margin-left: 10px;color: black;">请选择宽度：</strong><br >
    <button   id ="200h"   style="width: 30px;height:30px;border:1px;background-color:deepskyblue;margin-left: 10px">200</button>
    <button id = "400h"  style="width: 30px;height:30px;border:1px;background-color:deepskyblue;margin-left: 10px">400</button>
    <button  id = "600h" style="width: 30px;height:30px;border:1px;background-color:deepskyblue;margin-left: 10px ">600</button>
    <br >
    <br>
    <input  type="button"   id="recover" value="恢复"  style="background-color:mediumspringgreen;margin-left: 30px;"/>
    <input  type="button"   id="yes" value ="确定"  style="background-color:mediumspringgreen;margin-left: 126px"/>
</div>
<script>
    document.getElementById('click').onclick = click;
    document.getElementById('red').onclick = red;
    document.getElementById('yellow').onclick = yellow;
    document.getElementById('blue').onclick = blue;
    document.getElementById('200w').onclick = w2;
    document.getElementById('400w').onclick = w4;
    document.getElementById('600w').onclick = w6;
    document.getElementById('200h').onclick = h2;
    document.getElementById('400h').onclick = h4;
    document.getElementById('600h').onclick = h6;
    document.getElementById('recover').onclick = recover;
    document.getElementById('yes').onclick = yes;

    function click() {
        div2.style.display = 'block ';
    }
    function red() {
        div.style.backgroundColor = 'red';
    }
    function yellow() {
        div.style.backgroundColor = 'yellow';
    }
    function blue() {
        div.style.backgroundColor = 'blue';
    }
    function w2() {
        div.style.width = '200px';
    }
    function w4() {
        div.style.width = '400px';
    }
    function w6() {
        div.style.width = '600px';
    }
    function h2() {
        div.style.height = '200px';
    }
    function h4() {
        div.style.height= '400px';
    }
    function h6() {
        div.style.height = '600px';
    }
    function recover() {
        div.style.backgroundColor = '#67b168';
        div.style.width = '350px';
        div.style.height = '350px';
    }
    function yes() {
        div2.style.display = 'none';
    }
</script>
</body>
</html>
