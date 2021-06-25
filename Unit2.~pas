unit Unit2;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, ExtCtrls, StdCtrls;

type
  TForm1 = class(TForm)
    Image1: TImage;
    Timer1: TTimer;

    procedure timer1timer(sender:tobject);

  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;
  t,t1,t2,t3,t4,t5,t6,t7,t8,t9,t10,t11,x1,y1,x2,y2,x3,y3,x4,y4,faza,faza2,faza_placa,faza_cpu,x_test,y_test,sin_placa: integer;
  t_brat: integer = 63;
  t_placa: integer = 0;
  x_delta, y_delta, x_delta1, y_delta1: integer;

  avans,avans2,avans3,i: Integer;

  directie: boolean= true;
  directie1: boolean= false;

  const

  t1max=500;

  r1=60;
  r2=50;
  r3=30;
  x0=200;
  y0=250;
  
  Y_offset_banda = -35;
  X_offset_banda = 0;

  Y_offset_banda_2 = -200;
  X_offset_banda_2 = 30;

  Y_offset_banda_3 = -125;
  X_offset_banda_3 = 925;


implementation
      procedure tform1.timer1timer(sender:tobject);
    begin
      with  form1.Image1.canvas do
        begin

             //fundal
        pen.Width:=1;
        pen.Color:=clblack;
        //brush.Color:=RGB(153, 194, 255);
        brush.Color:=RGB(204, 204, 255);
        polygon([point(50,0),point(1200,0),point(1200,200),point(50,200)]);
        brush.Color:= RGB(51, 102, 153);
        polygon([point(50,200),point(1200,200),point(1200,520),point(10,520)]);
        brush.Color:= clpurple;
        polygon([point(50,0),point(50,200),point(10,520),point(0,520),point(0,0)]);

      pen.color:=rgb(22,114,50);
Brush.Color := clwhite;
font.color:=clBlack;
font.size:=10;
textout(20,20,'Nitu Andreea');

//BANDA TRANSPORTOARE

//corp banda

Pen.Color:=clBlack;
Brush.Color:=rgb(132, 162, 179);
polygon([Point(345+X_offset_banda,400+Y_offset_banda),Point(350+X_offset_banda,410+Y_offset_banda),Point(323+X_offset_banda,510+Y_offset_banda),Point(320+X_offset_banda,500+Y_offset_banda)]);
polygon([Point(345+X_offset_banda_2,400+Y_offset_banda_2),Point(350+X_offset_banda_2,410+Y_offset_banda_2),Point(323+X_offset_banda_2,510+Y_offset_banda_2),Point(320+X_offset_banda_2,500+Y_offset_banda_2)]);
polygon([Point(345+X_offset_banda_3,400+Y_offset_banda_3),Point(350+X_offset_banda_3,410+Y_offset_banda_3),Point(323+X_offset_banda_3,510+Y_offset_banda_3),Point(320+X_offset_banda_3,500+Y_offset_banda_3)]);
Pen.Color:=rgb(130, 158, 173);
    Brush.Color:= rgb(130, 158, 173);
    ellipse(325+X_offset_banda,424+Y_offset_banda,350+X_offset_banda,399+Y_offset_banda);


    ellipse(325+X_offset_banda_2,424+Y_offset_banda_2,350+X_offset_banda_2,399+Y_offset_banda_2);
    ellipse(325+X_offset_banda_3,424+Y_offset_banda_3,350+X_offset_banda_3,399+Y_offset_banda_3);
    Brush.Color := rgb(155, 189, 207);
polygon([Point(345+X_offset_banda,400+Y_offset_banda),Point(320+X_offset_banda,500+Y_offset_banda),Point(0+X_offset_banda,500+Y_offset_banda),Point(25+X_offset_banda,400+Y_offset_banda)]);

polygon([Point(345+X_offset_banda_2,400+Y_offset_banda_2),Point(320+X_offset_banda_2,500+Y_offset_banda_2),Point(0+X_offset_banda_2,500+Y_offset_banda_2),Point(25+X_offset_banda_2,400+Y_offset_banda_2)]);
polygon([Point(345+X_offset_banda_3,400+Y_offset_banda_3),Point(320+X_offset_banda_3,500+Y_offset_banda_3),Point(0+X_offset_banda_3,500+Y_offset_banda_3),Point(25+X_offset_banda_3,400+Y_offset_banda_3)]);
Pen.Color:=clBlack;



    Pen.Color:=clBlack;

