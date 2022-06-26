## ՔՆՆՈՒԹՅՈՒՆ N1

1. Թվարկել բոլոր թայփերը մեկնաբանելով և սահմանելով յուրաքանչյուրի աշխատանքը (բացառությամբ Symbol)

                պիմիտիվ թայփեր - 

number- բոլոր ամբողջական և տասնորդական թվերը,բացասական և դրական 

string - ցանկացած տեքստ հայտարարված "", կամ '',կամ ՝ ՝(ES6)ից

boolean - ունի երկու արյեք true կամ 1, false կամ 0։

undefied - երբ արժեք տված չէ, կամ չի գտնվել արժեք , արժեքի բացակայություն;

null -տալիս ենք, որ եղած արժեքը դատարկենք դարցնենք ,null ը դատարկություն է;

bigint(ES6) --- MAX SAFE INT ից մեծ թվերին են որոնց հետ խոչհուրդ չի տրվում աշխատել,ավելացնում է n;

               Refference թայփեր  կամ Object թայփեր -

 Array --- Զանգվածը նման է Object ին բայց key երի փոխարեն index ներ են,ըստ հերթականության սկսած 0ից [] 
 
 Function => --- Function ի մեջ ստեղծում ենք ցանկացաց կոդ,լոգիկա,գործողություն որի արդյունք վերադարցնում ենք return ով,ստանում
 
  է արգումենտներ,(պարամետրեր,կարող է և չստանալ որոնցով և կառող ենք կատարել գործողություններ։)

 new Date() ---  իր մեջ պարունակում է տարի,ամիս,օր,ժամ,րոպե,վարկյան,միլիվարկյան․․կարող ենք կպնել ցանկացածին։
 new Regexp() ---
 new Error()--- վերադարձնում է error
 Object ---js ում ամեն ինչ object է,ստեղցելուց գրում ենք key:value,  object ի մեջ ստեղծված functionin որի key ը գրված չէ կոչում ենք մեթոդ;


2. Ինչ տարբերություններ կան LET-ի, CONST-ի և VAR-ի միջև

LETը և CONSTը es6-ից են հասանելի դարձել; var ը չի ենթարկվում ոչ մի կանոնի, այն է, հնարավոր  Է նորից հայտարարել, կանչվում է իր 
ստեղցվելուց ավելի վերև, տեսանելի է նաև եթե հայտարարվաց է scop-երի մեջ; բացառությամբ function scop-ի,const-ով հայտարարված փոփոխականներ արյեքը չենք կարող փոխել, const-ով հայտարարվում են Refference type-երը, կամ այն արյեքները որոնք հաստատւն պետք է մնան; let ը const ը ենթարկվում են scop-երի օրենքներին։


3. Թվարկել տեսանելիության դաշտերը և սահմանել իրենց տարբերությունները

Global scope դա ամբողջ js դոքումենտն է,դրա մեջ հայտարարվածները տեսանելի են բոլորին; block scope փոփոխականները և այլն տեսանելի են միայն իր սահմանում բացառությամբ var ի և Global փոփոխականի; Function scope ը, պատկանում է իր ֆունկցիային և ամենախիստ սահմանն է միայն global փոփոխականն է տեսանելի։

4. Ի՞նչ տարբերություն կա Block Scope-ի և Function scope-ի միջև

var ով հայտարարված փոփոխականը կարող է դուրս գալ, կամ տեսանելի են եթե նույնիսկ գրված են բլոկ սկոպի մեջ օրինակ {var x = 1},Function scop ը ամենախիստ սահմանն է տեսանելի է միայն իր ֆունկցիային միայն global փոփոխականն է տեսանելի Function scope ից դուրս։

5. Ինչո՞վ են վտանգավոր գլոբալ փոփոխականներն ու var-երը

var ը և global փոփոխականների վտանգավորությունը այն է ,որ նրանք գրված լինելով scoperi մեջ (նպատակը այն է որ վերաբերվեն միայն տվյալ հատվածի կոդին) տեսանելի են scop ից դուրս և կարող են պատահաբար մոռացվել կամ փողվել փչացնելով scop ի մեջ գրված լոգիկան,կամ եթե var ի մեջ կա ինչ որ refference type օրինակ object, կարող ենք հավասարեցնել պրիմիտիվ type ի  );

6. Թվարկել ֆունկցիաները ըստ իրենց անունների ու մեկնաբանել իրենց աշխատանքը

