/* New Things Every Day — Da 106 */
/* Calculates minimum, maximum, average, and total */

function dailyLog106() {
    const numbers = [18, 42, 7, 93, 56, 31, 74];

    const total = numbers.reduce((sum, value) => sum + value, 0);
    const average = Number((total / numbers.length).toFixed(2));
    const minimum = Math.min(...numbers);
    const maximum = Math.max(...numbers);

    const report = {
        day: 106,
        timestamp: new Date().toISOString(),
        total,
        average,
        minimum,
        maximum
    };

    console.log("Day 106 Report:", report);
}

dailyLog106();
