# python
def normalize(s):
        return s.lower().capitalize()
L1 = ['adam', 'LISA', 'barT']
L2 = list(map(normalize, L1))
print(L2)


from functools import reduce
def prod(s):
    def fn(x,y):
        return(x*y)
    return reduce(fn,s)
print (prod([1,2,3,9,12]))




def char2num(s):
    L=list(map(int,s.split('.')))
    return L
def fn(x,y):
    return x+y*0.1**len(str(y))
def char2float(s):
    return reduce(fn,char2num(s))
print (char2float('12.3445666'))
