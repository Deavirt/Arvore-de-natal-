
int Tamanho = 10;

void StringRep(char *str, int n)
{
    for (int i = 0; i < n; i++)
    {
        printf("%s", str);
    }
}

int main()
{
    StringRep(" ", Tamanho);
    printf(" #\n");
    for (int i = 0; i < Tamanho; i++)
    {
        StringRep(" ", Tamanho - i);
        printf("#");
        StringRep("*", 2 * i + 1);
        printf("#\n");
    }
    int BaseTamanho = Tamanho / 3;
    int BaseGrossura = Tamanho / 3;
    for (int i = 0; i < BaseTamanho; i++)
    {
        StringRep(" ", Tamanho - BaseGrossura / 2);
        printf("#");
        StringRep("*", BaseGrossura);
        printf("#\n");
    }

    return 0;
}
