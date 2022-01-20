#Fib Seequence C

'int fib(unassigned i){
    if(i < 2){
        return i;
    }
    else{
        return fib(i - 1) + fin(i - 2);
    }
}


//calling fib 
int main(int argc, char *argv[]){
    for(i = 0; i < 50;  i++){
        printf("5d: %d\n", i, fib(i));
    }
}
'
mains need to be under functions in C in order to compile

'-Wall' print almost all of the warnings 
'-Werror' treats warnings as errors
    - run both on one line when compling 

    philosophy in C is that programmer is right -- take away your complier is not going to prevent you from making bugs the way modern langs do. 

C is in man page 3 so for example to look at C specific commands do 'man 3 printf' 

