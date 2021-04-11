---
title: 20/21 შემოდგომა ფინალური გამოცდის შეკითხვები
parent: რესურსები
---

<button id="toggle_answers">პასუხების დამალვა/ჩვენება</button>

<script>
const correctAnswers = [...document.getElementsByTagName('input')].filter(a => a.checked);
function toggleAnswers() {
    correctAnswers.forEach(a => a.checked = !a.checked);
}
document.getElementById('toggle_answers').onclick = toggleAnswers;
</script>


## ლექციები - 8 კითხვა 12ქ, 4x1 4x2

<!-- 1 3 -->
### 1. 1 ქულა
აქედან რომელში არ გამოიყენება კომპრესირების ალგორითმი?
- [ ] სურათი
- [ ] არქივი (zip, rar)
- [x] ტექსტური დოკუმენტი (word, txt)
- [ ] ყველაში გამოიყენება
- [ ] არცერთში გამოიყენება

<!-- 2 4 -->

### 2. 1 ქულა
არის თუ არა javascript პორტატული ენა? 
- [x] დიახ
- [ ] არა


<!-- 3 7 -->


### 3. 2 ქულა
აქედან რომელია პროტოკოლის მაგალითი?
- [ ] wifi კავშირი როუტერსა და კომპიუტერს შორის
- [ ] bluetooth კავშირი ლეპტოპსა და bluetooth სპიკერს შორის
- [ ] bluetooth კავშირი ორ ტელეფონს შორის
- [x] ყველა
- [ ] არცერთი

<!-- 4 9 -->
### 4. 1 ქულა
აქედან რომელია კლიენტი პროგრამის მაგალითი?
- [ ] skype
- [ ] Facebook-ის აპლიკაცია
- [ ] Facebook-ის საიტი
- [ ] ბრაუზერი
- [x] ყველა
- [ ] არცერთი


<!-- 5 13 -->
### 5. 2 ქულა
რომლის შეცვლა არის შესაძლებელი კლიენტ აპლიკაციაში?
- [x] front-end
- [ ] back-end
- [ ] ორივეს
- [ ] არცერთის


<!-- 6 14 -->
### 6. 2 ქულა
როგორ იგზავნება PGP გასაღები კომუნიკაციის დაწყებისას?
- [ ] დაშიფრულად
- [x] დაუშიფრავად

<!-- 7 15 -->
### 7. 2 ქულა
ხელოვნური ინტელექტის რომელ მიმართულებას იყენებს google text search?
- [x] supervised
- [ ] reinforcement
- [ ] unsupervised

<!-- 8 16 -->

### 8. 2 ქულა
აქედან რომელი კრიტერიუმი არის მნიშვნელოვანი ალგორითმის შეფასებისას?
- [ ] რამდენი ოპერაცია იქნება საჭირო
- [ ] რამდენი მეხსიერება ჭირდება
- [x] ორივე
- [ ] არცერთი

## სემინარები - 12 კითხვა 18ქ, 6x1, 6x2


### კარელი 3კ 5ქ, 1x1, 2x2
<!-- 9 -->
### 9. 2 ქულა
კარელი არის საწყის პოზიციაზე (1x1 უჯრა, იყურება აღმოსავლეთით). ამ კოდის შედეგად იქნება თუ არა ნებისმიერი მოცემულობის სამყაროში პირველი ხაზის ყველა უჯრაზე მხოლოდ ერთი ბურთი?

```javascript
while(frontIsClear()) {
    if (!beepersPresent()) {
        putBeeper();
    }
    move();
}
```

- [ ] ვერა, რადგან კოდში არის ბაგი
- [ ] ვერა, რადგან რიგ შემთხვევებში თუ რომელიღაც უჯრაზე უკვე არის ბურთი, კარელი დადებს მეორე ბურთს
- [ ] ეს კოდი აკმაყოფილებს პირობას
- [ ] ვერა, რადგან კარელი ბურთს მხოლოდ იმ უჯრებზე დადებს, რომელზეც უკვე არის ბურთი და საერთოდ არ დადებს ცარიელ უჯრებზე
- [x] ვერა, რადგან რიგ შემთხვევებში რომელიღაც უჯრაზე არ დაიდება ბურთი მაშინაც, როცა ცარიელია

