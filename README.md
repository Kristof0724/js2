# js2 
//alert('csáááááááááá');



console.log('hellóóóóó');
console.error('Hiba');
console.warn('lehet hiba');

//változók

//let,const,var
let kor =20;
kor = 21
//console.log(kor);


//adat típusok
const nev = 'Zsolt'; //string
const kor2 =21; //number
const suly = 80.5;
const felnott = false;// boolean
const date = new Date('2023-10-01');


const x = null;
let y = undefined;



console.log(typeof y);

//Műveletek

let szam1 = 10;
let eredmeny = szam1+=10
console.log(eredmeny);



var d = new Date();
var time = d.getHours();
var message = "Jó " + ((time<9)?"reggelt":"napot") + "!";
document.write(message);


if(time<9){
    document.write("<strong>Jó reggelt!</strong>")
}
else{
    document.write("Jó napot!")
}

function koszon(){
    var x = document.urlap1.nev.value;
    alert("Szia "+x+"!")
}

var ossz=0;
for(var i=1; i<=10; i++){
    ossz++;
}
document.write(ossz)

function figyelmeztet(){
    alert("Figyelmeztetve vagy")
}

function nevCsere(){
    document.getElementById("nev").value= "helyett péter";
}

function osszead(szam4,szam6){
    document.getElementById("szoveg").innerHTML=szam4 + szam6;
}

function kivon(szam4,szam6){
    document.getElementById("szoveg").innerHTML= szam4 - szam6;
}

function rahuz(elem) {
    elem.style.backgroundColor= "red";
}
function lehuz(elem) {
    elem.style.backgroundColor= "yellow";
}

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    
    <title>JavaScript</title>
</head>
<body>
    <h1>JavaScript Királyság</h1>
    <script src="main.js"> </script>
     <form name = "urlap1">
        Add meg a neved: <br>
        <input type="text" name="nev"><br>
        <input type="button" value="Köszönés" onclick="koszon()">
        <br>
        <br>
        <br>

        <input type="button" onclick="figyelmeztet()" value="Gomb">
       <br>
       <br>
        <p>A név beírása után kattints ki a bevitelimezőből</p>
        Írd ide a neved:<input type="text" id="nev" onchange="nevCsere()">
        <br>
       
        
      
    </form>    
    szam4:5 <br> szam6:3 <p id="szoveg"></p>
        <button id="gomb" onclick="osszead(5,3)" ondblclick="kivon(5,3)">Egy kattintással összead,kettővel kivon</button>

    <p>Húzd az egered a gombra</p>
    <button onmouseover="rahuz(this)" onmouseout="lehuz(this)"></button>
</body>
</html>
