# -task-2-.js-et nums=[980, 230, 210, 210, 210, 193, 190, 148, 123, 100, 100, 89, 87, 78, 78, 78, 67, 59, 56, 50, 34, 34, 34, 23, 23, 23, -190]
         [980, 230, 210, 210, 193, 190, 148, 123, 100, 100, 89, 87, 78, 78, 78, 67, 59, 56, 50, 34, 34, 34, 23, 23, 23, 3, 3, -190]
let sotmum =nums.sort()

console.log(sotmum)
 
//1C
function getUniqueNumbers(numbers) {
    return [new Set(numbers)];
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getUniqueNumbers(numbers);

console.log(result)

// 1D
;function calculateSum(numbers) {
    return numbers.reduce((sum, number) => sum + number, 0);
}
const number=[ 3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980]

const result = calculateSum(numbers);

console.log(result);

// 1E
function getNumbersLessThanOrEqualTo100(numbers) {
    let result = [];

    for (let number of numbers) {
        if (number <= 100) {
            result.push(number);
        }
    }

    return result;
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getNumbersLessThanOrEqualTo100(numbers);

console.log(result)

//1F
function getNumbersGreaterThan50(numbers) {
    return numbers.filter(number => number > 50);
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getNumbersGreaterThan50(numbers);


console.log(result);

// 1G
function getEvenNumbers(numbers) {
    return numbers.filter(number => number % 2 === 0);
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getEvenNumbers(numbers);

console.log(result);

// 1H
function getNumbersDivisibleBy3(numbers) {
    return numbers.filter(number => number % 3 === 0);
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getNumbersDivisibleBy3(numbers);

console.log(result);

//1I
function getNumbers(numbers) {
    return numbers.filter(number => number % 2 !== 0 && number % 3 !== 0);
}

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const result = getNumbers(numbers);

console.log(result);

// 1J
const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const numberOfElements = numbers.length;

console.log(numberOfElements);


// 1K

const numbers = [
    3, 56, 23, 78, 23, 78, 100, 123, 148, 193, 190, -190,
    210, 34, 67, 3, 78, 210, 34, 34, 50, 59, 89, 87,
    230, 210, 100, 23, 980
];

const reversedNumbers = numbers.slice().reverse();

console.log(reversedNumbers);


//2A
let numbers = [];

for (let element of elements) {
    if (typeof element === "number") {
        numbers.push(element);
    }
}

console.log(numbers);
//2B
let strings = [];
let i = 0;

while (i < elements.length) {
    if (typeof elements[i] === "string") {
        strings.push(elements[i]);
    }

    i++;
}

console.log(strings);

//2C
let sum = 0;
let i = 0;

do {
    if (typeof elements[i] === "number") {
        sum += elements[i];
    }

    i++;
} while (i < elements.length);

console.log(sum);

// 2D

let names = [];

for (let element of elements) {
    if (typeof element === "string") {
        names.push(element);
    }
}

let greeting = "Hello, " + names.slice(0, -1).join(", ") + ", and " + names[names.length - 1] + ".";

console.log(greeting);

// 2E

let newArray = [];

for (let element of elements) {
    if (typeof element !== "string") {
        newArray.push(element);
    }
}

console.log(newArray);

// 3A
const names = developers.map(developer => developer.name);

console.log(names);


// 3B
const totalPhones = developers.reduce(
    (total, developer) => total + developer.phones.length,
    0
);

console.log(totalPhones);

// 3C

const incompleteSetups = developers.reduce((total, developer) => {
    return total + developer.computerSetups.filter(setup =>
        setup.mice === 0 ||
        setup.keyboards === 0 ||
        setup.speakers === 0 ||
        setup.monitors === 0
    ).length;
}, 0);

console.log(incompleteSetups);

// 3D
const phoneBrands = developers.flatMap(developer => developer.phones);

const brandCounts = phoneBrands.reduce((counts, brand) => {
    counts[brand] = (counts[brand] || 0) + 1;
    return counts;
}, {});

console.log(brandCounts)


// 3E

const phoneBrands = developers.flatMap(developer => developer.phones);

const brandCounts = phoneBrands.reduce((counts, brand) => {
    counts[brand] = (counts[brand] || 0) + 1;
    return counts;
}, {});

const leastTrusted = Object.keys(brandCounts).filter(
    brand => brandCounts[brand] === Math.min(...Object.values(brandCounts))
);

console.log(leastTrusted)


//3F

const peopleWithoutPhones = developers.filter(
    developer => developer.phones.length === 0
).length;

console.log(peopleWithoutPhones);

// 3G
const peopleWithoutLaptops = developers.filter(
    developer => developer.laptops.length === 0
).length;

console.log(peopleWithoutLaptops);

//3H 

const peopleWithoutSetup = developers.filter(
    developer => developer.computerSetups.length === 0
).length;

console.log(peopleWithoutSetup);

// 3I
const developerWithMostGadgets = developers.reduce((most, developer) => {
    const laptops = developer.laptops.length;
    const phones = developer.phones.length;

    const setupGadgets = developer.computerSetups.reduce((total, setup) => {
        return total +
            setup.monitors +
            setup.keyboards +
            setup.mice +
            setup.speakers;
    }, 0);

    const totalGadgets = laptops + phones + setupGadgets;

    if (!most || totalGadgets > most.totalGadgets) {
        return {
            name: developer.name,
            totalGadgets: totalGadgets
        };
    }

    return most;
}, null);

console.log(developerWithMostGadgets);

// 3J
const developerWithMostPhones = developers.reduce((most, developer) => {
    if (!most || developer.phones.length > most.phones.length) {
        return developer;
    }

    return most;
}, null);

console.log(developerWithMostPhones.name);
console.log(developerWithMostPhones.phones);

// 3K
const developerWithMostSetups = developers.reduce((most, developer) => {
    if (!most || developer.computerSetups.length > most.computerSetups.length) {
        return developer;
    }

    return most;
}, null);

console.log(developerWithMostSetups.name);
console.log(developerWithMostSetups.computerSetups);

// 3L

const developerWithMostMonitors = developers.reduce((most, developer) => {
    const monitorCount = developer.computerSetups.reduce(
        (total, setup) => total + setup.monitors,
        0
    );

    if (!most || monitorCount > most.monitorCount) {
        return {
            name: developer.name,
            monitorCount: monitorCount
        };
    }

    return most;
}, null);

console.log(developerWithMostMonitors);