function Declaration - function myFunction (արգումենտներ){};ունի իր սեփական կոնտեկստը(this ը աշխատում է;)։կարող է կանչվել ցանկացած տեղ,իրեն սարքելուց առաջ օրինակ,նաև hoisting է լինում,այն է interpretator ը կոդը կարդալուց function Declaration-ներին հանում է վերև;

function expression - const myFunction = function(արգումենտներ){};ունի սեփական կոնտեկստ, բայց hoisting է չի լինում,կարող է կանչվել միայն իրեն սարքելուց(հայտարարելուց հետո);

arow function - myFunction => (արգումենտ) արգումենտ*արգումենտ; -այս օրինակում return կարիք չկա, եթե օգտագործում ենք scop եր return պետք է անենք։ es6 ից է հասանելի։

7. ինչ տարբերություն կա postfix և prefix գրելաձևի միջև, ու որ դեպքերում ենք իրենց օգտագործում

Օգտագործվում է increment/decrement ի ժամանակ(x++,x--) փոփփխականի արժեքը 1 ով մեծացնելուց կամ փոքրացնելուց (միայն թվերի հետ կարելի է օգտագործել) ;
postfix - (x++) վերադարցնում է սկզբնական արժեքը նախքան increment անելը (1ով մեծացնելը)
prefix - (++x)  վերադարցնում է  արժեքը արդեն increment արած (1ով մեծացրած)


8. Մեկնաբանել null-ի և undefined-ի տարբերությունները

undefined ը երբ արժեք տված չէ, կամ չի գտնվել արժեք , արժեքի բացակայություն;
null տալիս ենք, որ եղած արժեքը դատարկենք դարցնենք ,null ը դատարկություն է;

9. HTML-ում script թեգը միացնելու ամենահարմար վայրը դա ... շարունակել միտքը և սահմանել թե ինչու

փակվող body ից առաջ միացնելն է,  script ը block է անում html ծառին, ավելի օպտիմալ է, որ html ի head և body ին կառուցվեն ինչքան հնարավոր է։


10. JavaScript-ը արդյո՞ք կարող է բրաուզերում աշխատել առանց HTML-ի, գրեք այո կամ ոչ

Ոչ։

11. թվարկեք Boolean օպերատորները և սահմանեք նրանց նշանակություններն ու անունները

true կամ 1, false կամ 0։

12. ինչ տարբերություն կա այս օպերատոների միջև ==, ===

== ստուգում է համեմատվողների միայն value ները, === ավելի խիստ ստուգում է անում և type և value:  

13. ինչ տարբերություն կա պրիմիտիվ և հղումային թայփերի միջև

հղումային թայփերը նրանք են, որոնք պարունակում են ստեղծված օբյեկտների հղում/հասցե
պրիմիտիվ թայփերը իրենց մեջ տեղեկատվությունը պահվում է որպես այդ փոփոխականի արժեք



14. ինչի՞ համար են օգտագործվում BREAK և CONTINUE օպերատորները և ո՞րտեղ

Break ը  Օգտագործում ենք loop երում , և switch ում կրկնվող գործողությունը ինչ որ պայմանով ընդհատելու համար։
CONTINUE ն պայմանը բավարարելու դեպքում ընդհատում է loop ի միայն մեկ պտույտ։ շարունակելով loop ի պայմանը։
while loop ի ժամանակ CONTINUE ն չի կարելի օգտագոչծել; infinity loop կստանանք։


15. Ո՞ր մաթեմատիկական օպերատորի դեպքում և ո՞ր պագայաում console-ում կարող ենք ստանալ infinity

Թիվը բաժանենք 0-ի կստանանք infinity։


16. ի՞նչ է նշանակում NaN և ո՞ր դեպքում կարող ենք իրեն ստանալ

Նանը թիվ չէ; կստանանք եթե ինչ որ մաթեմատիկական գործողություն անենք թվի և այլ type ի միջև, console.log(5/"string"):


17. ի՞նչ է նշանակում NPM

հապավում է բացվում է node packige manager;


18. Ինչպե՞ս ենք NPM-ը միացնում մեր պրոյեկտին

npm init հրամանով


