# direct_design
В ходе рефакторинга решалась проблема большого метода. 
Для повышения читабельности кода он был разбит на более мелкие методы,
посредством вынесения методов. Таким образом, общий объём кода практически не изменился,
но в результате удалось избавиться от нескольких временных переменных:
	vorota1, vorota2: TTime;
	cur_date: TDate;
	Counter: Word;

И дублирования кода, вынесением методов: 
procedure TForm1.ChallDrawGate(var vorota1_date: TDate; var TimeShift: TTime;
                               var mas:  SortArray);

procedure TForm1.Shift(var TimeShift: TTime);