<!-- 10 -->
### 10. 1 ქულა
კარელი არის 3x3 სამყაროში საწყის პოზიციაზე (1x1 უჯრა, იყურება აღმოსავლეთით). რა მოხდება ამ კოდის გაშვების შემთხვევაში?
```javascript
while(frontIsClear()) {
    turnLeft();
    move(); // მესამე ხაზი
    turnLeft();
    move(); // მეხუთე ხაზი
}
```
- [ ] კარელი გაიჭედება უსასრულო ციკლში
- [ ] კარელი შეეჯახება კედელს მესამე ხაზზე (პირველ ან მომდევნო ციკლზე)
- [x] კარელი შეეჯახება კედელს მეხუთე ხაზზე (პირველ ან მომდევნო ციკლზე)
- [ ] კარელი დაასრულებს მოძრაობას საწყის პოზიციაზე
- [ ] კარელი დაასრულებს მოძრაობას მეორე რიგის პირველ უჯრაზე

<!-- 11 -->
### 11. 2 ქულა

როგორ სამყაროში იმუშავებს ეს კოდი ბაგის (ერორის) გარეშე?
```javascript
move();
while (beepersPresent()) {
    pickBeeper();
    move();
    putBeeper();
    turnAround();
    move();
    turnAround();
}
```
- [ ] ნებისმიერ სამყაროში
- [ ] სამყაროში, რომელშიც უჯრების რაოდენობა 4-ზე მეტი ან ტოლია
- [x] სამყაროში, რომელშიც უჯრების რაოდენობა 3-ზე მეტი ან ტოლია
- [ ] სამყაროში, რომელშიც უჯრების რაოდენობა 2-ზე მეტი ან ტოლია
- [ ] სამყაროში, რომელშიც უჯრების რაოდენობა 1-ზე მეტი ან ტოლია
- [ ] ვერცერთ სამყაროში ვერ იმუშავებს


### javascript 3კ 4ქ (ცალკე, კარელის და ვების გარეშე) 2x1, 1x2
### 12. 1 ქულა
<!-- 12 -->
რომელი ფუნქცია დაბეჭდავს ტექსტს ოთხჯერ?
```javascript
function f1() {
    let i = 0
    while (i !== 4) {
        i++;
        console.log('text')
    }
}

function f2() {
    let i = 0
    while (!(i === 4)) {
        i++;
        console.log('text')
    }
}
```
- [ ] f1
- [ ] f2
- [x] ორივე
- [ ] არცერთი

<!-- 13 -->

### 13. 1 ქულა
რას დაბეჭდავს ქვემოთ მოცემული კოდი?
```javascript
function f1(i) {
 i = i + 1
}

let i = 3
f1()
f1()
console.log(i)

```
- [ ] 2
- [x] 3
- [ ] 4
- [ ] 5
- [ ] 6
- [ ] არცერთი პასუხი არ არის სწორი

<!-- 14 -->
### 14. 2 ქულა
რას დააბრუნებს ეს ფუნქცია?
```javascript
function f1(m, n) {
    let k = 0
    for (let i = 1; i <= m; i++) {
        if (i % n === 0) {
            k++
        }
    }
    return k
}
```
- [ ] m-ს გამყოფების რაოდენობას
- [ ] n-ის გამყოფების რაოდენობას
- [ ] ლუწ რიცხვებს m-მდე
- [ ] კენტ რიცხვებს n-მდე
- [ ] არცერთი პასუხი არ არის სწორი

### html/css 3კ 4ქ(javascript-ის გარეშე) 2x1, 1x2
<!-- 15 -->
### 15. 1 ქულა
html1.png
რომელი სურათია ამ კოდის შესაბამისი? 

```html
<ul>
<ol>
<ul>
<li>hello</li>
</ul>
<li>hello2</li>
</ol>
<li>hello3</li>
</ul>
```

- [ ] 1
- [ ] 2
- [ ] 3
- [ ] არცერთი

სწორი პასუხი: 1

<!-- 16 -->
### 16. 1 ქულა
რაზე გავრცელდება მოცემული სელექტორი?

div, .someclass

- [x] ყველა div და ყველა someclass კლასის ელემენტზე
- [ ] ყველა someclass კლასის ელემენტზე, რომელიც მოთავსებულია div ელემენტში
- [ ] ყველა someclass კლასის ელემენტზე, რომელიც ასევე არის div 
- [ ] არცერთი არ არის სწორი

<!-- 17 -->
### 17. 2 ქულა
html3.png

პირველ სურათზე ნაჩვენებია ამ კოდის შესაბამისი საიტი. რომელ სურათშია მოცემული საიტი, რომელიც მიიღება .container კლასისთვის padding სტილის მოშორების შემდეგ?

