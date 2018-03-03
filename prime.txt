echo "Enter a number"
read num
count=0
for((i=1;i<=num;i++)) 
do
      	if test `expr $num % $i` -eq 0
	then
		(( count+1 ))
	fi
	
done
if test $count -eq 2								
then
	echo "It is a prime number"
else	
	echo "It is not a prime number"
fi   
