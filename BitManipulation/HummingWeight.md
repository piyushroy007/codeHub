## HummingWeight (No. of 1 bits)


## Solution 1: 
    var hammingWeight = function(n) {
        let count = 0;
         while (n > 0) {
            // check last bit
            count += n & 1;
            // shift right by 1 bit
            n = n >>> 1; // unsigned shift
        }
        return count;
    };
    
## Solution 2 :    
    
    var hammingWeight = function(n) {
        return n.toString(2).split('0').join('').length;
    };
