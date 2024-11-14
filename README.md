#include <iostream>

using namespace std;

int main()
{
    float Pd1, Pd2, I, V, Cont;
    int R=10;

    cout<< "INGRESE EL VALOR DE LA CORRIENTE: "<<endl;
    cin>>I;
    cout<< "INGRESE EL VALOR DEL VOLTAJE: "<<endl;
    cin>>V;


    Pd1= (I*I)*R;
    cout<< "SU VALOR DE PD1 ES: "<<Pd1<<endl;


    V=(I*R);
    Pd2= (V*V)/R;
    cout<< "SU VALOR DE PD2 ES: "<<Pd2<<endl;

    if (Pd1==Pd2) {
        cout<< "SON IGUALES"<<endl;

    }
    else if (Pd1>22.4){
    cout<< "CORTO CIRCUITO"<<endl;
    }
    else
    cout<< "FUNCIONA CORRECTAMENTE"<<endl;

    return 0;
}
