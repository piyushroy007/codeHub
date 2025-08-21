## Solution

    var sumSqDigits = function (x) {
      let s = 0;
      while (x > 0) {
        const d = x % 10;
        s += d * d;
        x = (x / 10) | 0;
      }
      return s;
    }
    var isHappy = function(n) {
        if (n <= 0) return false;
        const seen = new Set();
        while (n !== 1 && !seen.has(n)) {
            seen.add(n);
            n = sumSqDigits(n);
        }
        return n === 1;
    };