```html
<head>
    <style>
        .photo-gallery {
            background: rgb(255, 254, 217);
            padding: 25px;
        }
        .container {
            padding: 30px;
        }
        .photo {
            width: 200px;
            margin: 5px;
            border: 2px solid;
        }
    </style>
</head>
<body>
    <h1>Boxers are beautiful?</h1>
    <div class="container">
        <div class="photo-gallery">
            <img class="photo" src="https://....">
            <img class="photo" src="https://....">
            <img class="photo" src="https://....png">
        </div>
    </div>
</body>
```
- [ ] 2 (სურათებს შორის სივრცე შემცირებულია)
- [x] 3 (ყვითელი ფონი არის გადიდებული)
- [ ] 4 (სურათები მიწეულია მარცხნივ)
- [ ] არ შეიცვლება
- [ ] არცერთი პასუხი არ არის სწორი

სწორი პასუხი: 3

### web 3კ 4ქ (html/css/javascript ერთად) 2x1, 1x2
<!-- 18 -->
### 18. 1 ქულა
აქედან რომელი დააბრუნებს სიას?
1. document.querySelector
2. document.getElementsByClassname
3. document.getElementById

- [ ] 1.
- [x] 2.
- [ ] 3.
- [ ] ყველა
- [ ] არცერთი

<!-- 19 -->
### 19. 1 ქულა
რა მოხდება საიტზე ღილაკზე დაჭერის შემთხვევაში?
```html
<p id='text'>text1</p>
<button id="setText">click here</button>
<script>
    function setText() {
        document.getElementByID('text').innerText = 'text2'
    }
</script>
```
- [ ] ღილაკის ტექსტი შეცვლება და გახდება 'text2'
- [x] არაფერი მოხდება
- [ ] კონსოლში იქნება error იმის გამო, რომ საიტი setText() ფუნქციას ვერ პოულობს
- [ ] პარაგრაფის ტესტი შეიცვლება და გახდება 'text2'
- [ ] არცერთი პასუხი არ არის სწორი

<!-- 20 -->
### 20. 2 ქულა

რა მოხდება საიტის ჩატვირთვისას?
```html
<p id='text'>1</p>
<script>
    let elem = document.getElementByID('text')
    let previous = elem.innerText
    elem.innerText = previous + 1
</script>
```
- [ ] არაფერი მოხდება
- [ ] კონსოლში იქნება error იმის გამო, რომ საიტი ელემენტს ვერ პოულობს
- [ ] კონსოლში იქნება error იმის გამო, რომ რომელიღაც ოპერაცია ნებადართული არ არის
- [ ] პარაგრაფის ტესტი შეიცვლება და გახდება '2'
- [x] არცერთი პასუხი არ არის სწორი

## მეორე ქვიზის კითხვები
### 1 ქულა
რას დაბეჭდავს ქვემოთ მოცემული კოდი?
```javascript
function f1(n) {
    let a = 0;
    for (let i = 1; i <= n; i++) {
        if (i % 2 === 0) {
            a++
        } else {
            a--
        }
    }
    return a;
}
console.log(f1(5))
```
- [ ] 0
- [ ] 1
- [ ] 2
- [ ] 3
- [x] არცერთი პასუხი არ არის სწორი

### 2 ქულა
მოცემულია დავალების კოდი და ტესტის პირობა - "ღილაკზე დაჭერის შემდეგ პოსტის ველში შეყვანილი ტექსტი უნდა დაემატოს პოსტების ფიდში (დაპოსტილი პოსტები)". რომელ ფუნქციაში არის შესასწორებელი შეცდომა (ან ხაზი გამორჩენილი) იმისთვის, რომ კოდმა ეს პირობა დააკმაყოფილოს?
```html
<textarea id="post_text" placeholder="what's up?"></textarea>
<div id="button_container">
    <button id="new_post" onclick="newPost()">Post</button>
</div>
<div id="posts"></div>
<script>
    let postId = 1;
    function createNewPost(text, postId) {
      let elem = `
        <div id="post${postId}" class='post'>
        </div>`;
        document.getElementById("posts").insertAdjacentHTML("afterbegin", elem);
    }

    function newPost() {
      let input = document.getElementById("post_text").value;
      createNewPost(input, postId);
      postId++;
    }
</script>
```
- [x] createNewPost()
- [ ] newPost()
- [ ] ორივე
- [ ] არცერთი


### 2 ქულა
გვსურს გავიგოთ, არის თუ არა b a-ს გამყოფი. რომელი ფუნქცია იმუშავებს ამისთვის?
```javascript
f1(a, b) {
    return a % b
}


f2(a, b) {
    if (a % b) {
        return true
    }
    return false
}


f3(a, b) {
    if (a % b) {
        return true
    } else {
        return false   
    }
}
```
- [ ] f1
- [ ] f2
- [ ] f3
- [ ] f1 და f3
- [ ] ყველა
- [x] არცერთი