//animatie banda

             //numarul de linii verticale
for i:=0   to 9   do

begin
 avans:=avans+1;

            //distanta intre liniile verticale
moveto(25+X_offset_banda+i*32+avans2,400+Y_offset_banda);
lineto(0+X_offset_banda+i*32+avans2,500+Y_offset_banda);

moveto(25+X_offset_banda_2+i*32+avans2,400+Y_offset_banda_2);
lineto(0+X_offset_banda_2+i*32+avans2,500+Y_offset_banda_2);

moveto(25+X_offset_banda_3+i*32+avans2,400+Y_offset_banda_3);
lineto(0+X_offset_banda_3+i*32+avans2,500+Y_offset_banda_3);

              //avans>= x , x seteaza viteza benzii
              //modifci in ambele if- uri
if avans>=5 then
avans2:=avans2+1;
if avans>=5 then
avans:=0 ;
            //distanta de deplasare a benzii
if avans2>30 then
avans2:=0;
end;


    //animatie banda


 //lateral banda
   Brush.Color:=rgb(135, 123, 138);
    //lateral banda static
   roundrect(0+X_offset_banda,500+Y_offset_banda,310+X_offset_banda,525+Y_offset_banda,0,0);
   Brush.Color:=rgb(135, 123, 138);
   ellipse(25+X_offset_banda,500+Y_offset_banda,50+X_offset_banda,525+Y_offset_banda);
   Brush.Color:=rgb(135, 123, 138);
   ellipse(302+X_offset_banda,500+Y_offset_banda,327+X_offset_banda,525+Y_offset_banda);
   Brush.Color:=rgb(135, 123, 138);


    Brush.Color:=rgb(135, 123, 138);
    roundrect(0+X_offset_banda_2,500+Y_offset_banda_2,310+X_offset_banda_2,525+Y_offset_banda_2,0,0);
    Brush.Color:=rgb(135, 123, 138);
    ellipse(25+X_offset_banda_2,500+Y_offset_banda_2,50+X_offset_banda_2,525+Y_offset_banda_2);
    Brush.Color:=rgb(135, 123, 138);
    ellipse(302+X_offset_banda_2,500+Y_offset_banda_2,327+X_offset_banda_2,525+Y_offset_banda_2);
    Brush.Color:=rgb(135, 123, 138);

    Brush.Color:=rgb(135, 123, 138);
    roundrect(0+X_offset_banda_3,500+Y_offset_banda_3,310+X_offset_banda_3,525+Y_offset_banda_3,0,0);
    Brush.Color:=rgb(135, 123, 138);
    ellipse(25+X_offset_banda_3,500+Y_offset_banda_3,50+X_offset_banda_3,525+Y_offset_banda_3);
    Brush.Color:=rgb(135, 123, 138);
    ellipse(302+X_offset_banda_3,500+Y_offset_banda_3,327+X_offset_banda_3,525+Y_offset_banda_3);
    Brush.Color:=rgb(135, 123, 138);

    Pen.Color:=clBlack;
   //animatie miscare lateral banda

   //partea 1 a segmentului


    x1:=round(37+X_offset_banda +10*cos(t/10));
    y1:=trunc(512+Y_offset_banda +10*sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda,512+Y_offset_banda);
    //construirea segmentului catre punctul de pe cerc
    lineto(x1,y1);
    //partea 2 a segmentului
    x2:=round(37+X_offset_banda +10*-cos(t/10));
    y2:=trunc(512+Y_offset_banda + 10*-sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda,512+Y_offset_banda);
    lineto(x2,y2);





    x1:=round(314+X_offset_banda +10*cos(t/10));
    y1:=trunc(512+Y_offset_banda +10*sin(t/10));
    //mijlocul comun al segmentului
    moveto(314+X_offset_banda,512+Y_offset_banda);
    //construirea segmentului catre punctul de pe cerc
    lineto(x1,y1);
    //partea 2 a segmentului
    x2:=round(314+X_offset_banda +10*-cos(t/10));
    y2:=trunc(512+Y_offset_banda + 10*-sin(t/10));
    //mijlocul comun al segmentului
    moveto(314+X_offset_banda,512+Y_offset_banda);
    lineto(x2,y2);
    //rl este lungimea liniei ce se roteste

    x2:=round(37+X_offset_banda_2 +10*cos(t/10));
    y2:=trunc(512+Y_offset_banda_2 +10*sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda_2,512+Y_offset_banda_2);
    //construirea segmentului catre punctul de pe cerc
    lineto(x2,y2);
    //partea 2 a segmentului
    x3:=round(37+X_offset_banda_2 +10*-cos(t/10));
    y3:=trunc(512+Y_offset_banda_2 + 10*-sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda_2,512+Y_offset_banda_2);
    lineto(x3,y3);

    x2:=round(314+X_offset_banda_2 +10*cos(t/10));
    y2:=trunc(512+Y_offset_banda_2 +10*sin(t/10));
    //mijlocul comun al segmentului
    moveto(314+X_offset_banda_2,512+Y_offset_banda_2);
    //construirea segmentului catre punctul de pe cerc
    lineto(x2,y2);
    //partea 2 a segmentului
    x3:=round(314+X_offset_banda_2 +10*-cos(t/10));
    y3:=trunc(512+Y_offset_banda_2 + 10*-sin(t/10));
    //mijlocul comun al segmentului
    moveto(314+X_offset_banda_2,512+Y_offset_banda_2);
    lineto(x3,y3);

    x2:=round(37+X_offset_banda_3 +10*cos(t/10));
    y2:=trunc(512+Y_offset_banda_3 +10*sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda_3,512+Y_offset_banda_3);
    //construirea segmentului catre punctul de pe cerc
    lineto(x2,y2);
    //partea 2 a segmentului
    x3:=round(37+X_offset_banda_3 +10*-cos(t/10));
    y3:=trunc(512+Y_offset_banda_3 + 10*-sin(t/10));
    //mijlocul comun al segmentului
    moveto(37+X_offset_banda_3,512+Y_offset_banda_3);
    lineto(x3,y3);

   pen.Color:= clBlack;
   pen.Width:=7;
   moveto(445, 205);
   lineto(380, 519);

   moveto(475, 205);
   lineto(410, 519);

   pen.Width:=1;

   

   // Baza bratului
   roundrect(360 + t1, 479 - 5*t1, 430 + t1, 519 - 5*t1, 0, 0);
   polygon([point(445 + t1, 505 - 5*t1), point(445 + t1, 465 - 5*t1),point(430 + t1, 479 - 5*t1),point(430 + t1,519 - 5*t1)]);
   polygon([point(360 + t1, 479 - 5*t1), point(430 + t1, 479 - 5*t1), point(445 + t1, 465 - 5*t1), point(375 + t1, 465 - 5*t1)]);

   // Piciorul bratului
   roundrect(390 + t1, 475 - 5*t1, 420 + t1, 400 - 5*t1, 0, 0);
   polygon([point(420 + t1, 475 - 5*t1), point(430 + t1, 465 - 5*t1),point(430 + t1, 390 - 5*t1),point(420 + t1,400 - 5*t1)]);
   polygon([point(420 + t1, 400 - 5*t1), point(430 + t1, 390 - 5*t1), point(400 + t1, 390 - 5*t1), point(390 + t1, 400 - 5*t1)]);

   // Masa de asamblare

   polygon([point(460, 350), point(660, 350), point(710, 250), point(510, 250)]);
   roundrect(460,350,660,360,0,0);
   polygon([point(660, 350), point(660, 360), point(710, 260), point(710, 250)]);
   roundrect(480,360,500,400,0,0);
   polygon([point(500, 400), point(505, 390), point(505, 360), point(500, 360)]);
   roundrect(620,360,640,400,0,0);
   polygon([point(640, 400), point(645, 390), point(645, 360), point(640, 360)]);
   polygon([point(680, 320), point(688, 320), point(688, 305)]);

   // Brat 1
   roundrect(405 + t1, 397 - 5*t1, 415 + t1, 300 - 5*t1, 0, 0);

   ellipse(400 + t1, 280 - 5*t1, 420 + t1, 300 - 5*t1);
   ellipse(403 + t1, 283 - 5*t1, 417 + t1, 297 - 5*t1);

   // Brat 2
   //roundrect(320 + t1 + t2, 285 - 5*t1 + t2, 400 + t1, 295 - 5*t1, 0, 0);

   //Pen.Color:=rgb(135, 123, 138);
   Pen.Width:=8;
   Pen.Color:=clBlack;
   x4:=round(410+150*cos(-t_brat/20));
   y4:=trunc(290+150*sin(-t_brat/20));
   moveto(410 + t1, 290 - 5*t1);
   lineto(x4 + t1, y4 - 5*t1);
   Pen.Width:=1;

   // -----Placa de baza-----
   Brush.Color:=rgb(2, 79, 23);
   polygon([Point(5 + t6 + x_delta + t7, 430 + y_delta - 5*t7 + t3), Point(45 + t6 + x_delta + t7, 430 + y_delta - 5*t7 + t3), Point(55 + t6 + x_delta + t7, 390 + y_delta - 5*t7 + t3), Point(15 + t6 + x_delta + t7, 390 + y_delta - 5*t7 + t3)]);
   Pen.Color:=clBlack;
   Pen.Width:=2;
   moveto(38 + t6 + x_delta + t7, 395 + y_delta - 5*t7 + t3);
   lineto(35 + t6 + x_delta + t7, 410 + y_delta - 5*t7 + t3);
   moveto(42 + t6 + x_delta + t7, 395 + y_delta - 5*t7 + t3);
   lineto(39 + t6 + x_delta + t7, 410 + y_delta - 5*t7 + t3);
   moveto(46 + t6 + x_delta + t7, 395 + y_delta - 5*t7 + t3);
   lineto(43 + t6 + x_delta + t7, 410 + y_delta - 5*t7 + t3);
   moveto(50 + t6 + x_delta + t7, 395 + y_delta - 5*t7 + t3);
   lineto(47 + t6 + x_delta + t7, 410 + y_delta - 5*t7 + t3);
   font.size:=5;
   font.color:=clWhite;
   textout(11 + t6 + x_delta + t7, 415 + y_delta - 5*t7 + t3,'MOBO');
   Brush.Color:=rgb(135, 123, 138);
   Pen.Width:=1;
   // -------------------------

   // -----Procesor-----
   Brush.Color:=rgb(209, 206, 111);
   polygon([Point(-15 + t9 + x_delta1 + t11, 440 + Y_offset_banda_2 + y_delta1 - 5*t11 + t10), Point(-5 + t9 + x_delta1 + t11, 440 + Y_offset_banda_2 + y_delta1 - 5*t11 + t10), Point(0 + t9 + x_delta1 + t11, 430 + Y_offset_banda_2 + y_delta1 - 5*t11 + t10), Point(-10 + t9 + x_delta1 + t11,  430 + Y_offset_banda_2 + y_delta1 - 5*t11 + t10)]) ;
   Brush.Color:=rgb(135, 123, 138);
   // -------------------------
   
   // Brat cartezian
   roundrect(480, 25, 1000, 35, 0, 0);
   Brush.Color:=rgb(135, 123, 138);
   roundrect(950 + t4, 20, 1000 + t4, 40, 0, 0);
   roundrect(960 + t4, 40, 990 + t4, 100, 0, 0);
   roundrect(970 + t4, 100, 980 + t4, 120 + t5, 0, 0);
   roundrect(965 + t4, 120 + t5, 985 + t4, 130 + t5, 0, 0);

   t:=t+1;

     case faza of
     1: // Coboara bratul pana la masa
      begin
        t_brat:=t_brat+1;
        if(t_brat = 78) then
          begin
            x_delta:=round(410+150*cos(-78/20));
            y_delta:=trunc(290+150*sin(-78/20));
            t_brat:=t_brat;
            faza:=2;
          end;
       end;
     2: // Ia placa de baza de pe prima banda
      begin
        t_brat:=t_brat-1;
        
        x_delta:=round(410+150*cos(-78/20));
        y_delta:=trunc(290+150*sin(-78/20));
        x_delta:=x4-x_delta;
        y_delta:=y4-y_delta;
        if(t_brat = 63) then
          begin
            t_brat:=t_brat;
            faza:=3;
          end;
      end;
     3: // Se misca pana intre benzi
      begin
        t1:=t1+1;
        t7:=t7+1;
        if(t1=20) then
          begin
            t1:=t1;
            t7:=t7;
            faza:=4;
          end;
      end;
     4: // Aseaza placa de baza pe masa
      begin
        t_brat:=t_brat-1;
        x_delta:=round(410+150*cos(-78/20));
        y_delta:=trunc(290+150*sin(-78/20));
        x_delta:=x4-x_delta;
        y_delta:=y4-y_delta;
        if(t_brat = -18) then
          begin
            t_brat:=t_brat;
            x_delta:=x_delta;
            y_delta:=y_delta;
            faza_cpu:=1;
            faza:=5;
          end;
       end;
     5: // Lasa placa si ridica bratul
      begin
        t_brat:=t_brat+1;
        if(t_brat = 63) then
          begin
            t_brat:=t_brat;
            faza:=6;
          end;
      end;
     6: // Se misca la a doua banda
      begin
        t1:=t1+1;
        if(t1=32) then
          begin
            t1:=t1;
            faza:=0;
          end;
      end;
     7: // Coboara bratul
      begin
        t_brat:=t_brat+1;
        if(t_brat = 77) then
          begin
            t_brat:=t_brat;
            faza:=8;
          end;
      end;
     8: // Ia procesorul si ridica bratul
      begin
        t_brat:=t_brat-1;
        x_delta1:=round(410+150*cos(-77/20));
        y_delta1:=trunc(295+150*sin(-77/20));
        x_delta1:=x4-x_delta1;
        y_delta1:=y4-y_delta1;
        if(t_brat = 63) then
          begin
            t_brat:=t_brat;
            faza2:=1;
            faza:=9;
          end;
      end;
     9: // Se misca pana intre benzi
      begin
        t1:=t1-1;
        t11:=t11-1;
        if(t1=24) then
          begin
            t1:=t1;
            t11:=t11;
            faza:=10;
          end;
      end;
     10:  // Aseaza procesorul pe placa de baza de pe masa
      begin
        t_brat:=t_brat-1;
        x_delta1:=round(410+150*cos(-77/20));
        y_delta1:=trunc(295+150*sin(-77/20));
        x_delta1:=x4-x_delta1;
        y_delta1:=y4-y_delta1;
        if(t_brat = -24) then
          begin
            t_brat:=t_brat;
            x_delta1:=x_delta1;
            y_delta1:=y_delta1;
            faza:=11;
          end;
       end;
     11:  // Ridica bratul de pe masa
      begin
        t_brat:=t_brat+1;
        if(t_brat = 63) then
          begin
            t_brat:=t_brat;
            faza:=12;
          end;
      end;
     12:  // Se misca inapoi la prima banda
      begin
        t1:=t1-1;
        if(t1=0) then
          begin
            t1:=0;
            faza:=0;
          end;
      end;
     end;

     case faza_placa of
     0:
      begin
        t6:=t6+3;
        if(t6=240) then
          begin
            faza:=1;
            t6:=240;
            faza_placa:=2;
          end;
      end;
     1:
      begin
        t6:=t6+3;
        if(t6=1119) then
          begin
            //faza:=1;
            t6:=0;
            t3:=0;
            t7:=0;
            t1:=0;
            x_delta:=0;
            y_delta:=0;
            faza_placa:=0;
          end;  
      end;
     end;

     case faza_cpu of
     1:
      begin
        t9:=t9+3;
        if(t9=333) then
          begin
            faza:=7;
            t9:=t9;
            faza_cpu:=0;
          end;
      end;
     2:
      begin
        t9:=t9+3;
        if(t9=1119) then
          begin
            t9:=0;
            t10:=0;
            t11:=0;
            x_delta1:=0;
            y_delta1:=0;
            faza_cpu:=0;
          end;
      end;
     end;

     case faza2 of
     1:
      begin
        t4:=t4-4;
        if(t4=-480) then
          begin
            t4:=t4;
            faza2:=2;
          end;
      end;
     2:
      begin
        t5:=t5+4;
        if(t5=180) then
          begin
            t5:=t5;
            faza2:=3;
          end;
      end;
     3:
      begin
        t5:=t5-4;
        t3:=t3-4;
        t10:=t10-4;
        if(t5=0) then
          begin
            t5:=t5;
            t3:=t3;
            t10:=t10;
            faza2:=4;
          end;
      end;
     4:
      begin
        t4:=t4+4;
        t6:=t6+4;
        t9:=t9+4;
        if(t4=0) then
          begin
            t6:=t6;
            t9:=t9;
            t5:=t5;
            faza2:=5;
          end;
      end;
     5:
      begin
        t5:=t5+4;
        t3:=t3+4;
        t10:=t10+4;
        if(t5=180) then
          begin
            t5:=t5;
            t3:=t3;
            t10:=t10;
            faza2:=6;
            faza_cpu:=2;
            faza_placa:=1;
          end;  
      end;
     6:
      begin
        t5:=t5-4;
        if(t5=0) then
          begin
            t5:=t5;
            faza2:=0;
          end;
      end;
     end;
    
      

                end;
           end;

{$R *.dfm}


end.
