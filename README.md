# 10AcademyNante2023
# python code to check if a number "n" is a prime number
def test_prime (n):
  if n < 2 :
    return False
  for i in range(2,int(n**0.5)+1):
    if n % i==0 :
      return False
  return True
  
# python code to find all prime number between 0 and n
def all_prime (n) :
  prime = [m for m in range (n+1) if test_prime(m)]
  return prime
