// Linguagem c++, pode ser utilizado sites como https://www.onlinegdb.com/online_c++_compiler# para compilar, a ideia é que a pessoa coloque os dados e receba o retorno de seu investimento de acordo com a duração dele. É considerado que a cada um real investido gere trinta visualizações originais, ou seja, 0,033 centavos cada. Também foi levado em conta que os cliques, compartilhamentos e visualizações advindas dele não possuem custo.

// Não é armazenado as informações, funciona mais como uma calculadora detalhada relacionada a investimento de anúncios.

#Maysa-Lemes
#include <iostream>
#include<string.h>
using namespace std; 
 
int main()
{
string na, nc;
float  vo, vc, clic, d1, dt;
int ind, vt, co;

    cout<<"CADASTRO DE ANÚNCIOS\n\n";

    cout<<"Nome do Anúncio: ";
    cin>>na;
    cout<<endl;

    cout<<"Cliente: ";
    cin>>nc;
    cout<<endl;
   
    cout<<"Data de Início: ";  //é indicado colocar os dados assim: ddmmaa, exemplo: 160521.
    cin>>d1;
    cout<<endl;

    cout<<"Data de Término: ";
    cin>>dt;
    cout<<"\n";

    cout<<"Investimento por dia: "; 
    cin>>ind;
    cout<<endl;

    cout<<"Valor total investido: "<<vt; // irá ser calculado contando dia, mês e ano, então será necessário fazer uma conversão para o valor correto.
        vt =(dt-d1)*ind;
    cout<<vt<<"\n";
    
    cout<<"Quantidade máxima de visualizações: ";
        vo = (vt /1*30);
        vc = (vo/50)*40;
    cout<<(vo + vc )<< endl;
    
    cout<<"Quantidade máxima de cliques: ";
        clic =(vo + vc)/8;
    cout<<clic<<"\n";
    
    cout<<"Quantidade máxima de compartilhamentos: ";
        co = (vo+vc)/50;
    cout<<co;

return 0;
}
