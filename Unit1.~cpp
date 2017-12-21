//---------------------------------------------------------------------------

#include <vcl.h>
#pragma hdrstop
#include <mmsystem.h>

#include "Unit1.h"
//---------------------------------------------------------------------------
#pragma package(smart_init)
#pragma resource "*.dfm"
TForm1 *Form1;


char p1,p2,p3,p4,p5,p6,p7,p8,p9;
//numeracja pola w grze (ich zawartosc p1='n' nic, J =janusz M=murlock)
char kto;

void sprawdz()
{
        if     ((p1==p2 && p2==p3 && p1!='n') ||
                (p4==p5 && p5==p6 && p4!='n') ||
                (p7==p8 && p8==p9 && p7!='n') ||
                (p1==p4 && p4==p7 && p7!='n') ||
                (p2==p5 && p5==p8 && p2!='n') ||
                (p3==p6 && p6==p9 && p3!='n') ||
                (p1==p5 && p5==p9 && p1!='n') ||
                (p3==p5 && p5==p7 && p3!='n'))
        {
                char * w;
                if(kto=='m')
                {
                w="Wygra³y januszki";
                sndPlaySound("sound\\Janusz.wav", SND_ASYNC);
                }
                else
                {
                w="Wygra³y Murlocki";
                sndPlaySound("sound\\Murloc.wav", SND_ASYNC);
                }

                Application->MessageBox(w, "Koniec gry", MB_OK);
        }
        else if ((p1!='n' && p2!='n' && p3!='n' &&
                  p4!='n' && p5!='n' && p6!='n' &&
                  p7!='n' && p8!='n' && p9!='n' ))
             {
                char * w;
                w="Remis";
                Application->MessageBox(w, "Koniec gry", MB_OK);
             }



}

//---------------------------------------------------------------------------
__fastcall TForm1::TForm1(TComponent* Owner)
        : TForm(Owner)
{
}
//---------------------------------------------------------------------------


void __fastcall TForm1::FormCreate(TObject *Sender)
{
        pole1-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole2-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole3-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole4-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole5-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole6-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole7-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole8-> Picture -> LoadFromFile("img/Pusty.bmp");
        pole9-> Picture -> LoadFromFile("img/Pusty.bmp");
        tura-> Picture -> LoadFromFile("img/JanuszS.bmp");

        p1='n'; p2='n'; p3='n';
        p4='n'; p5='n'; p6='n';
        p7='n'; p8='n'; p9='n';

        kto='j';

        pole1->Enabled=true;
        pole2->Enabled=true;
        pole3->Enabled=true;
        pole4->Enabled=true;
        pole5->Enabled=true;
        pole6->Enabled=true;
        pole7->Enabled=true;
        pole8->Enabled=true;
        pole9->Enabled=true;

}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole1Click(TObject *Sender)
{
        if(p1=='n')
        {
                if(kto=='j')
                {
                pole1->Picture->LoadFromFile("img/Janusz.bmp");
                p1='j';
                kto='m';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole1->Picture->LoadFromFile("img/Murlock.bmp");
                p1='m';
                kto='j';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole1->Enabled=False;
        sprawdz();
        }


}
//---------------------------------------------------------------------------

void __fastcall TForm1::pole2Click(TObject *Sender)
{
        if(p2=='n')
        {
                if(kto=='j')
                {
                pole2->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p2='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole2->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p2='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole2->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole3Click(TObject *Sender)
{
        if(p3=='n')
        {
                if(kto=='j')
                {
                pole3->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p3='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole3->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p3='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole3->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole4Click(TObject *Sender)
{
        if(p4=='n')
        {
                if(kto=='j')
                {
                pole4->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p4='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole4->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p4='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole4->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole5Click(TObject *Sender)
{
        if(p5=='n')
        {
                if(kto=='j')
                {
                pole5->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p5='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole5->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p5='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole5->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole6Click(TObject *Sender)
{
        if(p6=='n')
        {
                if(kto=='j')
                {
                pole6->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p6='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole6->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p6='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole6->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole7Click(TObject *Sender)
{
        if(p7=='n')
        {
                if(kto=='j')
                {
                pole7->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p7='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole7->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p7='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole7->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole8Click(TObject *Sender)
{
        if(p8=='n')
        {
                if(kto=='j')
                {
                pole8->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p8='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole8->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p8='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole8->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------
void __fastcall TForm1::pole9Click(TObject *Sender)
{
        if(p9=='n')
        {
                if(kto=='j')
                {
                pole9->Picture->LoadFromFile("img/Janusz.bmp");
                kto='m';
                p9='j';
                tura->Picture->LoadFromFile("img/MurlockS.bmp");
                }
                else
                {
                pole9->Picture->LoadFromFile("img/Murlock.bmp");
                kto='j';
                p9='m';
                tura->Picture->LoadFromFile("img/JanuszS.bmp");

                }
        pole9->Enabled=False;
        sprawdz();
        }
}
//---------------------------------------------------------------------------




