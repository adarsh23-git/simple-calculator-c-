# simple-calculator-c-
simple calculator in c using goto and for loop

    int n,num1,num2;
    char a;
    for(n=0;;n+=1){
        printf("enter what you want :");
        scanf("\n%c",&a);         

        printf("enter no. :");
        scanf("%d",&num1);
        printf("enter no. :");
        scanf("%d",&num2);        
        
        if(a=='+'){
            goto add;
            
        }
        else if(a=='-'){
            goto sub;
            
        }
        else if(a=='*'){
            goto multiply;
                
        }
        else if(a=='/'){
            goto divison;    
        }
    
    
    
        add :
        printf("%d + %d = %d\n",num1,num2,num1+num2);
        continue;

        sub:
        printf("%d - %d = %d\n",num1,num2,num1-num2);
        continue;
        
        multiply:
        printf("%d * %d = %d\n",num1,num2,num1*num2);
        continue;

        divison:
        printf("%d / %d = %f\n",num1,num2,(float)num1/num2);
        continue;
    }
