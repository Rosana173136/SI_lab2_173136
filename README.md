# SI_lab2_173136


### Control Flow Graph
Фотографија од control flow graph-ot https://imgur.com/a/ztu9jgQ

3.1 Иницијализација на променливата i во рамката 

3.2 Услов во рамката (i < timesList.size())   

3.3 Зголемување на променливата i во рамката

### Цикломаткса комплексност
Во овој граф имаме 24 јазли и 34 ребра па зато цикломатската комплексност е: (34-24)+2 = 8 исто така овој резултат можеме да го добиеме и со броење на предикатни јазли(7) и додавање 1: 7+1 = 8.

### Тест случаи според критериумот Multicond
Имаме 4 if услови со multiple conditions:
if (hr < 0 || hr > 24)
T|T (hr =23 mins =59 sec= 59)
T|F (hr = 23 mins =59 sec=59 )
F|T (hr =25 mins =00 sec= 00)
F|F(hr =26 mins =59 sec=59 )

if (min < 0 || min > 59)
T|T (hr =23 mins =59 sec= 00)
T|F (hr =23 mins =59 sec=69 )
F|T (hr =23 mins =69 sec=59 )
F|F (hr =24 mins =-5 sec=60 )

if (sec >= 0 && sec <= 59)
T&T (hr =23 mins =00 sec=59 )
T&F (hr =23 mins =59 sec=61 )
F&T (hr =20 mins =-5 sec=10 )
F&F (hr = 25mins =63 sec=-6 )

if (hr == 24 && min == 0 && sec == 0)
T&T&T (hr =24 mins =00 sec=00 )
T&T&F (hr =24 mins =00 sec=16 )
T&F&T (hr =24 mins =30 sec=00 )
T&F&F (hr =24 mins =67 sec=55 )
F&T&T (hr =25 mins =00 sec=00 )
F&T&F (hr =-24 mins =00 sec=00 )
F&F&T (hr =25 mins =67 sec= 00)
F&F&F (hr =25 mins =61 sec=63 )


### Тест случаи според критериумот Every branch


