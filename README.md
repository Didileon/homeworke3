# homeworke3


Задание 1

function oddsAndEvens(nums)
{
var evens = [];
var odds = [];
for(var i = 0; i < nums.length; i++){
if(nums[i] % 2 === 0){
evens.push(nums[i])
}
else if (!nums[i] % 2 === 0) {
odds.push(nums[i])
}
}
return {"evens":evens,"odds":odds};
}

var myNums = [1, 2, 3, 4, 5, 6, 7, 9, "Elena", "Mause", "Nik"];
result = oddsAndEvens(myNums);
console.log(result.evens);

console.log(result.odds);

_______________________________________

Задание 2

 function isPrime(n) {
            if (!Number.isInteger(n) || n < 2 || n > 1000) return "данные неверны";
 
            let k = Math.sqrt(n);
            for (let i = 2; i <= k; i++)
                if (n % i === 0) return "не простое число";
 
            return "простое число";
        }
 
        console.log(isPrime(555));
        console.log(isPrime(7));



______________________________________________________________

Задание 3

function sum(a) {
    return function(b) {
        return a + b;
    };
}

let x = sum(3);
console.log( x(4), x(6), x(6) );

console.log( sum(4)(2), sum(2)(9), sum(17)(5) );

_________________________________________

Задание 4


function int(a, b) {
    let count = a;
    const timer = setInterval(() => {
        console.log(count);
        count++;
        if (count > b) {
            clearInterval(timer);
        }
    }, 1000);
}

int(7, 15);

__________________________________________________

Задание 5

const level = (a, b) => {
    if (Number.isInteger(a) && Number.isInteger(b)) {
        return a**b;
    }
}

console.log(level(2, 14));
console.log(level(8, 3));
console.log(level(11, 5));
console.log(level(7, 9));
