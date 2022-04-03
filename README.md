# /bin/bash
echo "Enter two numbers:";
read a;
read b;
echo "Enter Choice:";
echo "1. Addition:";
echo "2. substraction:";
echo "3. multiplication:";
echo "4. Division:";
read ch
case $ch in
1) res= 'echo $a + $b | bc';;
2) res= 'echo $a - $b | bc';;
3) res= 'echo $a * $b | bc';;
4) res= 'echo "scale=2 $a / $b "';;
esac
echo "Result is : $res"
