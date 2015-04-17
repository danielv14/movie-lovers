#MovieLovers
Detta är ett repo för en hemsidan som är del av en kurs, [Webbinformatik 2.0, 7ph](https://www.miun.se/utbildning/kurser/data-och-it/informatik/informatik-gr-a-webbinformatik-2.0-75-hp/om-kursen).
Uppgift 3 handlar om att skapa en enklare statisk hemsida där själva innehållet är oväsentligt, så länge hemsidan uppfyller vissa kriterier. Bland annat är navbar ett krav samt  att det ska finnas några externa länkar på hemsidan.

##Animate.css, normalize.css, wow.js och jquery
Normalize används för att nollställa all margin och padding. De andra två externa filer används för att skapa den effekt som finns i sign-up.php och möjliggör den effekt som finns på sidans andra wrapper. Då wow.js använder sig av jquery finns även jquery i js/jquery-2.1.3.min.js 

##Icke använda .js filer
js/main.js är en (än så länge) tom fil där eventuell egen javascript/jquery kod kan skrivas för använding på MovieLovers.
js/typed.js är en externt hämtad fil som inte heller används i nuläget.

##Användande av div-wrapper
Allt innehåll ska omslutas av en div med klassen 'wrapper'. Då blir innehållet centrerat och style'at på ett visst sätt med exempelvis en bredd på 960px. Gör såhär:
```
<div class="wrapper">
	<h1>All content should be properly wrapped</h1>
</div>
```

##Hjälpklasser till div's
I css/style.css finns det tre stycken hjälp-klasser som antingen ger extra utrymme ovanför eller nedanför en div. Dessa heter 'extra-margin-bottom', 'extra-margin-top' och 'extra-padding-small-bottom'. De ger en margin på 75px och 100px respektive. Klasserna används såhär:
```
<div class="wrapper extra-margin-bottom">
	<h1>This div has extra margin at the bottom</h1>
</div>
```
För extra margin i toppen:
```
<div class="wrapper extra-margin-top">
	<h1>This div has extra margin at the top</h1>
</div>
```
För extra padding i botten:
```
<div class="wrapper extra-padding-small-bottom">
	<h1>This div has extra padding in the bottom</h1>
</div>
```

##Hjälpande span-klasser
'span-yellow' kan användas när någon text ska ändra färg till hemsidans signaturfärg #F8AD09. Detta används flitigt här och där i hemsidan och ska text i en paragraf göras gul, gör såhär:
```
<p>Make text <span class="span-yellow">yellow</span> like this</p>
```
'span-emphasize' används när någon text ska göras något större och *italic*. Används på MovieLovers i samband med span-yellow. Använd såhär:
```
<p>Make text <span class="span-emphesize">bigger and italic</span> like this</p>
```
##Bilder
img/ innehåller croppade bilder som används på de olika php-sidorna. En logotyp finns även i denna katalog samt bakgrunden som används på en av div'arna i sign-up.php.