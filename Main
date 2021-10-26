int f[10000001];
int primeDivisor(int a, int b, int k)
{
    if (k > 10)return 0;
    int s=0;
    for(int i = 2; i <= b; i++)
        f[i] = 0;
    for (int p = 2; p <= b; p++) 
        if (f[p] == 0) 
            for (int i = p; i <= b; i += p) 
                f[i]++;
    for (int i = a; i <= b; i++) 
        if (f[i] == k)s++;
    return s;
}
