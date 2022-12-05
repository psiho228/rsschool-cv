# Sheredega Nikolay

## Contacts
+ Location: Georgia, Tbilisi
+ Phone: +79191066573
+ Email: irm.228322@gmail.com
+ GitHub: Psiho228
# About me

I'm good in team work and also very good at learning something new. I'm always trying to improve my skills.
Also I'm not a stressful person, and you can depend on me in any problem.
# Skills
+ HTML(basic)
+ CSS(basic)
+ JavaScript(basic)

# Code Example 

```java const api = "https://api.exchangerate-api.com/v4/latest/USD";

  

var search = document.querySelector(".searchBox");
var convert = document.querySelector(".convert");
var fromCurrecy = document.querySelector(".from");
var toCurrecy = document.querySelector(".to");
var finalValue = document.querySelector(".finalValue");
var finalAmount = document.getElementById("finalAmount");
var resultFrom;
var resultTo;
var searchValue;
  

fromCurrecy.addEventListener('change', (event) => {
    resultFrom = `${event.target.value}`;
});
  

toCurrecy.addEventListener('change', (event) => {
    resultTo = `${event.target.value}`;
});
  
search.addEventListener('input', updateValue);
  

function updateValue(e) {
    searchValue = e.target.value;
}
  

convert.addEventListener("click", getResults);
  

function getResults() {
    fetch(`${api}`)
        .then(currency => {
            return currency.json();
        }).then(displayResults);
}
  

function displayResults(currency) {
    let fromRate = currency.rates[resultFrom];
    let toRate = currency.rates[resultTo];
    finalValue.innerHTML = 
       ((toRate / fromRate) * searchValue).toFixed(2);
    finalAmount.style.display = "block";
} 
 ```
 # Experience
 None
 
 # Education
  + Three years of Moscow Technological University (unfinished)
  + Self-studing
  # English
  **B1-B2** (I had been learning English in school and passed exams, but I havent got much practice from then)