19. Ի՞նչ package-ներ գիտեք և ինչպե՞ս եք դրանք ավելացրել ձեր պրոյեկտի մեջ
jshint ռեալ ժամանակում անալիզ է անում  կոդը հետեվելով js կանոններին կարիք չկա run անել կոդը խնդիրները տեսնելու համար
jshint ը npm ի package է,
npm install -g jshint          հրամանով գլոբալ,
npm install --save-dev jshint   լոկալ պրոյեկտի մեջ;


20. Ի՞նչ տարբերություն կա DevDependecy-ի և Dependecy-ի միջև


DevDependecy իի մեջ են այն package ները որոնցից կախված է ծրագրավորողը(Օգնում է ծրագրավորողին պրոեկտի ընթացքում)։
Dependecy իի մեջ ի package ներից կաղված է պրոյեկտը։


21. for loop-ով աստղանիշներով console-ում ստանալ լիարժեք՝ կլորանման բան (անկյունները կոտրած), քառակուսի, եռանկյունի, 
ուղղանկյուն, երկու քառակուսի իրար կողք և ցանկացած տառ (latin)


let res =""
let armat = "         * "+"\n         *"

for(i = 0;i < 9; i++) {
  let result1 = "";
  let result = "";
  for (j = 0; j < 9 - i ; j++) {
    result += " ";
  }
  for (j = 0; j < 2 * i + 1 ; j++) {
    result += "*";
  }
  res += (result + result1) + ("\n")
};
console.log(res + armat);


22. ստեղծում ենք փոփոխական, որի մեջ ստեղծում եք սթրինգ 500 բառից բաղկացած պատմություն, ու էդ սթրիգի մեջ օգտագործում եք ${} սրանցից
ու մեջը գրում եք տարատեսակ JS կոդեր, որոնք կարող են ձեր պատմության հետ կապ ունենալ, օրինակ (տարեթվեր, անուններ և այլն)


const famousMen = {
    fullName: "Օնիկ Թադևոսի Կարապետյան",
    born: "1914",
    city: "Գյումրի",
    firstBook:"«Գարնանամուտ»",
    famousPoem:"Հայոց Դանթեական",
};


let textFortest = `${famousMen.fullName}ը Ծնվել է ${famousMen.born} թվականին Ալեքսանդրապոլ քաղաքում (այժմ՝ ${famousMen.city})։ 
Շիրազը մեծացել է աղքատության մեջ։ Առաջին գիրքը՝ «${famousMen.firstBook}» վերնագրով, հրատարակվել է 1935 թվականին։
Նովելագիր Ատրպետը տաղանդավոր պոետին տալիս է «Շիրազ» գրական անունը, որովհետև «Այս երիտասարդի բանաստեղծությունները Շիրազի թարմ և ցողով
ծածկված վարդերի բուրմունքն ունեն» (Շիրազը քաղաք է Իրանում, որը հայտնի է իր վարդերով և պոետներով)։
Սովորել է Երևանի համալսարանի բանասիրական ֆակուլտետում, այնուհետև՝ Մոսկվայի Մ. Գորկու անվան գրականության ինստիտուտի գրական բարձրագույն
դասընթացներում։ 1958 թվականին հրատարակում է «Քնար Հայաստանի» գրքի առաջին հատորը։ Երկրորդ և երրորդ հատորները
հրատարակվում են 1965 թվականին և 1974 թվականին։ Այս ժողովածուները ներառում են Շիրազի պոեզիայի լավագույն նմուշները։
Շիրազի ստեղծագործությունները չափածո են։ Նա հեղինակ է հանրաճանաչ հայրենասիրական և լիրիկական պոեմների ու բանաստեղծությունների,
որոնցից են՝ «Անի», «Սիամանթո և Խջեզարե», «Էքսպրոմտ», «Իմ սուրբ Հայրենիք», «Սերս գաղտնի թող մնա», «Հայերի ճակատագիր», «Անդրանիկին» և այլն։ 
Նա գրել է «${famousMen.famousPoem}» մեծածավալ պոեմը, որը Հայոց ցեղասպանության մասին է, թեմա, որն արգելված էր Խորհրդային Միությունում.
Գլուխգործոց համարվող այս ստեղծագործության առաջին տարբերակը գրվել է 1941 թ.[1] Շիրազի կենդանության օրոք այդ գործից միայն կարճ
հատվածներ հրատարակվեցին Խորհրդային Միությունում և մի քանի գլուխներ Բեյրութում և Թեհրանում։ Պոեմը 
ամբողջությամբ (ավելի քան 8000 տող) լույս տեսավ Երևանում 1990 թվականին։`
՝

