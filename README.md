# --<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>情人节</title>
    <style>
        *{
            margin: 0;
            padding: 0;
            list-style: none;
        }
        #time{
            color:red;
            font-size: 200px;
            text-align:center ;
            margin-top: 300px;
        }
        #pi{
            display: none;
            margin:300px auto;

        }
        body{
            background-color: black;
        }
        embed{
            margin:0 auto ;
        }

    </style>
</head>
<body>
<div id="time">5</div>
<img id="pi" src="13.gif" alt="" >

<audio autoplay="autoplay" controls="controls" preload="auto" src="http://111.208.73.42:83/2Q2W2CCFF9948B48B579A795CB9FCE40EEAE0706099E_unknown_9000DEC198831EC103EDC51B4848CC000BC5EAA7_1_111.208.25.232_83/jsdx.sc.chinaz.com/Files/DownLoad/sound1/201806/10294.mp3"></audio>
<script>

window.onload=function () {
    var i=7;
  var timer=  setInterval(function () {

    $('time').innerText-=1;
    if($('time').innerText==='0'){
        clearInterval(timer);
        $('time').style.display='none';
        $('pi').style.display='block';


    }


    },1000);
    var timer2=setInterval(function () {
        i-=1;
        console.log(i);

        if (i==0){
            clearInterval(timer2);
            $('pi').style.display='none';
            i=0;
        }

    },1000);



}
function $(id) {
    return typeof id==="string"?document.getElementById(id):null;

}
</script>
</body>
</html>
