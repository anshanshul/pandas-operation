# pandas-operation

 #enumrate
car={'hI':30,'kio':50,"iop":40,"oops":50}
for i,k in enumerate (car):

    print("i is ",i,"k is",k)
import pandas as p
s1= p.Series([12,25,60,68])
print(s1)
s1=p.Series([12,25,60,68],index =['A','AA','AAA','AAAA'])
print(s1)
print(s1['A'])
print(s1[['A','AAAA']])#retriving the multiple elemnts
ss1=p.Series(tuple('abcd'))#making series of tuple
print(s1)
s1=p.Series(range(5),index=['01','02','03','04','05'])
print(s1)
s1=p.Series(range(5),index=list('ansha'))#duplicate index of series
print(s1)
print(s1['a'])
s1=p.Series(['hadoop','weid','tyapo'],index = [1,3,5])
print(s1)
s2=s1.reindex(range(5))
print(s2)
s2=s1.reindex(range(5),fill_value='python')#filling a specific values on blank space
print(s2)
s2=s1.reindex(range(5),method='ffill')#fill the empty value according is above
print(s2)
s3=p.Series([112,25,60,68])
print(s3*4)
print(s3+2)
######################################################################

d={'name':['anuj','vikas','suamn','popo'],'Age':[25,26,27,28],'Amount':[25000,24000,26000,600]}
d1=p.DataFrame(d)
print(d1)
print(d1.describe())
data=p.read_csv('test.csv')
print(data)
print(data.crim)
print(data.crim > 1.00 )
print(data.head())
print(data.head(1))
print(data.describe())
print(data.crim.mean())

