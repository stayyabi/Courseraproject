
# Assignment_of_Guessing_Number
# Run_at_25_07_2022 @9:51 pm
# 20 Lines of Code
```
function guess(){
    true_ans=$(ls -l |grep "^-"|wc -l)
    while true;
    do
        echo "Your Guess Number is"
        read  number
        if [ $number -lt $true_ans ]
        then
            echo "Your Guess is less than actual true number"
        elif [ $number -gt $true_ans ]
        then
            echo "Your Guess is greater than actual true number"
        else
            echo " congratulation, you Guessed right!"
        break;
        fi
    done
}
echo "guess the files number in the current directory!"
guess
``````