23. ստեղծում եք ֆունկցիա, որը կաշխատի ֆակտորիալ ֆորմուլայով

function fact(n){
        
        let result = 1;
        while(n>0) {
            result *= n
            n--
    };      
        return result;
    }

console.log(fact(5));

24. ստեղծում եք ֆունկցիա, որը կաշխատի ֆիբոնաչի ֆորմուլայով

const fibNum = function(num1,num2){
    let fibArr = [num1,num2]

    if(num2 < num1 || typeof(num1) !== "number" && num2 !== "number" ) {
        return "Երկրորդ թիվը առաջինից մեծ չէ կամ թվեր չեն գրված"
    };

    for(i = 2;i < 3; i++){
    fibArr[i] = fibArr[i-1] + fibArr[i-2]
    }
    return fibArr
  };
  console.log(fibNum(3,4))


25. ստեղծում եք ֆունկցիա, որը որպես արգումենտ ստանում ա ինչ-որ հայտնի շենք/կառույց, ու վերադարձնում ա էդ շենքի պարամետրերը (բարձրություն, լայնություն, քմ և այլն)

const petronasTowers = {
    height: "451,9 m",
    roof: "378,6m",
    floorCount:"88 FLOUR Count",
    floorArea: "395,000 m2"
};

function infoBuilding (name){

    let parameters =  Object.values(name)
    const buildingDetails = [];
    for(i = 0; i < parameters.length; i++){
        buildingDetails[i] = parameters[i]
    }
   return buildingDetails
};

console.log(infoBuilding(petronasTowers))

26. ստեղծում եք ֆունկցիա, որը իր մեջ ստեղծում է մեքենաներ (արգումենտներով), որ ամեն կանչելուց կարողանաք այլ պարամետրեր տալ ու ստանալ տարբեր մեքենաներ

const newCar = function(mark,model,year){
    if(typeof(mark) === "string" && typeof(model) === "string" && typeof(year) === "number"){
        return `${mark}  ${model}  ${year}`
    };
    return "Type Right Car"
} 

console.log(newCar("BMW","X5",2017))

27. ստեղծում եք 2 զանգված, որտեղ առաջինում պետք է լինեն և բացասական և դրական թվեր, ու for loop-ի միջոցով զանգվածից հանեք դրական թվերը, իսկ բացասականները դրեք 2րդ դատարկ զանգվածի մեջ

const numList = [1,8,9,6,4,7,-1,-4,-19,9,-81,-64];
const numListNeg = [];
k=0

for(i = 0;i < numList.length; i++){
    
    if(numList[i] < 0){
        numListNeg[k] = numList[i]
        k++

    }
}

console.log(numListNeg)



28. ստեղծում եք օբյեկտ, որտեղ նկարագրում եք մարդու, որը ունի ընկերներ, ստատուսներ, սև ցուցակի մեջ մարդիկ, լայքեր, էլ. հասցե, հեռախոս, գաղտնաբառ և այլն (նմանեցնել Ֆեյսբուքին)

const userId1 = {
    fullName: "Հակոբ Հակոբյան",
    age: "20",
    friendsList: ["Հայկ Հակոբյան","Վլադիմիր Մուրադյան","Վարդան Կարապետյան","Դոնալդ Տրոամփ"],
    blackList: ["Խաչատրյան Վարդուհի,Առաքելիան Մարիամ,Գասպարյան Վահե"],
    email: "example@gmail.com",
    tel: "077-xx-xx-xx",
    education: "example university"
    posts: ["Բարևներ"," "," "]

    };

29. ստեղծում եք զանգված, ու մեջը 10 հատ օբյեկտ, ամեն օբյեկտում ձեր նախընտրած մարդկանց մասին մի քանի ինֆորմացիա՝ անուն ազգանուն, տարիք, մասնագիտություն ու ազգություն, հետո loop-ի միջոցով էդ օբյետկտերի մարդկանց անունները տպում եք կոնսոլում

listofUsers =  [
    { fullName: "Լիկա Ավագյանց",age: "17", },
    { fullName: "Սամսոն Խաչատրյան", age: "21", },
    { fullName: "Ալիսա Սուրենյանց", age: "23", },
    { fullName: "Մանե Սարգսյան", age: "24", },
    { fullName: "Նելլի Դավթյան", age: "25",},
    { fullName: "Քրիստինե Արսենյան", age: "30",},
    { fullName: "Տիգրան Ռուբենյան", age:"20", },
    { fullName: "Անի Առուստամյան", age:"17", },
    { fullName: "Կարինե Տոնոյան", age: "31", },     
];

