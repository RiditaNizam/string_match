# string_match
CodingBat Python Warmup-2

Given 2 strings, a and b, return the number of the positions where they contain the same length 2 substring. So "xxcaazz" and "xxbaaz" yields 3, since the "xx", "aa", and "az" substrings appear in the same place in both strings.

def string_match(a, b):
  
    count = 0
  
    if len(a) < len(b):
      shorter = a
    
    else:
  
      shorter = b
  
    for i in range(len(shorter)-1):
  
      if a[i:i+2] == b[i:i+2]:
  
        count += 1
  
    return count
