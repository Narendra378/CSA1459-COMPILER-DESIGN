%{
int line=0;
int ch=0;
int word=0;
%}
%%
\n line++;
([ ])+ word++;
. ch++;
%%
int yywrap(){}
int main(int argc,char*argv[]){
yyin=fopen(argv[1],"r");
yylex();
printf("no of line is:%d\n",line);
printf("no of words is:%d\n",word);
printf("no of characters is:%d\n",ch);
fclose(yyin);
}