for(i = 0;i < listofUsers.length; i++){
    if(typeof(listofUsers[i].fullName) === "string"){
        console.log(listofUsers[i].fullName)
    }
};


30. ստեղծում եք Math անունով օբյեկտ, որի մեջ մեթոդներով ստեղծում ենք այն մաթեմատիկական ալգորիթմներ (արմատ, քառակուսի և այլն)

const math = {

    perimeter (a,b,c) {
        p = a + b + c
        if(a === undefined || b === undefined || c === undefined){
            return "Complete All Fields"
        };
        if(typeof(a) !== "number" || typeof(b) !== "number" || typeof(c) !== "number"){
            return "Not A Number"
        };
        return `perimeter of triangle = ${p}`
    },

    pythagoreanTheorem(a,b){

        if(a === undefined || b === undefined){
            return "Complete All Fields"
        };
        if(typeof(a) !== "number" || typeof(b) !== "number"){
            return "Not A Number"
        };
        let result=Math.pow((a*a)+(b*b),1/2); 
           return result;
    }

    

}
console.log(math.pythagoreanTheorem(3,3))



## ի՞նչ կստանանք կանսոլում ԿԱՐԵՎՈՐ Է ՈՐ ԱՌԱՆՑ ԿՈՆՍՈԼ ԱՆԵԼՈՒ ՊԱՏԱՍԽԱՆԵՔ !!!!!!!!!!

31. 
typeof true - boolean
typeof false - boolean
typeof function () {} - function
typeof null - object
typeof [] -object
typeof {} -object
typeof " " - string
typeof 0 - number
typeof 1 - number
typeof NaN - number
typeof undefined - undefined
typeof Object - object
typeof Object() - function
typeof Array - function
typeof Array() - object բացառություն
typeof Boolean - function
typeof Bollean() - bollean

32. NaN || 2 || undefined  - 2

33. NaN && 2 && undefined ?

34. 1 && 2 && 3  - 3

35. !1 && 2 || !3 - false

36. 25 || null && !3 - 25

37. NaN || null || !3 || undefined || 5 - 5

38. NaN || null && !3 && undefined || 5 - 5

39. 5 === 5 && 3 > 1 || 5 - 5 true

40. 10 <= 8 && !9 || 10 > 5 true

41. 
const a = true, b = false;
console.log(!a) - false
console.log(!b) - true

42. 
const a = true, b = false, c = 4;
console.log(a || b); - true
console.log(b || b); - false
console.log((c>2) || (c<2)); - true

43. 
const a = true, b = false;
const c = 4;
console.log(a && a); true
console.log(a && b); false 
console.log((c > 2) && (c < 2)); false

44. 
const a = 2, b = 'hello';
console.log(a !== 2); false
console.log(a !== '2'); false
console.log(b !== 'Hello'); true

45. 
console.log( true || true );  true
console.log( false || true ); true
console.log( true || false ); true
console.log( false || false ); false

46. 
Ինչ կստանանք կոնսոլի մեջ
let x = 4;
do {
     console.log("FALSE");
     x++;
} while (x > 4 && x > 6)  FALSE

47. 
console.log( 1 || 0 );  1
console.log( null || 1 ); 1
console.log( null || 0 || 1 ); 1
console.log( undefined || null || 0 ); 0
console.log( null || 2 && 3 || 4 ); 4

48. 
if (-1 || 0) console.log( 'first' ); ktpi 'first'
if (-1 && 0) console.log( 'second' ); chi tpi
if (null || -1 && 1) console.log( 'third' ) ktpi;'third'

49. 
console.log(!undefined); true
console.log(!null); true
console.log(!20); false
console.log(!0);  true
console.log(!NaN); true
console.log(!{}); false
console.log(!''); true // որովհետև սթրինգի մեջ դաըարկ է
console.log(!'OK'); false
console.log(!false); true
console.log(!true); false

50. 
const a = 5, b = 10;
(a != b) && (a < b); true
(a > b) || (a == b); false
(a < b) || (a == b); true     
!(a < b); false
!(a > b); true
