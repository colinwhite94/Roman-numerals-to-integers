class Solution:
    def romanToInt(self, s: str) -> int:
        
        rom_dict = {"I": 1, "V": 5, "X": 10, "L": 50, "C": 100, "D": 500, "M": 1000}
        total = 0
        i = 0

        while i < len(s):
            if i < len(s) - 1 and rom_dict[s[i]] < rom_dict[s[i+1]]:
                total = total + rom_dict[s[i+1]] - rom_dict[s[i]]
                i = i + 2

            else:
                total = total + rom_dict[s[i]]
                i = i + 1
        return(total)
